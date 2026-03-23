# Project: neiwen.github.io

## Git Workflow

- Main branch: `master`
- Remote: `origin` (git@github.com:Neawhen/neiwen.github.io.git)

## Agent Workflow for Code Changes

When making code changes (new features, bug fixes, refactoring, content updates):

1. **Always create a new branch** from `master` with a descriptive name (e.g., `feat/add-about-page`, `fix/nav-links`, `content/update-services`)
2. **Commit changes** to the new branch with clear commit messages
3. **Push the branch** to `origin`
4. **Create a Pull Request** via `gh pr create` targeting `master`, with a clear title and description
5. **Return the PR URL** to the user for review

Branch naming conventions:
- `feat/` — new features
- `fix/` — bug fixes
- `content/` — content updates
- `refactor/` — code refactoring
- `style/` — styling changes

## Permissions Note

- The agent is allowed to create branches, push to origin, and create PRs
- The agent should NOT merge PRs — leave that for the user to review and merge
- The agent should NOT force-push or delete branches
