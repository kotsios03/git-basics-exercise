# Git Basics: Mini Exercise (30–45 min)

A hands-on exercise to learn core Git and GitHub workflows: commits, branches, merge conflicts, and pull requests.

Audience: High school students, first-time Git users.

## Setup

If you don't have Git or a GitHub account yet, follow the setup instructions in [SETUP.md](SETUP.md) first.

## Prerequisites

- Git installed
- GitHub account

## Tools you can use

- All steps show terminal commands; you can also use VS Code or GitHub Desktop.
- VS Code: open the folder, use the Source Control view to stage/commit/push, and the branch picker (bottom left) to create/switch branches. Use the built-in terminal for commands that are faster to type (merges, reverting).
- GitHub Desktop: any action shown with a command can be done through the menus/buttons; keep the same branch names.
- Quick reference: see [tools-quick-reference.md](tools-quick-reference.md) for screenshots-free step lists.

## What students will practice

- Making meaningful commits with messages
- Creating and switching branches
- Pushing to GitHub and opening a Pull Request (PR)
- Resolving a simple merge conflict
- Viewing history and undoing with `revert`

## Quick start

0) If needed, complete [SETUP.md](SETUP.md).
1) Fork this repo on GitHub.
2) Clone your fork to your computer.
3) Complete the tasks in order (each file has copy-pasteable commands):
   - tasks/01-commit.md
   - tasks/02-branch-and-pr.md
   - tasks/03-merge-conflict.md
   - tasks/04-history-and-revert.md
4) Use ONE branch and ONE PR for everything:
   - Your main branch for this exercise is `feature/bio` (created in Task 2).
   - For Task 3 you will make temporary conflict branches, then merge back into `feature/bio`.
   - Keep pushing `feature/bio` so the same PR shows all your work.
5) Open a PR from `feature/bio` into `main` on your fork.
6) Submit the PR URL to your teacher.

## Repo structure

- starter/ — small starter files you will edit
- tasks/ — step-by-step instructions
- CHECKLIST.md — self-check of what you completed

## Submission

- Share the URL of your Pull Request.
- Make sure your PR shows your commits and a resolved conflict.

## Teacher notes

See teacher-guide.md for a rubric and suggested walkthrough.
