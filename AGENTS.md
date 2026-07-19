# Codex Collaboration Rules

These rules apply whenever Codex works in this repository.

## Git Hygiene

- Check `git status --short --branch` before making changes.
- Check the current branch before editing. Use `main` only for small documentation/setup changes unless the user asks otherwise.
- Prefer a feature branch named `codex/<short-task-name>` for game code, assets, or risky changes.
- Do not overwrite or revert changes made by Ethan or jqre765-cell unless explicitly asked.
- Keep commits focused. A commit should explain one coherent change.
- Before committing, summarize changed files with `git diff --stat` and review the actual diff.
- Run available tests, builds, linters, or a relevant smoke check before committing game code.
- If verification cannot be run, say that clearly in the final update.
- After committing, push the branch when the user asks or when the task is clearly meant to update the shared GitHub repo.

## Commit Messages

Use short, plain commit subjects:

- `Add player movement prototype`
- `Fix camera bounds at map edge`
- `Document Git workflow`

For larger commits, include a body with:

- What changed
- Why it changed
- How it was tested

## Collaboration Defaults

- Keep `README.md` useful for humans who are opening the project fresh.
- Put longer process notes in `docs/`.
- Avoid committing generated build output, dependency folders, editor caches, or large binaries unless they are intentional source assets.
- Call out merge conflicts, untracked files, and risky changes early.
- Favor clarity over cleverness in game code, especially while the team is new to Git.
