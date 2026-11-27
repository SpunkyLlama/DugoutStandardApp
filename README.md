# Dugout Standard App

Source for **Coach Rob's MVPs**, a youth team effort tracker (workouts, culture points, MVP race, effort scouting reports). Single self-contained page: `index.html`.

## Environments

| Environment | Source | Where |
|---|---|---|
| **Prod** | `main` | Live app artifact |
| **Dev sandbox** | feature branch | Separate dev artifact, labeled "DEV SANDBOX" |

`main` always matches what is live. Nothing reaches prod without a merged PR.

## Change workflow

1. **Issue.** Every change starts as a GitHub issue describing the problem or feature.
2. **Branch.** `issue-<number>-short-name`, cut from `main`.
3. **Dev.** The branch is published to the dev sandbox for testing. Prod is untouched.
4. **PR.** Opened against `main`, linked with `Closes #<number>`, including what changed and how it was tested.
5. **Merge.** Reviewed and merged by a maintainer.
6. **Release.** `main` is published to the prod artifact.

The dev copy differs from `main` only in its title and a header label; those are applied at publish time and never committed.
