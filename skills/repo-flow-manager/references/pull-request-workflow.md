# Pull Request Workflow

## Purpose

This workflow keeps repository changes visible, reviewable, and easy to merge.

## Flow

1. Start from a clean understanding of the current repo state
2. Create or choose a focused branch
3. Make the smallest useful set of changes
4. Review the diff before pushing
5. Push the branch to GitHub
6. Open the pull request
7. Check status, comments, and CI
8. Address review feedback
9. Merge when approved
10. Confirm the merge reached `main`

## Decision points

- Use git when the task is purely local branch/commit work
- Use GitHub MCP when you need GitHub-side intelligence or server-backed actions
- Use the GitHub plugin when it exposes the exact action needed

## PR checklist

- Branch name is clear
- Commit message describes the outcome
- PR title matches the work
- PR body explains intent and scope
- Any blockers are named
- Any local-only assets are called out

## Merge discipline

- Merge only after review or explicit approval
- Prefer a single merge path for each branch
- Confirm `main` reflects the intended change

