# Pull Request Draft: Phase A Planning And AI-DLC Baseline

## Title

Establish Nethra Data Explorer planning baseline, AI-DLC workflow, skills, and research foundation


## Summary

This pull request establishes the initial Phase A baseline for **Nethra Data Explorer**.

It does not implement application code yet. Instead, it creates the product, architecture, AI-DLC, sprint-management, research, and skill foundation required before Codex begins implementation.

The delivery model intentionally starts with **Sprint -1 and Sprint 0 running together**:

- **Sprint -1:** Codex, GitHub, repository, and sprint tracking setup
- **Sprint 0:** Conversational AI-DLC transition, intent discovery, skills, and agent-role refinement


## Why This Exists

The user is transitioning from a traditional Scrum background into an AI-DLC / Codex-agent delivery model.

This baseline creates the shared context needed for agentic implementation:

- product intent
- functional and non-functional intents
- architecture direction
- AI-DLC workflow
- sprint tracking
- agent roles
- project-local skills
- research foundation around Our World in Data
- expert-guided knowledge graph direction


## Product Direction Captured

Nethra Data Explorer is defined as a dynamic, explainable data intelligence app.

The product should help users:

- import datasets
- detect schema
- discover ontology
- enrich knowledge graphs with expert knowledge
- generate dynamic dashboards
- discover patterns
- run statistical models
- ask agentic questions
- receive evidence-backed explanations
- generate narrative reports

The first target domain is **poverty tracking**, but the architecture is intended to support other domains later.


## Major Artifacts Added

### Product And Sprint Planning

- `task-plan.txt`
- `doc/sprint-progress.md`
- `doc/sprint-backlog.md`
- `doc/sprint-review-notes.md`

These define the delivery model, sprint sequence, task breakdown, progress tracking, and review checkpoints.


### Architecture

- `architecture-plan.txt`
- `doc/architecture-diagram.svg`

These define the layered architecture:

- Data Layer
- Schema and Metadata Layer
- Ontology and Explainability Layer
- Expert Knowledge Graph Layer
- Dynamic Application Layer
- Visualization Layer
- Analysis Layer
- Pattern Discovery Layer
- Statistical Modeling Layer
- Agent Layer
- Report Layer
- Persistence Layer
- Integration Layer
- Delivery and Project Management Layer


### AI-DLC Operating Model

- `doc/aidlc-gap-analysis.md`
- `doc/ai-decision-log.md`
- `doc/ai-definition-of-done.md`
- `doc/agent-eval-plan.md`
- `doc/scrum-to-aidlc-transition-map.md`
- `doc/conversational-discovery-log.md`

These documents map Scrum concepts into AI-DLC/Codex-agent concepts and define how the team should manage human approval, agent work packages, evals, traceability, and AI-generated implementation.


### Intent Documents

- `doc/intent-identification-workflow.md`
- `intent-brief-template.md`
- `doc/functional-intents.md`
- `doc/non-functional-intents.md`
- `doc/product-intent-knowledge-base.md`
- `doc/assumptions-and-risks.md`
- `doc/acceptance-criteria-catalog.md`

These documents define the business/product intent, functional scope, quality expectations, assumptions, risks, and reusable acceptance criteria.


### Agent Roles

- `doc/agent-role-definitions.md`

Initial agent roles include:

- Product Owner Agent
- Business Analyst Agent
- Solution Architect Agent
- Data Analyst Agent
- Expert Knowledge Curator Agent
- QA and Evaluation Agent
- Delivery Orchestrator Agent


### Project-Local Skills

#### `skills/product-ba-po-intent`

Guides Codex to preserve BA/PO context, product intent, functional and non-functional requirements, acceptance criteria, risks, and assumptions.

#### `skills/owid-agentic-researcher`

Supports research around Our World in Data, OWID Grapher, OWID APIs, comparable products, and hypothetical agentic versions of OWID-like functionality.

Includes:

- `references/owid-research-brief.md`
- `research/initial-owid-agentic-product-research.md`

