Nethra Data Explorer — AI-DLC Operating Plan (AI-DLC Version)
=============================================================

This AI-DLC formatted document converts the original `task-plan.txt` into explicit AI-DLC artifacts: Intents, Bolts, Units, Agents, Validation gates, and Learning records. Nothing from the original plan is omitted; items are reorganized so each cycle, bolt set, task and test is represented as an AI-DLC entity.

High-level mapping used in this conversion
- Intent: product- or domain-level goal (mapped from Intent Board, Intent Layer)
- Bolt: the smallest useful execution unit (mapped from Bolt Board and Bolt Sets)
- Unit: a task inside a bolt (mapped from Tasks lists)
- Agent Role: actor responsible for bolt/unit (mapped from Agent Roles)
- Validation: test or acceptance criteria (mapped from Testing Plan / Demo At End)
- Learning: logs, decision records, and audit artifacts (mapped from Learning Layer)

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

Bolt Board (AI-DLC)
---------------------
The Bolt Board lists Bolts (named per original Bolt Sets). Each Bolt contains Units (explicit tasks). Each Unit should have: one outcome, one owner agent, one input set, one output set, one validation check, and steering point if needed.

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
- Intent -> Elaboration -> Bolt Decomposition -> Agent Execution -> Agent Testing -> Human Validation -> Commit/PR/Merge -> Learning Log -> Next Intent

Learning Layer (AI-DLC Data)
- Retain: learning log, AI decision log, assumptions and risks, architecture decision records, review notes, validation notes

Final AI-DLC Structure
- intent board
- elaboration phase
- architecture layer
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
  - Cycle 1: Dataset Import And Schema Detection (Import Bolt Set)
- Phase D: AI-DLC Capability Bolt Sets
  - Cycle 2: Dynamic UI Generator (Interface Bolt Set)
  - Cycle 2.5: Ontology Discovery And Semantic Tagging (Meaning Bolt Set)
  - Cycle 2.6: Expert-Guided Knowledge Graph Enrichment (Knowledge Bolt Set)
  - Cycle 3: Charts And Data Views (Visualization Bolt Set)
  - Cycle 4: Analysis Engine (Pattern Bolt Set)
  - Cycle 4.5: Agentic Explainable AI Pattern Discovery (Explainability Bolt Set)
  - Cycle 4.6: Statistical Modeling And Prediction Engine (Statistics Bolt Set)
  - Cycle 5: Agentic Explanation Panel (Conversation Bolt Set)
  - Cycle 6: LLM Agent Integration (Reasoning Bolt Set)
  - Cycle 7: Report Builder (Narrative Bolt Set)
  - Cycle 8: Dataset Library And Reusability (Workspace Bolt Set)
  - Cycle 9: Polish, Reliability, And Demo Package (Delivery Bolt Set)

Bolt Definitions (each bolt includes Units mapped from original Tasks)

Bolt: bolt.setup.codex-github (Cycle -1)
- Title: Codex, GitHub, And Cycle Tracking Setup
- Units:
  - unit.setup.connect-github: Create or select GitHub repo for the product
  - unit.setup.codex-access: Confirm Codex can read/write repo workspace
  - unit.setup.git-identity: Confirm Git identity for commits
  - unit.setup.github-auth: Confirm GitHub authentication available
  - unit.setup.mcp-app: Configure GitHub MCP/app access if needed
  - unit.setup.branch-test: Verify Codex can create a branch
  - unit.setup.commit-test: Verify Codex can commit code
  - unit.setup.pr-test: Verify Codex can open/prepare PR
  - unit.setup.pr-template: Create PR template (summary, test evidence, review notes)
  - unit.setup.issue-tracker-config: Configure issue tracker (Jira or markdown) if available
  - unit.setup.issue-project: Create initial issue project/board mapping if available
  - unit.setup.epics: Create initial epics for product areas
  - unit.setup.cycle-issues: Create cycle issues if issue tracker available
  - unit.setup.markdown-fallback: Create markdown cycle tracker files if no issue tracker
  - unit.setup.progress-file: Add simple progress file with status marks
  - unit.setup.status-labels: Define status labels: Not Started, In Progress, Blocked, Done
  - unit.setup.demo-checklist: Define end-of-cycle demo checklist
 - Validation:
  - PR workflow verified; test branch/commit/PR created; markdown tracker present if issue tracker absent

