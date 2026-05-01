# Nethra Data Explorer

## Concept

Nethra Data Explorer is an agentic, explainable data intelligence platform.

Users import a dataset, and the system:
- understands schema and ontology
- builds the interface dynamically
- discovers patterns and runs statistics
- explains findings with evidence
- supports expert knowledge enrichment
- generates reports
- runs locally in containers first
- later deploys to Azure

The first domain is poverty tracking, but the structure is designed for other domains without creating one custom page per dataset.

## Concept Diagram

![Nethra Logical Architecture](./logical-architecture.png)

## AI-DLC Operating Model

```mermaid
flowchart TD
    A[Intent Section] --> B[Elaboration Phase]
    B --> C[Implementation Section]
    C --> D[Stage 1]
    D --> E[Stage 2]
    E --> F[Stage 3]
    F --> G[Stage 4]
    G --> H[Validation Gates]
    H --> I[Learning Layer]
    H --> B
```

## Intent Section

- Product Intent
- Business Intent
- User Intent
- Functional Intent
- Non-Functional Intent
- Architecture Intent
- Delivery Intent

## Implementation Section

### Stage 1: Data Onboard and Schema
- Architecture Bolt
- Foundation Bolt
- Import Bolt

### Stage 2: Generated UI and Charts
- Interface Bolt
- Visualization Bolt

### Stage 3: Basic Analysis and Explainability
- Pattern Bolt
- Explainability Bolt

### Stage 4: Testable Report and Polish
- Statistics Bolt
- Conversation Bolt
- Reasoning Bolt
- Narrative Bolt
- Workspace Bolt
- Delivery Bolt

## Unit Elaboration Rule

Units are produced during bolt elaboration.

Each stage is an MVP slice. Each bolt inside a stage is broken into units to make implementation easier and more agent-friendly.

## Bolt Structure

- Architecture Bolt
- Foundation Bolt
- Import Bolt
- Interface Bolt
- Meaning Bolt
- Knowledge Bolt
- Visualization Bolt
- Pattern Bolt
- Explainability Bolt
- Statistics Bolt
- Conversation Bolt
- Reasoning Bolt
- Narrative Bolt
- Workspace Bolt
- Delivery Bolt

## MVP Execution Loop

Intent Section -> Elaboration Phase -> Implementation Section -> Stage -> Bolt -> Unit -> Validation -> Learning

## Reference Assets

- [Logical Architecture Image](./logical-architecture.png)
- [AI-DLC Operating Model](./ai-dlc-operating-model.md)
- [MVP Bolt Catalog](./mvp-bolts.md)