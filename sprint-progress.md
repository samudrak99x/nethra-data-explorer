# Sprint Progress Tracker

Status marks:
- [ ] Not Started
- [~] In Progress
- [!] Blocked
- [x] Done

## Delivery Phases

### Phase A: Setup And Intent

Run together:
- Sprint -1: Codex, GitHub, And Sprint Tracking Setup
- Sprint 0: Conversational AI-DLC Transition And Intent Discovery

### Phase B: First Implementation

Run together after Phase A has enough context:
- Sprint 0.5: Foundation And Product Shape
- Sprint 1: Dataset Import And Schema Detection

### Phase C: Product Capability Sprints

Run after Phase B:
- Sprint 2 onward

## Sprint -1: Codex, GitHub, And Sprint Tracking Setup

- [x] Select or create GitHub repository
- [x] Confirm Codex can access the repository workspace
- [x] Rename local project repository to nethra-data-explorer
- [x] Prepare nethra-data-explorer as Codex project root
- [x] Link local repo to GitHub remote origin
- [!] Confirm Git identity for commits
- [x] Confirm GitHub authentication
- [x] Configure GitHub MCP/app access if needed
- [x] Verify branch creation
- [x] Verify commit workflow
- [x] Push branch to GitHub remote
- [!] Verify pull request workflow
- [x] Create PR template
- [x] Check Jira MCP availability
- [ ] Configure Jira project/board if available
- [ ] Create Jira epics and sprint tasks if available
- [x] Create markdown progress tracker fallback
- [x] Create sprint backlog file
- [x] Create sprint review notes file
- [x] Create AI-DLC gap analysis document
- [x] Create intent brief template
- [x] Create AI decision log
- [x] Create AI-specific Definition of Done
- [x] Create agent evaluation plan

## Sprint 0: Conversational AI-DLC Transition And Intent Discovery

- [x] Create intent identification workflow document
- [x] Create functional intents document
- [x] Create non-functional intents document
- [x] Create intent brief template
- [x] Create Scrum-to-AI-DLC terminology map
- [x] Create conversational discovery log
- [x] Create assumptions and risks section
- [x] Create acceptance criteria catalog
- [x] Create project-local BA/PO skill draft
- [x] Create project-local OWID agentic researcher skill
- [x] Create initial OWID agentic research report
- [x] Add expert-guided knowledge graph enrichment to plan
- [x] Create project-local expert knowledge graph skill
- [x] Create initial agent role definitions
- [ ] Decide which agent roles should become skills
- [ ] Refine product skills progressively
- [ ] Review intent documents before implementation

## Sprint 0.5: Foundation And Product Shape

- [ ] Create React project structure
- [ ] Create app layout
- [ ] Add mock poverty CSV/JSON
- [ ] Define DatasetSchema TypeScript types
- [ ] Define DatasetMetadata TypeScript types
- [ ] Build static mock "Dataset loaded" screen
- [ ] Add basic navigation

## Sprint 1: Dataset Import And Schema Detection

- [ ] Build file upload component
- [ ] Parse CSV and JSON
- [ ] Show first 20 rows in preview
- [ ] Implement schema inference engine
- [ ] Add confidence labels
- [ ] Allow user to correct column roles manually

## Sprint 2: Dynamic UI Generator

- [ ] Build UI generation rules
- [ ] Generate filters from dimensions
- [ ] Generate measure dropdown from measures
- [ ] Generate default chart config
- [ ] Add selected dataset state management
- [ ] Build reusable chart container

## Sprint 2.5: Ontology Discovery And Semantic Tagging

- [ ] Define OntologyModel TypeScript types
- [ ] Define SemanticTag TypeScript types
- [ ] Build semantic tagging rules for poverty datasets
- [ ] Build column-to-concept mapping
- [ ] Detect indicators versus dimensions
- [ ] Detect derived or related measures where possible
- [ ] Add ontology discovery panel
- [ ] Allow users to approve or correct semantic tags
- [ ] Store approved ontology with dataset metadata

## Sprint 3: Charts And Data Views

- [ ] Add chart library
- [ ] Build line chart component
- [ ] Build bar chart component
- [ ] Build ranking table
- [ ] Implement data filtering pipeline
- [ ] Implement latest-year calculation
- [ ] Add empty states
- [ ] Add chart loading/error states

## Sprint 4: Analysis Engine

- [ ] Build analysis utility functions
- [ ] Build trend scoring
- [ ] Build anomaly detection
- [ ] Build pattern discovery engine
- [ ] Build pattern scoring and ranking
- [ ] Build explainable evidence output for each pattern
- [ ] Build data quality report
- [ ] Connect insights to selected filters
- [ ] Add insight cards panel

## Sprint 4.5: Agentic Explainable AI Pattern Discovery

- [ ] Define PatternResult TypeScript model
- [ ] Define PatternEvidence TypeScript model
- [ ] Implement pattern detection functions
- [ ] Implement pattern ranking logic
- [ ] Implement confidence scoring
- [ ] Implement importance scoring
- [ ] Build pattern cards UI
- [ ] Build pattern detail/evidence drawer
- [ ] Connect pattern results to agent context
- [ ] Add explainable AI prompt/response rules

## Sprint 4.6: Statistical Modeling And Prediction Engine

- [ ] Define StatisticalModelResult TypeScript model
- [ ] Define HypothesisTestResult model
- [ ] Define ForecastResult model
- [ ] Implement descriptive statistics utilities
- [ ] Implement method recommendation rules
- [ ] Implement ANOVA baseline
- [ ] Implement t-test baseline
- [ ] Implement chi-square baseline where appropriate
- [ ] Implement correlation analysis
- [ ] Implement simple linear regression baseline
- [ ] Implement simple time-series forecasting baseline
- [ ] Build statistical model cards UI
- [ ] Build assumptions and limitations UI
- [ ] Connect statistical results to agent context
- [ ] Add explainable statistical response rules

## Sprint 5: Agentic Explanation Panel

- [ ] Build agent chat UI
- [ ] Build prompt/question classifier
- [ ] Connect classifier to analysis engine
- [ ] Connect classifier to ontology model
- [ ] Connect classifier to pattern discovery results
- [ ] Connect classifier to statistical model results
- [ ] Generate natural-language summaries
- [ ] Add suggested follow-up questions
- [ ] Add response cards

## Sprint 6: LLM Agent Integration

- [ ] Create agent API route
- [ ] Build structured analysis payload
- [ ] Add system instructions for data-grounded answers
- [ ] Add response validation
- [ ] Add loading and error states
- [ ] Add fallback to rule-based agent if API fails

## Sprint 7: Report Builder

- [ ] Build report generator
- [ ] Add report preview page
- [ ] Add chart snapshots or chart references
- [ ] Add markdown export
- [ ] Add saved report state

## Sprint 8: Dataset Library And Reusability

- [ ] Add dataset list
- [ ] Add local persistence
- [ ] Add metadata edit screen
- [ ] Add duplicate dataset handling
- [ ] Add sample datasets
- [ ] Add dataset deletion

## Sprint 9: Polish, Reliability, And Demo Package

- [ ] Polish UI
- [ ] Add responsive design checks
- [ ] Add loading skeletons
- [ ] Improve wording
- [ ] Add demo dataset button
- [ ] Add final QA checklist
- [ ] Prepare demo script
