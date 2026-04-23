# Branching Policy

## Branches

- `main`: mirror the preferred upstream and keep divergence minimal.
- `ax6600-dev`: integration branch for rebases, cherry-picks, and patch validation.
- `ax6600-stable`: release branch consumed by the firmware repository.

## Rules

- Rebase `ax6600-dev` onto `main` when the upstream moves.
- Merge or fast-forward `ax6600-stable` only after firmware-level canary validation passes.
- Record source-level patch rationale in commit messages and link back to firmware ADRs when the decision originated there.
