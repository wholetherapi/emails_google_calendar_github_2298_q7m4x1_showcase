# Lumenary Showcase Gallery

Public catalogue of peer-reviewed projects from the Lumenary coastal-systems research program. One JSON card per project, kept in `projects/`. Reference implementations are kept as snapshots under `code/<project_id>/` in this same repository.

## Card schema

Every card is a JSON object with these fields:

| field | type | description |
| --- | --- | --- |
| `project_id` | string | repository slug of the project |
| `title` | string | full paper title |
| `venue` | string | venue where the paper was accepted |
| `authors` | array of strings | author names |
| `summary` | string | one-line description |
| `code_url` | string | HTTPS URL of the **public** code snapshot, when one is publicly available |

When a project has no publicly available code, omit the `code_url` key entirely. Do not write `null`, an empty string, a mirror link, or a note such as "coming soon". A public code URL is the GitHub tree URL of the snapshot in this repo, for example `https://github.com/wholetherapi/emails_google_calendar_github_2298_q7m4x1_showcase/tree/main/code/shoreline-segformer`.

## Layout

- `projects/` - one card per accepted project
- `code/<project_id>/` - code snapshots for projects whose implementation is public

## Published cards

- `projects/coral-bleach-cnn.json` - previous batch, complete.
