# Scrum To AI-DLC Transition Map

## Purpose

This document helps transition from a traditional Scrum delivery mindset to an AI-DLC / Codex-agent delivery mindset.

Sprint 0 is intentionally conversational and flexible. The goal is to learn the new operating model, reshape terminology, and create the right skills, agent roles, and context artifacts before implementation starts.

The longer-term goal is to stop thinking in Scrum-first terms altogether and move to an AI-DLC-native planning cycle.


## Terminology Map

| Scrum Term | AI-DLC / Codex-Agent Equivalent | Notes |
|---|---|---|
| Product Backlog | Intent Backlog | Backlog items describe intended outcomes, constraints, and acceptance signals. |
| Sprint Planning | Intent Framing Session | Clarifies business intent, user intent, risks, and agent-executable tasks. |
| User Story | Intent Brief | Captures goal, scope, assumptions, acceptance criteria, and demo expectation. |
| Task | Agent Work Package | A bounded unit Codex can plan, implement, verify, and report on. |
| Definition of Done | AI Definition of Done | Adds evidence, traceability, tests/evals, and human review. |
| Daily Scrum | Progress Sync | Uses tracker updates, Codex status, blockers, and decisions. |
| Developer | Human + AI Agent Team | Codex implements, user steers and approves. |
| Scrum Master | Delivery Orchestrator | Keeps workflow healthy, blockers visible, and AI-DLC controls followed. |
| Product Owner | Intent Owner | Owns product direction, priorities, acceptance, and tradeoffs. |
| Business Analyst | Intent Analyst | Helps discover functional/non-functional intent and acceptance criteria. |
| Code Review | Human Validation Gate | Reviews implementation, assumptions, tests, and risks. |
| Sprint Review | Demonstration Checkpoint | Shows working artifact and validates outcome. |
| Retrospective | Learning Log | Captures what to improve in prompts, skills, agents, and delivery flow. |


## Mindset Shift

Traditional Scrum often assumes humans decompose and assign work to humans.

AI-DLC assumes humans and AI agents co-create the delivery path:
- humans provide intent, judgment, and approval
- agents explore, plan, implement, test, and explain
- persistent context helps agents stay aligned
- work can be reorganized as understanding improves

### What Changes In Practice

- Backlog items become intents, not just stories.
- Planning becomes elaboration, not just estimation.
- Tasks become bolts that agents can execute and test.
- Validation becomes a formal steering point, not a late-stage sign-off.
- Progress tracking follows the agent loop, not only the human ceremony calendar.


## Sprint 0 Transition Goals

- Understand AI-DLC terminology.
- Decide which Scrum concepts remain useful.
- Convert backlog items into intent briefs.
- Create reusable product context.
- Create or draft BA/PO/QA/Architect-style skills or agent roles.
- Define human approval gates.
- Define how Codex reports progress.
- Decide what is tracked in Jira versus markdown.


## AI-DLC Native Planning Cycle

Use this as the default cycle for Nethra once the transition is complete:

1. Intent capture
2. Mob elaboration
3. Architectural shaping
4. Bolt decomposition
5. Agent execution
6. Agent testing
7. Human validation at steering points
8. Commit / PR / review
9. Learning log update


## Planning Vocabulary To Prefer

- Intent instead of user story
- Elaboration instead of refinement
- Bolt instead of task
- Steering point instead of ceremony gate
- Agent loop instead of developer workflow
- Learning log instead of retrospective notes
- Validation gate instead of final review only


## Recommended Sprint 0 Conversations

1. Product intent conversation
2. Functional intent conversation
3. Non-functional intent conversation
4. Architecture intent conversation
5. Delivery workflow conversation
6. Agent role conversation
7. Skill creation conversation
8. Acceptance criteria conversation
9. Review and approval conversation


## Output Of Sprint 0

Sprint 0 does not need code.

Sprint 0 should produce:
- intent documents
- AI-DLC terminology map
- agent role definitions
- skill drafts
- acceptance criteria
- risk and assumption notes
- delivery workflow
- progress tracker
- enough clarity to start implementation

## Output Of The Transition

When the transition is complete, the planning system should feel AI-DLC-native:

- work starts from intent
- the team elaborates the shape of the work before execution
- Codex and other agents receive bolts, not vague tasks
- humans step in at well-defined steering points
- delivery artifacts record decisions, assumptions, and validation
- the planning cycle supports continuous refinement instead of fixed Scrum ceremony dependence
