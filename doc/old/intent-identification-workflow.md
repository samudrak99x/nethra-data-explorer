# Intent Identification Workflow

## Purpose

This workflow captures product intent before Codex starts implementation. It acts as the AI-DLC inception layer for the project.

The goal is to make sure Codex understands not only the tasks, but also the business intent, user value, constraints, quality attributes, and acceptance criteria.


## Workflow

```text
Business Intent
   -> User Goals
   -> Functional Intents
   -> Non-Functional Intents
   -> Assumptions And Risks
   -> Acceptance Criteria
   -> Human Approval
   -> Codex Implementation Context
```


## Step 1: Identify Business Intent

Questions:
- What problem are we solving?
- Who is the user?
- What decision should the product help the user make?
- Why does this product need to be agentic?
- Why does it need explainability?

Current answer:
The product helps users import datasets, understand their meaning, discover patterns, run statistical analysis, ask natural-language questions, and generate explainable reports.


## Step 2: Identify Functional Intent

Functional intent describes what the system must do.

Examples:
- The system must import CSV/JSON datasets.
- The system must infer schema.
- The system must discover ontology.
- The system must generate dynamic dashboards.
- The system must explain patterns with evidence.

Detailed functional intents are tracked in functional-intents.md.


## Step 3: Identify Non-Functional Intent

Non-functional intent describes how the system must behave.

Examples:
- Explanations must be evidence-backed.
- Agent answers must not invent data.
- UI generation should be explainable.
- Forecasts must show uncertainty and caveats.
- The system must be testable sprint by sprint.

Detailed non-functional intents are tracked in non-functional-intents.md.


## Step 4: Identify Assumptions

Initial assumptions:
- MVP starts with local CSV/JSON files.
- Poverty tracking is the first domain.
- Local browser storage is acceptable for MVP.
- Rule-based agent comes before LLM integration.
- Jira may not be available, so markdown tracking must remain supported.


## Step 5: Identify Risks

Initial risks:
- Dataset schema detection may be wrong.
- Ontology tagging may be wrong.
- Agent may overstate statistical findings.
- Forecasts may be misunderstood as facts.
- Generic UI generation may become confusing.
- LLM usage may become expensive if full datasets are sent.


## Step 6: Define Acceptance Criteria

Acceptance criteria must be testable and demonstratable.

Each sprint should answer:
- What can the user see?
- What can the user do?
- What can be tested?
- What changed from the previous sprint?
- What remains limited or risky?


## Step 7: Human Approval

Before implementation starts, the user should approve:
- product intent
- functional scope
- non-functional expectations
- first implementation sprint
- delivery workflow


## Step 8: Convert Intent Into Codex Context

Codex should use these files during implementation:
- task-plan.txt
- architecture-plan.txt
- aidlc-gap-analysis.md
- functional-intents.md
- non-functional-intents.md
- product-intent-knowledge-base.md

The project-local skill draft is in:
- skills/product-ba-po-intent/SKILL.md
