# Repo Flow Manager Test Report

Date: 2026-05-01

## Scope

Tested the skill instructions for the combined repo workflow:

- local git for branch and commit work
- GitHub plugin for PR and review flow
- GitHub MCP for hosted GitHub gaps

## What was checked

### 1. Workflow ordering
Verified that the skill now presents a clear order:

1. Check repo state
2. Create branch
3. Make changes
4. Stage and commit
5. Push branch
6. Open or update PR
7. Review and CI
8. Resolve conflicts
9. Merge
10. Confirm main

Result: Pass

### 2. Tool assignment
Verified that the skill assigns the tools by role rather than forcing one tool for everything:

- local git for branch creation and commits
- GitHub plugin for PR operations and merge flow
- GitHub MCP for gaps in hosted GitHub coverage

Result: Pass

### 3. Conflict handling guidance
Verified that the skill includes a conflict workflow:

- compare with main
- identify conflicting files
- restore or adjust overlap
- recheck mergeability

Result: Pass

### 4. PR workflow clarity
Verified that the reference file documents the pull request lifecycle in a usable order.

Result: Pass

## Limitations observed

- The skill is descriptive, not executable by itself.
- Local git write access can still be blocked by the sandbox in some Codex sessions.
- GitHub plugin and MCP capabilities can vary by session, so the skill correctly treats them as selectable paths rather than hard requirements.

## Conclusion

The skill is ready for use as a repo-flow guide.
It clearly separates the responsibilities of local git, GitHub plugin, and GitHub MCP, which makes the end-to-end pull request cycle easier to run in practice.
