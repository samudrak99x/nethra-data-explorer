# AI-DLC Gap Analysis And Codex Operating Model

## Purpose

This document maps our current Codex-based delivery plan against AWS AI-DLC ideas so we can manage AI-agent implementation with discipline, traceability, and human oversight.

The goal is not to replace Scrum completely. The goal is to keep the useful structure of Scrum while adding AI-native delivery controls for Codex.


## Current Delivery Context

We are building an agentic, explainable data intelligence product.

Current planning artifacts:
- task-plan.txt
- architecture-plan.txt
- architecture-diagram.svg
- sprint-progress.md
- sprint-backlog.md
- sprint-review-notes.md

Current delivery model:
- Sprint-based planning
- Codex implementation
- GitHub commits and pull requests
- Jira MCP if available
- Markdown sprint tracker fallback
- End-of-sprint demo


## AI-DLC Concepts To Adopt

AWS AI-DLC emphasizes:
- AI as a central collaborator, not just a coding assistant
- AI creates plans and asks clarifying questions
- Humans approve critical decisions
- AI executes with validated context
- Persistent context is stored in the repository
- Workflows adapt to task complexity
- Human oversight is explicit and auditable
- Delivery includes inception, construction, and operations


## Scrum To AI-DLC Mapping

| Traditional Scrum Concept | Codex / AI-DLC Equivalent |
|---|---|
| Product Backlog | Intent backlog |
| Sprint Planning | AI-assisted intent and task planning |
| Sprint | Sprint or short AI-DLC bolt |
| User Story | Unit of work with intent brief |
| Developer task | Agent-executable task |
| Daily Scrum | Progress tracker plus Codex status update |
| Code Review | Human validation gate |
| Sprint Review | Demo of working artifact |
| Retrospective | Agent/process learning log |


## Gap Analysis

| Area | Current State | Gap | Recommended Action |
|---|---|---|---|
| Inception | Product and sprint plans exist | No formal intent brief per unit of work | Add intent brief template |
| Adaptive workflow | Fixed sprint plan exists | Same depth for all tasks | Add complexity-based workflow depth |
| Human approval | PR review planned | Approval gates are not explicit enough | Add plan, architecture, implementation, and demo gates |
| Agent rules | General Codex behavior only | No project-specific steering rules | Add Codex operating rules file |
| Audit trail | Sprint tracker exists | Decisions and assumptions not separately logged | Add AI decision log |
| Behavioral testing | Unit/UI tests planned | Agent answers need eval-style tests | Add agent evaluation plan |
| Security | Not fully defined | Need scanning and review checks | Add secrets, dependency, and PR security checklist |
| Operations | Mostly MVP build plan | Deployment, monitoring, rollback not detailed | Add operations sprint tasks later |
| Cost control | Not defined | LLM/API usage can grow | Add cost and usage review checklist |
| AI Definition of Done | Standard DoD exists | AI-generated work needs extra criteria | Add AI-specific DoD |


## AI-DLC Operating Model For Codex

Use this loop for each sprint or major unit of work:

```text
Intent Brief
   ↓
Codex Plan
   ↓
Human Approval
   ↓
Codex Implementation
   ↓
Tests + Evals
   ↓
Human Review
   ↓
Commit + Pull Request
   ↓
Sprint Demo
   ↓
Retrospective / Learning Log
```


## Intent Brief Template

Each major unit of work should have:

- Title
- Business goal
- User value
- Scope
- Out of scope
- Assumptions
- Constraints
- Acceptance criteria
- Test expectations
- Demo expectation
- Human decisions required
- Risks


## Human Approval Gates

Use these checkpoints:

1. Plan Approval
   - User approves goal, scope, and acceptance criteria.

2. Architecture Approval
   - User approves structure for large or risky changes.

3. Implementation Review
   - User reviews PR, code summary, tests, and limitations.

4. Demo Approval
   - User confirms sprint output is testable and demonstratable.

5. Release Approval
   - User approves deployment or publishing.


## Adaptive Workflow Depth

Not every task needs the same process weight.

### Small Task

Examples:
- typo fix
- small UI copy update
- minor tracker update

Workflow:
- intent
- implement
- verify
- update tracker

### Medium Task

Examples:
- add one component
- add one utility function
- add one testable feature

Workflow:
- intent brief
- short Codex plan
- implement
- test
- review notes
- commit/PR

### Large Task

Examples:
- schema engine
- ontology engine
- pattern discovery engine
- statistical modeling engine
- LLM agent integration

Workflow:
- intent brief
- architecture note
- implementation plan
- user approval
- incremental commits
- tests and evals
- PR review
- demo
- retrospective note


## AI-Specific Definition Of Done

A task is done only when:

- Implementation is complete
- Tests or manual verification are complete
- Agent-generated code has been reviewed
- No invented assumptions remain undocumented
- Any unresolved risks are listed
- Progress tracker is updated
- Review notes are written
- PR is opened or prepared when GitHub is connected
- Demo path is documented


## Agent Evaluation Requirements

For agentic product features, normal tests are not enough.

We also need eval-style checks:
- Does the agent answer only from available data?
- Does the agent cite evidence values?
- Does the agent mention missing data?
- Does the agent distinguish observation from interpretation?
- Does the agent avoid causal claims unless supported?
- Does the agent explain uncertainty for predictions?
- Does the agent explain why the UI was generated?


## Security And Quality Checks

Before PR review:
- Check for secrets
- Check dependency changes
- Check generated code for unsafe file/network behavior
- Check user-uploaded file handling
- Check error handling
- Check accessibility basics for UI work
- Check that tests or manual verification are recorded


## Cost And Usage Checks

Before LLM integration:
- Define what data is sent to the model
- Avoid sending full datasets unnecessarily
- Use summaries and computed facts where possible
- Add fallback rule-based responses
- Track token/API usage during testing
- Add user-visible errors for quota or API failure


## Operations Gap To Address Later

Future operations tasks should include:
- Deployment target
- Environment variables
- Logging
- Error monitoring
- Rollback plan
- Data privacy controls
- Usage monitoring
- Model/API cost monitoring


## New Files To Add For AI-DLC Tracking

Recommended:
- aidlc-gap-analysis.md
- intent-brief-template.md
- ai-decision-log.md
- ai-definition-of-done.md
- agent-eval-plan.md


## Immediate Actions

1. Keep Scrum-style sprint tracking.
2. Add AI-DLC operating controls.
3. Create intent brief template.
4. Create AI decision log.
5. Create AI-specific Definition of Done.
6. Add agent eval plan before LLM integration.
7. Update Sprint -1 to include these setup tasks.
