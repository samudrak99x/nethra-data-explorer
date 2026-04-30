# Nethra Data Explorer — AI-DLC Operating Plan (AI-DLC Version)

This AI-DLC formatted document converts the original `task-plan.txt` into explicit AI-DLC artifacts: Intents, Stages, Bolts, Units, Agents, Validation gates, and Learning records. Nothing from the original plan is omitted; items are reorganized so each stage, bolt, unit, task and test is represented as an AI-DLC entity.

High-level mapping used in this conversion
- Intent: product- or domain-level goal (mapped from Intent Board, Intent Layer)
- Stage: an MVP phase or release slice
- Bolt: the smallest useful execution unit inside a stage
- Unit: a task inside a bolt, produced during bolt elaboration
- Agent Role: actor responsible for bolt/unit
- Validation: test or acceptance criteria
- Learning: logs, decision records, and audit artifacts

Intent Board
------------
Primary Intent (AI-DLC Intent)
- id: intent.primary.dataset-agentic
- title: Make imported datasets explainable, dynamic, and expert-enriched data products
- description: users import a dataset; the system understands schema, ontology, and semantics; it generates the interface and analysis surfaces; explains patterns with evidence; supports expert enrichment and cloud deployment.

Domain Intent (AI-DLC Intent)
- id: intent.domain.poverty-first
- title: Start with poverty tracking
- description: target poverty tracking initially; keep architecture flexible for health, education, climate, economy, and other domains without one custom page per dataset.

Implementation Constraints (Architecture Intent)
- Frontend: React + TypeScript
- Charts: Recharts or Apache ECharts
- Data import: CSV/JSON upload
- Initial data: mock poverty datasets
- Agent layer: rule-based analysis first, LLM/ OpenAI integration later
- Storage: local browser storage first, database later
- Testing: unit tests, UI tests, manual demo checklists
- Delivery workflow: AI-DLC intent, elaboration, bolt, validation, learning cycle
  - Cycle tracking: issue tracker (Jira or markdown) if available

AI-DLC Intent: Elaboration Layer
- id: intent.elaboration.schema-driven
- description: Dataset schema and metadata drive the whole platform; changes to dataset should regenerate UI, filters, charts, insights, and agent behavior.

AI-DLC Intent: Explainability
- id: intent.explainability.evidence-first
- description: The app should explain semantic meaning, entities, indicators, dimensions, relationships, patterns, tests, predictions, UI rationales, interpretation assumptions, and agent reasoning paths.

Architecture Layer (AI-DLC Architecture Intent)
- Architect agent for system-wide design and stack decisions
- Architecture decision records
- Deployment/DevOps planning (environments, CI/CD, release flow)
- Security, secrets, monitoring, rollback decisions documented early
- Clear separation: product intent, implementation intent, architecture intent

Intent Layer (AI-DLC)
- Holds: product intent, business intent, user intent, functional intent, non-functional intent, architecture intent

Elaboration Phase (AI-DLC artifact)
- Produces: intent briefs, acceptance criteria, assumptions, risks, dependencies, architecture direction, bolt candidates, validation points

Stage Board (MVP Phases)
----------------------
The MVP is organized into stages. Each stage contains bolts. Each bolt is elaborated into units.

MVP Stages
- Stage 1: Data Onboard & Schema
  - Architecture Bolt
  - Foundation Bolt
  - Import Bolt
- Stage 2: Generated UI + Charts
  - Interface Bolt
  - Visualization Bolt
- Stage 3: Basic Analysis & Explainability
  - Pattern Bolt
  - Explainability Bolt
- Stage 4: Testable Report + Polish
  - Statistics Bolt
  - Conversation Bolt
  - Reasoning Bolt
  - Narrative Bolt
  - Workspace Bolt
  - Delivery Bolt

Bolt Board (AI-DLC)
---------------------
The Bolt Board lists Bolts (named per original Bolt Sets). Each Bolt contains Units (explicit tasks produced during bolt elaboration). Each Unit should have: one outcome, one owner agent, one input set, one output set, one validation check, and steering point if needed.

Agent Roles (AI-DLC Roles)
- Architect Agent
- Design Agent
- Coding Agent
- Testing Agent
- Research Agent
- Knowledge Graph Agent
- Explanation Agent

Validation Gates (AI-DLC)
- Human validation at: intent approval, elaboration approval, architecture approval, bolt approval, integration review, demo review, release approval

Execution Loop (AI-DLC Sequence)
- Intent -> Elaboration -> Stage Selection -> Bolt Decomposition -> Unit Elaboration -> Agent Execution -> Agent Testing -> Human Validation -> Commit/PR/Merge -> Learning Log -> Next Intent

Learning Layer (AI-DLC Data)
- Retain: learning log, AI decision log, assumptions and risks, architecture decision records, review notes, validation notes

Final AI-DLC Structure
- intent board
- elaboration phase
- stage board
- bolt board
- validation gates
- learning layer

AI-DLC Operating Phases (mapped from original)
- Phase A: Setup And Intent
  - Cycle -1: Codex, GitHub, And Cycle Tracking Setup
  - Cycle 0: Conversational AI-DLC Transition And Intent Discovery
- Phase B: AI-DLC Planning And Architecture
  - Cycle 0.5: AI-DLC Operating Model And Planning System
  - Cycle 0.6: Architecture Elaboration And Project Skeleton
- Phase C: AI-DLC Implementation Foundation
  - Cycle 0.7: Foundation And Product Shape
  - Cycle 1: Dataset Import And Schema Detection (Import Bolt)
- Phase D: AI-DLC Capability Bolts
  - Cycle 0.8: Architecture Bolt
  - Cycle 2: Dynamic UI Generator Bolt
  - Cycle 2.5: Ontology Discovery And Semantic Tagging Bolt
  - Cycle 2.6: Expert-Guided Knowledge Graph Enrichment Bolt
  - Cycle 3: Charts And Data Views Bolt
  - Cycle 4: Analysis Engine Bolt
  - Cycle 4.5: Agentic Explainable AI Pattern Discovery Bolt
  - Cycle 4.6: Statistical Modeling And Prediction Engine Bolt
  - Cycle 5: Agentic Explanation Panel Bolt
  - Cycle 6: LLM Agent Integration Bolt
  - Cycle 7: Report Builder Bolt
  - Cycle 8: Dataset Library And Reusability Bolt
  - Cycle 9: Polish, Reliability, And Demo Package Bolt

Bolt Definitions (each bolt is elaborated into Units during bolt elaboration)

Bolt: bolt.architecture.bootstrap (Cycle 0.8)
- Title: Architecture Bolt
- Units:
  - unit.arch.record-adr: Define initial architecture decision records
  - unit.arch.azure-map: Confirm Azure service mapping
  - unit.arch.local-compose: Create local container layout and Docker Compose baseline
  - unit.arch.skeleton: Scaffold frontend and backend shells
  - unit.arch.authn: Define authentication model
  - unit.arch.authz: Define authorization model
  - unit.arch.secrets: Define secrets and environment strategy
  - unit.arch.deployment: Define deployment and health-check baseline
- Validation:
  - Architecture skeleton, auth model, Azure mapping, and local container workflow are documented and reviewable
