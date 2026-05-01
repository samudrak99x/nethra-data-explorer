---
name: repo-flow-manager
description: Manage the end-to-end repository workflow for Codex using local git for branch creation and commits, the GitHub plugin for pull request and review work, and GitHub MCP for hosted GitHub gaps such as missing file or repo operations. Use when the user wants PR flow, branch flow, merge flow, or a single skill to coordinate repo actions.
---

# Repo Flow Manager

Use this skill when the user wants the repository workflow handled end to end.

## Tool choice

Use the simplest working path in this order:

1. Local `git` for branch creation, staging, committing, and pushing when the sandbox allows it.
2. GitHub plugin for pull requests, reviews, comments, status checks, and merge operations.
3. GitHub MCP for hosted GitHub actions that are better exposed there or when plugin coverage is missing.

## Operating rule

Do not force one tool for every step.
Pick the tool that is actually available for the step at hand.

## Core flow

```text
Check repo state
  -> Create branch
  -> Make changes
  -> Stage / commit
  -> Push branch
  -> Open or update PR
  -> Review / CI / comments
  -> Resolve conflicts if needed
  -> Merge
  -> Confirm main
```

## What to use each tool for

### Local git
- branch creation
- staging and committing
- pushing changes

### GitHub plugin
- fetch files and PRs
- compare branches
- inspect review comments and CI
- create or update text files and commits when needed
- merge pull requests

### GitHub MCP
- hosted GitHub access
- repo-aware AI operations
- PR / issue / branch actions that the plugin surface does not expose cleanly

## Pull request workflow

1. Create or choose a feature branch.
2. Make the change set small and reviewable.
3. Commit the work locally.
4. Push the branch.
5. Open or update the pull request.
6. Review diff, comments, and CI.
7. Resolve conflicts or failing checks.
8. Merge when the PR is clean.
9. Confirm `main` received the change.

## Conflict workflow

When a branch diverges:

1. Compare branch to `main`.
2. Identify the files that actually conflict.
3. Restore or adjust the overlapping files.
4. Rebase or rebuild the branch content.
5. Recheck mergeability.
6. Merge only when GitHub accepts it.

## Rules

- Prefer text-first GitHub plugin operations for PR work.
- Use MCP when the GitHub plugin surface is missing the needed action.
- Use local git for branch and commit mechanics whenever possible.
- Keep the workflow visible to the user with the current branch, PR number, and merge status.

## When to read the reference

Read [references/pull-request-workflow.md](references/pull-request-workflow.md) when you need the exact PR lifecycle, tool mapping, or merge checklist.
