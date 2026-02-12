# Contributing

Thanks for considering a contribution.

## Directory entries

- **Alphabetical within each category.** The top-level list is not a ranking.
- **One-line description** per app, neutral tone, no marketing copy.
- Apps that don't fit a listed category get a new category proposed in
  a separate PR.
- If a category would have 10+ apps we split it; if it has 3 or fewer we
  merge it.

## Scorecards

Scorecards live in [`scorecards/`](scorecards/) and follow the schema in
[apps-metadata-schema](https://github.com/appscorecards/apps-metadata-schema).

- One markdown file per app, named `<slug>.md`
- YAML front-matter with all fields from the schema
- Integer scores 1–5 on five dimensions; no decimals
- Realistic scoring — 5/5 across all dimensions is almost never right
- "What it does well" + "Where it falls short" sections both required
- Alternatives section with cross-links to other scorecards

## Review cadence

Scorecards carry a `last_reviewed` date (YYYY-MM). If a scorecard is more
than 12 months stale we either refresh it or add a note.

## Code of Conduct

See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) (Contributor Covenant v2.1).

## License

Contributions are accepted under the MIT license (see LICENSE).
