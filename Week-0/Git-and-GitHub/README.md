# Git and GitHub

Create a **new GitHub repository under your own account** and complete the tasks there.

## Resources

- [Git and GitHub video](https://www.youtube.com/watch?v=apGV9Kg7ics)
- [Git Cheat Sheet — Education edition](git-cheat-sheet-education.pdf)
- [GitHub Flow — official guide](https://docs.github.com/en/get-started/using-github/github-flow)

## Assignment

Create and use your own GitHub repository. Complete every step yourself.

Create a folder named `Github` in your repository, then do these steps in order:

1. Clone the repository and create a `dev` branch.
2. On `dev`, create `notes.md` with one sentence. Commit and push it.
3. Create `feature/add-notes` from `dev`. Add a second sentence to `notes.md`, commit, and push.
4. Switch back to `dev`. Create `todo.md` with `- First task`, then commit and push it.
5. Switch to `feature/add-notes` and merge `dev` into it. Push the branch, open a PR into `dev`, then merge the PR.
6. Create `feature/rebase-practice` from `dev`. Add `- Feature task` below the first line in `todo.md` and commit. Switch to `dev`, add `- Dev task` above the first line, and commit. Switch back and rebase your feature branch onto `dev`.
7. Push the rebased branch and open a second PR into `dev`. Review and merge it.
8. **Merge conflict practice:** From `dev`, create `conflict/one` and `conflict/two`. Edit the same line in a file differently on each branch and commit. Merge `conflict/one` into `dev`, then merge `dev` into `conflict/two`. Resolve the conflict, commit, and merge `conflict/two` into `dev`.

