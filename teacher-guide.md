# Teacher Guide

Suggested flow (35–45 min):

1) 5 min — Explain Git (snapshots), GitHub (remote), and the goals
2) 10–15 min — Students do Tasks 1–2 (commits, branch, PR)
3) 10–15 min — Students do Task 3 (conflict) and Task 4 (history/revert)
4) 5–10 min — Debrief: good commit messages, when to branch, how to resolve conflicts

Rubric (10 points):

- (2) Commits: 3+ commits, clear messages
- (2) Branching: created `feature/...`
- (2) PR: opened and described changes
- (2) Conflict: resolved correctly and pushed
- (2) History/Revert: demonstrated `git log` and a `revert` commit

Tips:

- If students share computers, let them fork individually but pair on the same machine.
- Encourage small, meaningful commits.
- If conflict feels hard, demo once on projector first.
- Collect from students (see CHECKLIST.md):
  - PR URL to their fork
  - Branch name (should be `feature/bio`)
  - Last 5 commits (`git log --oneline --max-count 5`)
  - Confirmation they pushed after the revert
