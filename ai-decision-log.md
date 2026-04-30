# AI Decision Log

This file records important AI-DLC decisions, assumptions, approvals, and delivery choices made while Codex helps implement the product.

## Decision Statuses

- Proposed
- Accepted
- Rejected
- Superseded


## Decisions

### 2026-04-30: Use Markdown Sprint Tracking Until Jira MCP Is Available

Status: Accepted

Context:
The user wants Jira integration if available, but is also comfortable using text or markdown files for sprint tracking.

Decision:
Use markdown tracker files as the active tracking system until Jira MCP is connected.

Rationale:
Jira tools are not currently exposed in this Codex session, while markdown files are already available and reviewable in the workspace.

Implications:
- sprint-progress.md is the active sprint status file.
- sprint-backlog.md is the active backlog file.
- sprint-review-notes.md is the active review file.
- Jira can be added later without blocking implementation.


### 2026-04-30: Run Sprint -1 And Sprint 0 Together

Status: Accepted

Context:
The user is transitioning from traditional Scrum to AI-DLC and also needs implementation infrastructure.

Decision:
Run Sprint -1 and Sprint 0 together as Phase A.

Rationale:
Sprint -1 creates the workspace, repository, tracking, and review workflow. Sprint 0 creates the product intent, AI-DLC terminology, skills, agent roles, and acceptance model.

Implications:
Implementation should not start seriously until enough infrastructure and intent context exist.


### 2026-04-30: Keep Sprint 0 Conversational And Flexible

Status: Accepted

Context:
The user wants Sprint 0 to support learning, restructuring, skill creation, and progressive refinement.

Decision:
Sprint 0 is not a rigid requirements phase. It is a conversational AI-DLC transition and intent discovery sprint.

Rationale:
AI-DLC benefits from evolving context, agent roles, and skills as product intent becomes clearer.

Implications:
Sprint 0 documents and skills can change throughout the sprint.


### 2026-04-30: Local Git Initialized, GitHub Commit/PR Workflow Blocked

Status: Accepted

Context:
Sprint -1 requires repository setup, commit workflow, and PR workflow.

Decision:
Initialize local Git in the current Codex workspace and use the main branch. Defer commits and GitHub PR workflow until Git identity and GitHub authentication are available.

Rationale:
The workspace was not a Git repository. GitHub CLI is not available in this session, and Git user.name/user.email are not configured.

Implications:
- Project files are now inside a local Git repository.
- Commits require Git identity configuration.
- Remote PR automation requires GitHub authentication or GitHub MCP/app setup.
- Markdown tracker remains the active progress system.


### 2026-04-30: GitHub Plugin Access Confirmed

Status: Accepted

Context:
The user installed the GitHub plugin for Codex.

Decision:
Use the GitHub connector for repository inspection and GitHub-side operations where supported.

Rationale:
The connector can access repositories for `samudrak99x` and `Agentri-ai`.

Implications:
- GitHub authentication is unblocked through the connector.
- We still need to choose the target repository for this product.
- Local Git commits still need local Git identity configuration.
- Direct local push/PR automation may still depend on available connector operations or user-provided repository setup.


### 2026-04-30: Rename Product Project To Nethra Data Explorer

Status: Accepted

Context:
The user asked to create a new project for the product named `nethra-data-explorer`.

Decision:
Rename the local project folder to `nethra-data-explorer` and update planning documents to use the product name Nethra Data Explorer.

Rationale:
The new name is more meaningful for the product and should be reflected in local project structure and planning documents.

Implications:
- The local repository path is now `workdir/nethra-data-explorer`.
- The product working name is now Nethra Data Explorer.
- A matching GitHub repository still needs to be created or selected.


### 2026-04-30: Prepare Nethra Data Explorer As Codex Project Root

Status: Accepted

Context:
The user asked to associate the project with Codex.

Decision:
Treat `workdir/nethra-data-explorer` as the Codex project root for this product.

Rationale:
The folder contains the local Git repository, planning documents, sprint trackers, AI-DLC controls, and project-local skills.

Implications:
- Future Codex work should run from `workdir/nethra-data-explorer`.
- CLI usage can target this folder with `codex --cd workdir/nethra-data-explorer`.
- If the Codex desktop app requires explicit project selection, the user should open/select this folder as the project root.


### 2026-04-30: Link Local Repository To GitHub Remote

Status: Accepted

Context:
The user provided the target repository name `samudrak99x/nethra-data-explorer`.

Decision:
Set local Git remote `origin` to `https://github.com/samudrak99x/nethra-data-explorer.git`.

Rationale:
This aligns the local Codex project repository with the intended GitHub repository.

Implications:
- The local repository is now linked to the intended GitHub remote.
- The GitHub plugin repository list does not yet show this repo, so app installation/access may need to refresh.
- Commits and push still require local Git identity and remote repository availability.


### 2026-04-30: Create Phase A Planning Baseline Branch And Commit

Status: Accepted

Context:
The user requested a branch and pull request with comprehensive notes for the planning baseline.

Decision:
Create local branch `phase-a/sprint-0-planning-baseline`, add a comprehensive pull request draft, and commit the Phase A planning baseline locally.

Rationale:
The branch and commit provide a reviewable baseline for Sprint -1 and Sprint 0 work even though remote push and PR creation are currently blocked by GitHub credential/tooling limitations.

Implications:
- Local commit `156f1c6` contains the Phase A baseline.
- `PR_DRAFT_PHASE_A.md` contains the comprehensive PR description.
- Push is blocked by missing local HTTPS Git credentials.
- Pull request creation is pending until the branch can be pushed or a connector PR creation tool is available.
