# 04 — Git & GitHub

## Why it matters

Git records your work; GitHub makes it reviewable, shareable, and ready for CI/CD. Learn this after Linux and before scripting so every later lab has a reliable history.

## What to learn

**Git:** `init`/`clone`, `add`/`commit`, branches, merge, `pull`/`fetch`, `push`, simple merge conflicts, `.gitignore`, and `git revert` basics.

**GitHub:** repositories, Pull Requests, Issues, code-review basics, forks, branch-protection basics, repository secrets, and how GitHub Actions runs workflows from repository changes. Learn the open-source contribution flow: fork → branch → change → test → Pull Request.

## Practical examples

Use a branch and Pull Request for a change instead of editing `main` directly. Put `.env` in `.gitignore`; store CI credentials in repository or environment secrets. Use `git revert` to make a new commit that safely undoes a shared change.

## Short lab (20 minutes)

**Clone → Branch → Change → Commit → Push → Pull Request → Merge.** Clone a repository, create a branch, improve one line in its README, commit and push it, open a Pull Request, review the diff, merge it, and pull the updated default branch locally.

## Common mistakes

Committing secrets, working only on `main`, using `pull` without checking status, deleting unfamiliar code during a conflict, or force-pushing shared branches.

## When to move on

- [ ] I can clone/init, add, commit, branch, merge, fetch, pull, push, and revert a simple change.
- [ ] I can resolve a simple conflict and keep local secrets ignored.
- [ ] I can open a Pull Request, respond to basic review, and explain where GitHub Actions secrets belong.

## Trusted resources

[Pro Git](https://git-scm.com/book/en/v2) · [Git reference](https://git-scm.com/docs) · [GitHub Pull Requests](https://docs.github.com/pull-requests) · [GitHub Actions secrets](https://docs.github.com/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions)
