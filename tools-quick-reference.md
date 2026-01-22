# VS Code & GitHub Desktop Quick Reference

Use these if you prefer GUI tools instead of only terminal commands.

## VS Code
- Open folder: File → Open Folder… (or drag the repo in).
- Branching: bottom-left branch name → `Create new branch`, type name (e.g., `feature/bio`), press Enter.
- Staging/committing: Source Control view → click `+` next to files → type message → Commit.
- Pushing: Source Control view → `Sync`/`Push` button.
- Pull/Fetch: same `Sync`/`Pull` options in Source Control.
- Merge conflicts: open file → use code lens buttons (`Accept Current`, `Accept Incoming`, `Accept Both`). After fixing, save, then `+` to stage and Commit.
- Built-in terminal: View → Terminal. Use when the UI doesn’t offer an action (e.g., `git merge`, `git revert`).

## GitHub Desktop
- Clone/open: File → Clone repository… (or Add local repo).
- Branching: Branch → New Branch… (name it `feature/bio`), Create Branch; switch via top-left branch menu.
- Staging/committing: select changed files → check the boxes to stage → write summary → Commit to <branch>.
- Pushing: blue `Push origin` button (top).
- Pulling: `Fetch origin` / `Pull origin`.
- Merge conflicts: app highlights conflicts → use “Open in editor” or “Open in external editor,” fix markers, return and click “Mark as resolved,” then Commit merge.

Reminder: Keep using the branch names shown in the tasks (e.g., `feature/bio`, `feature/conflict-a`, `feature/conflict-b`) so your PR stays consistent.