#### `skills/expert-knowledge-graph`

Guides future work around expert-guided ontology and knowledge graph enrichment.

Focuses on:

- expert conversations
- uploaded documents/photos/videos
- claim extraction
- evidence artifacts
- provenance
- validation
- agent use of expert knowledge


## Key Product Decisions Captured

### Dataset-Driven, Not Page-Driven

The product should not create one hardcoded page per dataset.

Instead:

```text
dataset + schema + metadata + ontology + expert knowledge
  -> generated UI
  -> generated analysis
  -> generated explanations
  -> generated reports
```


### Explainability Is Core

The system must explain:

- how it interpreted data
- why UI controls were generated
- why patterns were detected
- why statistical methods were recommended
- which evidence supports an answer
- where expert knowledge came from


### Expert Knowledge Graph Enrichment

After automatic ontology discovery, the system should support local/domain expert knowledge.

Experts can contribute through:

- conversations
- uploaded documents
- uploaded photos
- uploaded videos
- notes
- URLs
- dataset annotations

Expert claims must include:

- provenance
- evidence
- validation status
- confidence

The agent must distinguish:

```text
dataset-derived fact
vs
expert-provided knowledge
vs
unverified claim
```


### OWID Is Inspiration, Not A Clone

Our World in Data is treated as inspiration for:

- trusted public data storytelling
- source transparency
- data and metadata reuse
- interactive charts
- chart data APIs

Nethra goes beyond OWID by supporting:

- user-imported datasets
- dynamic schema and ontology discovery
- agentic analysis
- expert knowledge enrichment
- statistical testing
- forecasting
- explainable AI answers


## Delivery Model

### Phase A: Setup And Intent

Runs together:

- Sprint -1
- Sprint 0

Exit criteria:

- Codex project root is ready
- GitHub repository is selected and remote is linked
- sprint tracking exists
- AI-DLC context exists
- product intent docs exist
- initial skills exist
- initial agent roles exist


### Phase B: First Implementation

Runs together after Phase A:

- Sprint 0.5
- Sprint 1

Goal:

- create app shell
- add poverty mock data
- implement CSV/JSON import
- preview rows
- infer schema


### Phase C: Product Capability Sprints

Includes:

- Dynamic UI Generation
- Ontology Discovery
- Expert Knowledge Graph Enrichment
- Charts and Data Views
- Pattern Discovery
- Explainable AI Pattern Cards
- Statistical Modeling and Prediction
- Agentic Explanation
- LLM Integration
- Report Builder
- Dataset Library
- Polish and Demo Package


## Verification Performed

- Local project folder created at:
  - `/Users/samudrakanankearachchi/Documents/Codex/workdir/nethra-data-explorer`
- Local Git repository initialized.
- Branch created:
  - `phase-a/sprint-0-planning-baseline`
- GitHub remote linked:
  - `https://github.com/samudrak99x/nethra-data-explorer.git`
- GitHub plugin access confirmed for:
  - `samudrak99x`
  - `Agentri-ai`
- Jira MCP checked and not available in this session.
- Markdown tracking selected as active fallback.


## Current Limitations / Blockers

- GitHub plugin repository list does not yet show `samudrak99x/nethra-data-explorer`.
- Pull request creation is not exposed by the currently available GitHub connector tools.
- Remote push may require GitHub app access refresh or local Git credentials.
- No application code has been implemented yet.
- Jira integration is deferred until Jira MCP/tools are available.


## Review Focus

Please review:

- whether the AI-DLC transition model makes sense
- whether Sprint -1 and Sprint 0 should remain paired
- whether the product intents are accurate
- whether expert knowledge graph enrichment is correctly positioned
- whether OWID research direction is useful
- whether the proposed skills and agent roles are the right starting set


## Suggested Next Step After This PR

Start **Phase B**:

```text
Sprint 0.5 + Sprint 1
```

This will create the first working app baseline:

- React/TypeScript project
- app shell
- mock poverty dataset
- CSV/JSON import
- data preview
- schema inference
- user correction of schema roles

