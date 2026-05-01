# Pull Request Workflow

## Preferred division of labor

- Local git: branch creation, staging, committing, pushing
- GitHub plugin: PR inspection, comments, reviews, CI, merge
- GitHub MCP: hosted GitHub operations that are missing or awkward in the plugin surface

## End-to-end flow

1. Check repo state.
2. Create a branch.
3. Make the change.
4. Commit locally.
5. Push the branch.
6. Open or update the pull request.
7. Inspect comments, diff, and CI.
8. Resolve conflicts if the branch no longer merges cleanly.
9. Merge the pull request.
10. Confirm the target branch updated.

## Good PR shape

- Clear title
- Short summary of what changed
- Acceptance criteria
- Tests or verification
- Known limitations
- Review focus

## Conflict handling

- Compare the branch with `main`.
- Keep the branch content aligned with the target branch where possible.
- Restore root files if an archive move caused delete-vs-modify friction.
- Recheck mergeability before merging.

## Tool selection rule

Use the first tool that can complete the step cleanly.
Do not add extra tool hops unless they are needed to fill a gap.