Bolt: bolt.cycle0.intent-discovery (Cycle 0)
- Title: Conversational AI-DLC Transition And Intent Discovery
- Units:
  - unit.intent.functional: Create functional intents document
  - unit.intent.nonfunctional: Create non-functional intents document
  - unit.intent.mapping: Create legacy-process-to-AI-DLC terminology map
  - unit.intent.discovery-log: Create conversational discovery log
  - unit.intent.brief-template: Create intent brief template
  - unit.intent.assumptions-risks: Create assumptions and risks section
  - unit.intent.acceptance-catalog: Create acceptance criteria catalog
  - unit.intent.ba-po-skill: Create project-local BA/PO skill draft
  - unit.intent.agent-roles: Identify needed project agents or roles
  - unit.intent.role-drafts: Draft agent role descriptions
  - unit.intent.skill-decisions: Decide which agent roles become skills/instructions/tracker templates
  - unit.intent.refine-skills: Refine skills and intent docs progressively during Cycle 0
  - unit.intent.link-tracker: Link intent docs from cycle tracker
  - unit.intent.review: Review intent documents before starting implementation
- Validation:
  - Functional intents documented; non-functional intents documented; acceptance criteria testable; BA/PO skill draft exists; agent role drafts exist

Bolt: bolt.phaseb.operating-model (Cycle 0.5)
- Title: AI-DLC Operating Model And Planning System
- Units:
  - unit.operating-model.spec: Draft AI-DLC operating model
  - unit.plan-system: Define planning system artifacts and workflows
  - unit.adoption-criteria: Set adoption/exit criteria for Phase B
- Validation:
  - Operating model documented and linked to cycle tracker

Bolt: bolt.phaseb.architecture-skeleton (Cycle 0.6)
- Title: Architecture Elaboration And Project Skeleton
- Units:
  - unit.arch.skeleton: Create project skeleton (frontend, initial folders)
  - unit.arch.decisions: Start architecture decision records
  - unit.arch.devops: Outline deployment and CI/CD plan
  - unit.arch.security: Document initial security/secrets/monitoring approach
  - unit.arch.separation: Define separation between product/implementation/architecture intent
- Validation:
  - Project skeleton opens; ADRs created; CI/CD and security plan outlines present

Bolt: bolt.foundation.product-shape (Cycle 0.7)
- Title: Foundation And Product Shape
- Units:
  - unit.foundation.react-setup: Create React project structure
  - unit.foundation.app-layout: Create app layout (sidebar, main workspace)
  - unit.foundation.dataset-panel: Add dataset panel
  - unit.foundation.chart-area: Add chart and insight area
  - unit.foundation.agent-placeholder: Add agent panel placeholder
  - unit.foundation.mock-dataset: Add mock poverty CSV/JSON
  - unit.foundation.dataset-schema-types: Define DatasetSchema TypeScript types
  - unit.foundation.dataset-metadata-types: Define DatasetMetadata TypeScript types
  - unit.foundation.dataset-loaded-screen: Build static mock "Dataset loaded" screen
  - unit.foundation.navigation: Add basic navigation
- Validation:
  - App loads; mock dataset readable; metadata parsed; layout works desktop/mobile

Bolt: bolt.import.schema-detection (Cycle 1)
- Title: Dataset Import And Schema Detection
- Units:
  - unit.import.file-upload: Build file upload component
  - unit.import.parse-csv-json: Parse CSV and JSON
  - unit.import.preview: Show first 20 rows in preview
  - unit.import.schema-engine: Implement schema inference engine
  - unit.import.confidence: Add confidence labels
  - unit.import.manual-correct: Allow user to correct column roles manually
- Validation:
  - Upload valid CSV/JSON; handle missing values; confirm schema edits saved; test with poverty mock

Bolt: bolt.ui.dynamic-generator (Cycle 2)
- Title: Dynamic UI Generator
- Units:
  - unit.ui.filter-panel: Build dynamic filter panel
  - unit.ui.country-selector: Country selector
  - unit.ui.region-selector: Region selector
  - unit.ui.year-range: Year range selector/time slider
  - unit.ui.category-filters: Category filters (gender, urban_rural)
  - unit.ui.measure-selector: Dynamic measure selector
  - unit.ui.chart-recommendations: Dynamic chart recommendations
  - unit.ui.default-dashboard: Default dashboard generation
  - unit.ui.rules-engine: Build UI generation rules
  - unit.ui.state-management: Add selected dataset state management
  - unit.ui.reusable-chart-container: Build reusable chart container
