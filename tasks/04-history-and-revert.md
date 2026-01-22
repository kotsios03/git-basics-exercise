# Task 4 — History and revert

Goal: Inspect commit history and undo one change safely.

Steps:

1) Be on your PR branch and view a compact history graph:
   ```
   git checkout feature/bio
   git log --oneline --graph --decorate --all
   ```
2) Pick a previous commit you can safely revert (e.g., your change to hello.txt), copy its hash (first 7+ characters).
3) Create a revert commit (this adds a new commit that undoes the old one):
   ```
   git revert <hash>
   ```
   (VS Code: use Source Control “…” menu → Undo Last Commit won’t create a revert; prefer the command so your PR shows the revert commit.)
4) Push your branch and confirm the new revert commit appears in your PR:
   ```
   git push
   ```

Hints:

- Revert creates a new commit that undoes the chosen commit — it does not delete history.
- If revert opens an editor, write a short message and save/close.
- Avoid reverting a merge commit for this exercise.
