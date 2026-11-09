# skills
Skills for real engineering. Steps in building AI factory

| Skill | What it does |
|---|---|
| [`ship`](docs/ship.md) | A ship gate for coding agents. A coordinator drives, an independent judge on the strongest model finds production blockers (tenant data leaks, data loss, N+1, latency, new dependencies, abuse and cost), Sonnet fixers fix them, and the judge reviews again until none are left. Then it opens a PR, or pushes a small clean change straight to main where allowed. Also reviews open PRs, and can run review-only in CI. |