- Validation:
  - Datasets with year create time slider; country creates country filter; categories create checkbox filters; multiple measures create metric selector

Bolt: bolt.meaning.ontology-discovery (Cycle 2.5)
- Title: Ontology Discovery And Semantic Tagging
- Units:
  - unit.ontology.model-types: Define OntologyModel TypeScript types
  - unit.ontology.semantic-types: Define SemanticTag TypeScript types
  - unit.ontology.rules: Build semantic tagging rules for poverty datasets
  - unit.ontology.mapping: Build column-to-concept mapping
  - unit.ontology.detect: Detect indicators versus dimensions
  - unit.ontology.derived: Detect derived or related measures
  - unit.ontology.panel: Add ontology discovery panel
  - unit.ontology.user-approval: Allow users to approve/correct semantic tags
  - unit.ontology.store: Store approved ontology with dataset metadata
- Validation:
  - Poverty columns tagged correctly; measures separated from dimensions; user corrections saved

Bolt: bolt.knowledge.kg-enrichment (Cycle 2.6)
- Title: Expert-Guided Knowledge Graph Enrichment
- Units:
  - unit.kg.model: Define KnowledgeGraph model
  - unit.kg.claim-model: Define ExpertClaim model
  - unit.kg.evidence-model: Define EvidenceArtifact model
  - unit.kg.provenance: Define Provenance model
  - unit.kg.editor: Build knowledge graph editor
  - unit.kg.conversation-capture: Build expert conversation capture workflow
  - unit.kg.claim-extraction: Build claim extraction review workflow
  - unit.kg.evidence-attachments: Build evidence attachment workflow
  - unit.kg.link-ontology: Link expert claims to ontology entities and indicators
  - unit.kg.human-approval: Add human approval step before claims become trusted
  - unit.kg.confidence-display: Add confidence and provenance display
  - unit.kg.agent-usage: Connect knowledge graph context to agent answers
- Validation:
  - Add/approve entities; attach evidence; agent cites provenance when used; agent warns when expert knowledge unverified

Bolt: bolt.visualization.charts-views (Cycle 3)
- Title: Charts And Data Views
- Units:
  - unit.charts.add-library: Add chart library
  - unit.charts.line: Build line chart component
  - unit.charts.bar: Build bar chart component
  - unit.charts.ranking-table: Build ranking table
  - unit.charts.summary-cards: Build summary cards
  - unit.charts.empty-states: Add empty states
  - unit.charts.loading-error: Chart loading and error states
  - unit.charts.filter-pipeline: Implement data filtering pipeline
  - unit.charts.latest-year: Implement latest-year calculation
- Validation:
  - Chart updates when filters change; measure selector changes chart; year range changes visible data; country selection changes lines

Bolt: bolt.analysis.pattern-engine (Cycle 4)
- Title: Analysis Engine
- Units:
  - unit.analysis.utils: Build analysis utility functions
  - unit.analysis.trend-scoring: Build trend scoring
  - unit.analysis.anomaly-detection: Build anomaly detection
  - unit.analysis.pattern-discovery: Build pattern discovery engine
  - unit.analysis.pattern-ranking: Build pattern scoring and ranking
  - unit.analysis.evidence-output: Build explainable evidence output for each pattern
  - unit.analysis.data-quality-report: Build data quality report
  - unit.analysis.filter-link: Connect insights to selected filters
  - unit.analysis.insight-cards: Add insight cards panel
- Validation:
  - Known trends/anomalies detected; missing values detected; evidence present; pattern scores reproducible

Bolt: bolt.explainability.pattern-discovery (Cycle 4.5)
- Title: Agentic Explainable AI Pattern Discovery
- Units:
  - unit.pattern.workspace: Pattern discovery workspace
  - unit.pattern.cards: Pattern cards UI
  - unit.pattern.evidence-view: Pattern evidence view
  - unit.pattern.confidence: Pattern confidence score
  - unit.pattern.importance: Pattern importance score
  - unit.pattern.explanation: Pattern explanation
  - unit.pattern.suggested-next: Suggested next investigation
  - unit.pattern.agentic-questions: Agentic pattern questions
  - unit.pattern.models: Define PatternResult, PatternEvidence TypeScript models
  - unit.pattern.implementation: Implement detection, ranking, scoring, evidence, UI
  - unit.pattern.connect-agent: Connect pattern results to agent context
