# Git Workflow PoC — Malafi

Proof of concept for the Malafi Git Workflow Plan (GitFlow with Environment branches).

| Branch | Type | Receives from |
|---|---|---|
| `production` | long-lived | `release/*`, `hotfix/*` |
| `preprod` | long-lived | `release/*`, `hotfix/*` |
| `staging` | long-lived | `release/*`, `hotfix/*` |
| `develop` | long-lived (default) | `feature/*`, back-merges |
| `release/vX.Y.Z` | short-lived | `bugfix/*` |
| `feature/<TICKET>-<desc>` | short-lived | — |
| `bugfix/<TICKET>-<desc>` | short-lived | — |
| `hotfix/vX.Y.Z` | short-lived | — |

PR titles follow Conventional Commits: `feat(MAL-123): add appointments list`.
