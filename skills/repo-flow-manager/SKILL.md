---
name: repo-flow-manager
description: Manage the full repository workflow across local git, GitHub MCP, and GitHub plugin. Use when the user wants branches, commits, pushes, pull requests, PR review, merge coordination, or a documented PR workflow, regardless of which GitHub tool path is available.
---

# Repo Flow Manager

Use this skill to manage the end-to-end repository flow.

## Goal

Keep one consistent workflow across:
- local git commands
- GitHub MCP
- GitHub plugin

Choose the most reliable available path for the current task.

## Tool selection

Prefer this order:
1. Local git for branch, commit, fetch, merge, and push
2. GitHub MCP for repo-aware inspection, PR/issue/CI intelligence, and GitHub-hosted automation
3. GitHub plugin when it exposes the exact action needed or MCP is missing that capability

If a path is blocked, switch to the next available path rather than stopping.

## Workflow

1. Check current branch and repo state
2. Identify uncommitted changes
3. Group changes into a focused branch
4. Commit locally
5. Push the branch
6. Create or update the pull request
7. Review status, comments, and checks
8. Merge when approved
9. Record the outcome in the repo docs if needed

## Branching rules

- Use one branch per coherent work package
- Keep the branch name short and descriptive
- Prefer `phase-a/...` for ongoing planning work

## Pull request rules

- Keep PRs focused
- Include a short summary of what changed
- Note whether the change is docs, skills, visuals, or workflow
- Call out anything intentionally left local or pending

## PR workflow reference

Read [pull-request-workflow.md](references/pull-request-workflow.md) when you need the exact PR sequence, checklist, or merge discipline.

## Output style

When using this skill, always report:
- current branch
- files changed
- tool path used
- PR state
- merge status


## Visual reference

- [Repo Flow Manager Diagram](assets/repo-flow-manager.png)
