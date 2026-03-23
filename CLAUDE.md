# Project: neiwen.github.io

## Git Workflow

- Main branch: `master`
- Remote: `origin` (git@github.com:Neawhen/neiwen.github.io.git)

## Agent Workflow for Code Changes

When making code changes (new features, bug fixes, refactoring, content updates):

1. **Always create a new branch** from `master` with a descriptive name (e.g., `feat/add-about-page`, `fix/nav-links`, `content/update-services`)
2. **Collect ALL changes** before creating the PR — do not create the PR until all related changes are committed. If the user requests additional changes during the conversation, commit them to the same branch before creating the PR.
3. **Commit changes** to the new branch with clear commit messages
4. **Push the branch** to `origin`
5. **Create a Pull Request** via `gh pr create` targeting `master`, with a clear title and description
6. **Return the PR URL** to the user for review
7. If the user requests more changes after the PR is created but before merge, commit and push to the same branch — do NOT create a separate PR for related changes.

Branch naming conventions:
- `feat/` — new features
- `fix/` — bug fixes
- `content/` — content updates
- `refactor/` — code refactoring
- `style/` — styling changes

## Important Rules

- **Do not create PR prematurely** — wait until all related changes in the conversation are ready
- **One topic = one PR** — group related changes (e.g., about + publications + services + news from the same CV update) into a single PR
- Before creating a branch, always `git checkout master && git pull` to start from latest
- After a PR is merged, always `git checkout master && git pull` before starting new work

## Jekyll Site Structure

- `_pages/about.md` — homepage / bio
- `_pages/services.md` — academic services
- `_pages/publications.md` — publications page (years list must include all publication years)
- `_bibliography/papers.bib` — publication entries (BibTeX format)
- `_news/announcement_*.md` — news items (numbered sequentially)

## Permissions Note

- The agent is allowed to create branches, push to origin, and create PRs
- The agent should NOT merge PRs — leave that for the user to review and merge
- The agent should NOT force-push or delete branches