- Validation:
  - Known gap/convergence/outlier patterns detected; evidence included; missing data lowers confidence

Bolt: bolt.statistics.modeling (Cycle 4.6)
- Title: Statistical Modeling And Prediction Engine
- Units:
  - unit.stats.recommender: Statistical method recommender
  - unit.stats.hypothesis-workflow: Hypothesis testing workflow
  - unit.stats.anova-workflow: ANOVA workflow
  - unit.stats.timeseries-workflow: Time-series analysis workflow
  - unit.stats.prediction-workflow: Basic prediction workflow
  - unit.stats.model-cards: Model result cards UI
  - unit.stats.explain-panel: Statistical explanation panel
  - unit.stats.assumptions-panel: Assumptions and limitations panel
  - unit.stats.utils: Implement descriptive stats, t-test, chi-square, correlation, regression, simple forecasting
  - unit.stats.models: Define StatisticalModelResult, HypothesisTestResult, ForecastResult models
  - unit.stats.connect-agent: Connect statistical results to agent context
- Validation:
  - Descriptive stats match fixtures; tests return expected results; warnings for small sample/missing data

Bolt: bolt.agentic.explanation-panel (Cycle 5)
- Title: Agentic Explanation Panel
- Units:
  - unit.agentic.ask-panel: Build ask-a-question panel
  - unit.agentic.suggested-questions: Suggested questions list
  - unit.agentic.rule-agent: Rule-based agent responses
  - unit.agentic.evidence-explanations: Evidence-backed explanations
  - unit.agentic.next-chart: Recommended next chart
  - unit.agentic.caveats: Caveats when data missing
  - unit.agentic.classifier: Prompt/question classifier
  - unit.agentic.connect-analysis: Connect classifier to analysis/ontology/patterns/stats
  - unit.agentic.response-cards: Add response cards UI
- Validation:
  - Ask flows return data-based answers; agent does not invent values; caveats shown when needed

Bolt: bolt.llm.integration (Cycle 6)
- Title: LLM Agent Integration
- Units:
  - unit.llm.api-route: Create agent API route
  - unit.llm.payload: Build structured analysis payload
  - unit.llm.system-instructions: Add system instructions for data-grounded answers
  - unit.llm.guardrails: Guardrails to not invent data; cite values; mention missing data
  - unit.llm.response-modes: Implement response modes (simple, analyst, policy brief, chart rec)
  - unit.llm.validation: Add response validation and rule-based fallback
  - unit.llm.error-handling: Add loading and error states
- Validation:
  - LLM answers match dataset values; missing data acknowledged; fallback works on API fail

Bolt: bolt.reports.report-builder (Cycle 7)
- Title: Report Builder
- Units:
  - unit.report.generator: Build report generator
  - unit.report.sections: Define report sections (Overview, Main Findings, Chart Explanations, Data Caveats, Suggested Next Analysis)
  - unit.report.preview: Build report preview page
  - unit.report.markdown-export: Add markdown export
  - unit.report.saved-state: Add saved report state
  - unit.report.chart-snapshots: Add chart snapshots or references
- Validation:
  - Report uses selected dataset; updates after filters; includes caveats; markdown export works

Bolt: bolt.workspace.dataset-library (Cycle 8)
- Title: Dataset Library And Reusability
- Units:
  - unit.library.dataset-list: Add dataset list
  - unit.library.persistence: Add local persistence
  - unit.library.metadata-editor: Add metadata edit screen
  - unit.library.duplicate-handling: Add duplicate dataset handling
  - unit.library.sample-datasets: Add sample datasets
  - unit.library.delete: Add dataset deletion
  - unit.library.templates: Add dataset templates (poverty, health, education, climate)
  - unit.library.save-load: Save/load workspace
- Validation:
  - Multiple datasets load; switching regenerates UI; saved metadata persists; delete works

