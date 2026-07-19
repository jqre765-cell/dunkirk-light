# Git Workflow

This is the working agreement for collaborating on Dunkirk Light.

## First-Time Setup

Clone the repository:

```powershell
git clone https://github.com/jqre765-cell/dunkirk-light.git
cd dunkirk-light
```

Confirm your identity:

```powershell
git config user.name
git config user.email
```

If either value is missing:

```powershell
git config user.name "Your Name"
git config user.email "your-email@example.com"
```

## Daily Routine

Before starting work:

```powershell
git status --short --branch
git pull
```

Create a branch for a meaningful change:

```powershell
git switch -c codex/add-player-movement
```

Check what changed:

```powershell
git status --short
git diff
```

Commit a complete piece of work:

```powershell
git add README.md
git commit -m "Document Git workflow"
```

Push your branch:

```powershell
git push -u origin codex/add-player-movement
```

## Commit Checklist

Before each commit:

- `git status --short` shows only files you expect.
- `git diff` has no accidental edits, secrets, or temporary files.
- The program still opens, builds, or passes the most relevant test available.
- The commit message says what changed in plain language.

## Branch Rules

- `main` should stay usable.
- Use short-lived branches for game features, experiments, and bug fixes.
- Pull before starting and before pushing.
- Do not force-push shared branches.
- If Git reports a conflict, stop and resolve it carefully instead of guessing.

## Good Commit Message Examples

```text
Add player movement prototype
Fix enemy spawn timer reset
Document project controls
Ignore local editor files
```

## When Working With Codex

Ask Codex to:

- Check Git status before edits.
- Make a focused change.
- Run the relevant verification.
- Commit with a clear message.
- Push when the change is ready to share.
