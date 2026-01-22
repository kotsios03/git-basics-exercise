# Task 3 — Create and resolve a merge conflict (solo)

Goal: Experience a simple merge conflict and resolve it.

Setup:
We prepared starter/profile.txt with a line: `Favorite color: TBD`

Steps:

1) Make sure your working tree is clean on `feature/bio` (your PR branch):
   ```
   git checkout feature/bio
   git status
   ```
2) Create and switch to branch `feature/conflict-a`:
   ```
   git checkout -b feature/conflict-a
   ```
3) Edit starter/profile.txt to say: `Favorite color: Blue` and commit:
   ```
   echo "Favorite color: Blue" > starter/profile.txt
   git add starter/profile.txt
   git commit -m "Set favorite color to Blue"
   ```
4) Switch back to `feature/bio`:
   ```
   git checkout feature/bio
   ```
5) Create and switch to branch `feature/conflict-b`:
   ```
   git checkout -b feature/conflict-b
   ```
6) Edit starter/profile.txt to say: `Favorite color: Green` and commit:
   ```
   echo "Favorite color: Green" > starter/profile.txt
   git add starter/profile.txt
   git commit -m "Set favorite color to Green"
   ```
7) Merge `feature/conflict-a` into `feature/conflict-b` (you should see a CONFLICT):
   ```
   git merge feature/conflict-a
   ```
8) Resolve the conflict:
   - Open starter/profile.txt; you will see `<<<<<<<`, `=======`, `>>>>>>>` markers.
   - Replace the whole file content with one line mentioning both colors, e.g.:
     ```
     Favorite color: Blue or Green
     ```
   - VS Code: in the editor, choose “Accept Both Changes” then edit the final line to read `Favorite color: Blue or Green`.
9) Mark the conflict resolved and finish the merge:
   ```
   git add starter/profile.txt
   git status
   git commit -m "Resolve color conflict"
   ```
10) Merge the resolved branch back into your PR branch and push:
   ```
   git checkout feature/bio
   git merge feature/conflict-b
   git push
   ```

Hints:

- Use your editor’s conflict resolution UI if available.
- After resolving, run `git status` to confirm only resolved files remain.