Bolt: bolt.delivery.polish-demo (Cycle 9)
- Title: Polish, Reliability, And Demo Package
- Units:
  - unit.delivery.empty-states: Improve empty states
  - unit.delivery.mobile-layout: Improve mobile layout
  - unit.delivery.chart-tooltips: Improve chart tooltips
  - unit.delivery.source-panel: Add data source/citation panel
  - unit.delivery.onboarding: Demo onboarding flow
  - unit.delivery.sample-button: Add demo dataset button
  - unit.delivery.error-handling: Add final error handling
  - unit.delivery.qa-checklist: Add final QA checklist
  - unit.delivery.demo-script: Prepare demo script
- Validation:
  - Full app walkthrough passes; upload dataset; confirm schema; generate UI; ask agent questions; generate report; test desktop/mobile

MVP Feature List (AI-DLC Intent / Must-Have)
- Must Have:
  - CSV/JSON import
  - Schema detection
  - Ontology discovery
  - Semantic tagging
  - Expert-guided knowledge graph enrichment
  - Explainable UI generation
  - Metadata confirmation
  - Dynamic filters
  - Dynamic charts
  - Poverty mock dataset
  - Trend analysis
  - Pattern discovery
  - Explainable AI pattern cards
  - Statistical modeling
  - Hypothesis testing
  - Basic prediction
  - Data quality checks
  - Agent explanation panel
  - Report generation

- Should Have:
  - Multiple datasets
  - Saved local datasets
  - Suggested questions
  - Chart recommendations
  - Markdown export

- Later:
  - Real database
  - User accounts
  - Real OWID-style API ingestion
  - Map visualizations
  - PDF export
  - Scheduled data updates
  - Multi-agent analysis
  - Collaboration

Testing Strategy (AI-DLC Validation Specs)

Unit Tests (mapped units)
- Schema detection
- Ontology discovery
- Semantic tagging
- Knowledge graph enrichment
- Expert claim validation
- Data parsing
- Filtering
- Trend calculation
- Pattern discovery
- Pattern scoring
- Pattern evidence generation
- Statistical model selection
- Hypothesis testing
- Forecasting baseline
- Ranking calculation
- Anomaly detection
- Data quality checks

UI Tests
- Upload flow
- Schema confirmation
- Ontology confirmation
- Knowledge graph editing
- Filter interactions
- Chart switching
- Agent question flow
- Inspect pattern evidence
- Inspect statistical model result
- Report generation

Manual Demo Tests
 - Can a user open it?
 - Can a user see something useful?
 - Can a user interact with it?
 - Can we explain what changed?
 - Is there a visible improvement from the last cycle?

Data Testing
- Use multiple mock datasets: clean poverty, missing values, duplicate rows, no time column, no geography column, multiple measures

First Build Recommendation (AI-DLC Delivery Order)
- Phase A + B together (Preparation cycle): Cycle -1 and Cycle 0, and Cycle 0.5 + 0.6 respectively
- After that: Phase C then Phase D bolts in order listed above

Recommended AI-DLC Delivery Order
- Phase A: Setup And Intent
  - Cycle -1 and Cycle 0 together
Phase B: AI-DLC Planning And Architecture
  - Cycle 0.5 and Cycle 0.6 together
Phase C: Implementation Foundation
  - Cycle 0.7 and Cycle 1
Phase D: Capability Bolt Sets
  - Bolt sets 2 -> 9 in sequence or parallel where dependencies allow

Exit Criteria (per phase)
- Phase A: Codex workspace ready; GitHub/issue-tracker/markdown trackers ready; product intent docs exist; AI-DLC transition map exists; skills and agent roles drafted; user approves context to begin
- Phase B: App opens; mock poverty dataset exists; CSV/JSON import and preview works; schema detection works; user can correct detected schema roles

AI-DLC Metadata and Traceability
- For each Bolt and Unit record:
  - owner agent role
  - inputs (data, docs, configs)
  - outputs (code, UI, models, metadata)
  - validation criteria (unit/integration tests, demo checklist)
  - ADR references and decision logs

Next steps I can take now
- Option A: Commit this AI-DLC converted file to the repo (done).
- Option B: Create a cross-reference section in `doc/task-plan.txt` linking to this AI-DLC file.
- Option C: Expand each Unit with estimated effort, priority, and owner mapping.

If you want Option C, tell me the estimated capacity or prioritization rules and I will annotate units with estimates.
