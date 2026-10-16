# Contributing to the BulletinAI use-case dataset

This repository is the open data companion to [BulletinAI](https://bulletinai.app). Additions and corrections are welcome as pull requests and GitHub issues.

Open an issue to suggest a use case, report a broken source link, or fix a credit. Open a pull request to add or edit records in [`data/usecases.json`](data/usecases.json). If a change introduces a new outcome, platform, role, difficulty, or status, update [`data/categories.md`](data/categories.md) in the same pull request.

## What belongs here

A good entry is a real playbook someone can follow: a concrete outcome, the platform it runs on, the steps, and a public source that already describes it. Prefer vendor documentation, official template galleries, and maintained community lists.

Write the playbook in your own short steps. Link and credit the original source. Do not paste long excerpts from the source.

## Entry schema

`data/usecases.json` is a JSON array. Each element is one use case. Field order below is the order used in the file.

| Field | Required | Type | Rules |
| --- | --- | --- | --- |
| `id` | yes | string | Stable unique slug. Lowercase kebab-case, prefixed with the next zero-padded number (`01-`, `02-`, …). Keep it once published: BulletinAI page URLs use this id (`https://bulletinai.app/u/{id}`). |
| `title` | yes | string | Short name of the use case. |
| `outcome` | yes | string | One value from Outcomes in [`data/categories.md`](data/categories.md). |
| `platforms` | yes | array of strings | One or more platforms. Use the names in the taxonomy. Name the product when the taxonomy’s “Other” bucket applies (for example `Lindy`, `Relevance AI`, `Microsoft Copilot`). |
| `role` | yes | string | One value from Roles. |
| `difficulty` | yes | string | `No-code`, `Low-code`, or `Technical`. |
| `setup_time_estimate` | yes | string | A rough estimate, marked as an estimate, such as `~10m (estimate)` or `~1h (estimate)`. |
| `tools` | yes | array of strings | Products and accounts the steps actually use. |
| `playbook` | yes | array of strings | Ordered steps. One action per string. Three steps is typical. |
| `source_url` | yes | string | `https` URL of the original source. No affiliate ids, referral codes, or tracking query parameters. |
| `source_credit` | yes | string | Human-readable credit: publisher and page or list name. |
| `status` | yes | string | `community` (unverified), `official example` (from the vendor), or `verified` (tested by BulletinAI). New submissions from outside BulletinAI should use `community`. |
| `notes` | yes | string | Caveats a reader needs (license requirements, “not medical advice”, security notes). Use `""` when there is nothing to add. |
| `bulletin_url` | yes | string | `https://bulletinai.app/u/{id}` when that page exists. Use `""` for an entry that is not on the site yet. |

Allowed `difficulty` values match the taxonomy labels, without the parenthetical explanation:

- `No-code` — chat only
- `Low-code` — connect apps or import a template
- `Technical` — self-host or API keys

JSON values for `status`:

- `community`
- `official example`
- `verified`

### Entry template

```json
{
  "id": "66-short-kebab-case-slug",
  "title": "Short descriptive title",
  "outcome": "Inbox & email",
  "platforms": ["ChatGPT"],
  "role": "Ops/manager",
  "difficulty": "No-code",
  "setup_time_estimate": "~10m (estimate)",
  "tools": ["ChatGPT"],
  "playbook": [
    "First concrete step.",
    "Second concrete step.",
    "What the person receives or checks."
  ],
  "source_url": "https://example.com/original-source",
  "source_credit": "Publisher — page or list name",
  "status": "community",
  "notes": "",
  "bulletin_url": ""
}
```

## Affiliate links

Do not include affiliate program URLs, referral codes, affiliate ids, or tracking parameters in `source_url`, `notes`, or anywhere else in an entry. Link the public page a reader would open, not a partner or affiliate redirect.

## Review checklist

- The JSON file parses, and the new object is inside the top-level array.
- `id` is unique.
- `outcome`, `role`, `difficulty`, and `status` use the values documented above.
- `source_url` opens the page named in `source_credit`.
- The playbook steps are specific enough to follow and are not a long copy of the source.
- `notes` records limits the source itself states (paid add-on, unverified community skill, not medical advice).
- No affiliate identifiers.

## Issues

Use an issue when you are unsure the source is public, the steps are incomplete, or you want BulletinAI to review a playbook before it is added. Include the title, outcome, platform, and source URL.
