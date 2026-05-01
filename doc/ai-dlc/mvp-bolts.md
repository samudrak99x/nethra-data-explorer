# Nethra Data Explorer MVP Bolt Catalog

This document captures the MVP stage structure for the first AI-DLC release path.

## MVP Structure

The MVP is organized as stages. Each stage contains bolts. Each bolt is elaborated into units.

## MVP Stages

### Stage 1: Data Onboard & Schema

Includes bolts:
- Architecture Bolt
- Foundation Bolt
- Import Bolt

### Stage 2: Generated UI + Charts

Includes bolts:
- Interface Bolt
- Visualization Bolt

### Stage 3: Basic Analysis & Explainability

Includes bolts:
- Pattern Bolt
- Explainability Bolt

### Stage 4: Testable Report + Polish

Includes bolts:
- Statistics Bolt
- Conversation Bolt
- Reasoning Bolt
- Narrative Bolt
- Workspace Bolt
- Delivery Bolt

### Architecture Bolt

Purpose:
Establish the technical foundation before feature work starts.

Units:
- define initial architecture decision records
- confirm Azure service mapping
- create local container layout and Docker Compose baseline
- scaffold frontend and backend shells
- define authentication model
- define authorization model
- define secrets and environment strategy
- define deployment and health-check baseline

### Foundation Bolt

Purpose:
Create the initial app shell and product structure.

Units:
- create React project structure
- create app layout
- add dataset panel
- add chart and insight area
- add agent panel placeholder
- add mock poverty CSV/JSON
- define DatasetSchema types
- define DatasetMetadata types
- build static dataset-loaded screen
- add basic navigation

### Import Bolt

Purpose:
Import datasets and detect structure.

Units:
- build file upload component
- parse CSV and JSON
- show preview rows
- implement schema inference engine
- add confidence labels
- allow user correction of detected roles

### Interface Bolt

Purpose:
Generate the UI from dataset structure.

Units:
- build filter generation rules
- generate filters from dimensions
- generate measure selector
- generate chart options
- build reusable chart container
- manage selected dataset state

### Meaning Bolt

Purpose:
Discover ontology and semantic tags.

Units:
- define ontology model types
- define semantic tag types
- build semantic tagging rules
- map columns to concepts
- detect indicators and dimensions
- allow users to approve or correct tags

### Knowledge Bolt

Purpose:
Enrich ontology with expert knowledge.

Units:
- capture expert conversations
- accept document, image, and video evidence
- extract claims
- track provenance
- validate expert knowledge
- update knowledge graph

### Visualization Bolt

Purpose:
Render the data as charts and views.

Units:
- build line chart
- build bar chart
- build ranking table
- build summary cards
- implement filtering pipeline
- implement latest-year calculation

### Pattern Bolt

Purpose:
Detect trends and changes.

Units:
- build trend scoring
- build anomaly detection
- build pattern discovery engine
- build pattern scoring and ranking
- produce explainable evidence for each pattern

### Explainability Bolt

Purpose:
Turn patterns into understandable findings.

Units:
- define pattern result model
- define pattern evidence model
- build pattern cards UI
- build pattern detail drawer
- connect results to agent context
- add explainable AI response rules

### Statistics Bolt

Purpose:
Run baseline statistical analysis and prediction.

Units:
- define statistical model result types
- define hypothesis test result types
- define forecast result types
- implement descriptive statistics
- implement ANOVA baseline
- implement t-test baseline
- implement chi-square baseline where appropriate
- implement correlation analysis
- implement simple linear regression baseline
- implement simple time-series forecast baseline

### Conversation Bolt

Purpose:
Enable interactive agent explanation.

Units:
- build agent chat UI
- build prompt classifier
- connect classifier to analysis results
- connect classifier to ontology results
- connect classifier to statistical results
- generate natural-language summaries

### Reasoning Bolt

Purpose:
Add LLM-backed reasoning with guardrails.

Units:
- create agent API route
- build structured analysis payload
- add system instructions for grounded answers
- add response validation
- add fallback to rule-based agent

### Narrative Bolt

Purpose:
Generate reports.

Units:
- build report generator
- add report preview
- add markdown export
- add saved report state

### Workspace Bolt

Purpose:
Support reuse and persistence.

Units:
- add dataset list
- add local persistence
- add metadata edit screen
- add duplicate dataset handling
- add sample datasets
- add dataset deletion

### Delivery Bolt

Purpose:
Polish and prepare the product for review.

Units:
- polish UI
- add responsive design checks
- add loading skeletons
- improve wording
- add demo dataset button
- add final QA checklist
- prepare demo script

## Bolt Rules

- One intent per bolt
- One owner agent per bolt
- One outcome per bolt
- One validation check per bolt
- Use steering points for ambiguous or high-risk bolts
- Units are created during bolt elaboration and capture the actionable steps for the bolt

## MVP Exit Condition

The MVP is complete when every MVP stage has its bolts defined, each bolt has been elaborated into units, and the first cycle can be executed end to end.
