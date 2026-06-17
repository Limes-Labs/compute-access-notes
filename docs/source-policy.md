# Source Policy

Last checked: 2026-06-17.

## Rule

Every factual program claim should have:

- `source_url`
- `source_title`
- `date_checked`
- `status`
- `confidence`

If a claim does not have a public source, mark it as Limes interpretation or `needs_verification`.

## Status Values

| Status | Meaning |
| --- | --- |
| `confirmed_public` | Supported by a public source checked by Limes. |
| `needs_verification` | Plausible or useful, but not confirmed by reviewed public sources. |
| `stale` | Source exists but may be outdated or superseded. |
| `contact_pending` | A question has actually been sent and is awaiting response. Requires a contact-log row. |
| `deprecated` | Do not rely on this claim; kept only for historical context. |

## Contact Log Rule

Do not claim contact progress, partnership, eligibility, or access unless there is a public-safe record in [../data/contact-log.csv](../data/contact-log.csv).

Draft emails and planned questions are not contact progress.

## Public-Safe Notes

Public notes should avoid:

- private names unless permission exists
- email contents beyond a short non-sensitive summary
- claims of endorsement
- legal conclusions
- guessing hidden eligibility requirements

When in doubt, write "needs verification" and link the official helpdesk or call page.
