# Task 2 — Branch and Pull Request

Goal: Create a feature branch, add a new file, push, and open a PR.

Steps:

1) Create a new branch named `feature/bio`.
   ```
   git checkout -b feature/bio
   git branch --show-current
   ```
2) Create a file `bio.md` with:
   - Your name as a heading
   - 3 bullet points about you
   Example:
   ```
   echo "# Your Name
- I like ...
- I want to learn ...
- My favorite food is ..." > bio.md
   ```
   (VS Code: create a new file, type the content, save.)
3) Commit with a clear message:
   ```
   git status
   git add bio.md
   git commit -m "Add bio with three facts"
   ```
   (VS Code: open the Source Control panel, click + to stage bio.md, type the commit message, click Commit.)
4) Push your branch to your GitHub fork (sets the upstream the first time):
   ```
   git push -u origin feature/bio
   ```
   (VS Code: click the Sync/Push button in Source Control.)
5) On GitHub, open a Pull Request from `feature/bio` into `main` of YOUR fork. Use a short description like “Adds my bio file.”
6) Keep this same branch and PR for all remaining tasks. You will push more commits to `feature/bio`.

Hints:

- Use `git branch --show-current` to confirm you’re on the new branch.
- Use `git push -u origin feature/bio` the first time.
