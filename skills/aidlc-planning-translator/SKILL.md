---
name: aidlc-planning-translator
description: Use when shaping or refining the Nethra Data Explorer AI-DLC plan, separating intent from implementation, defining stage-based MVP slices, or producing planning diagrams and visual artifacts.
---

# AI-DLC Planning Translator

Use this skill when the user wants to plan and deliver Nethra Data Explorer in a pure AI-DLC-native way.

## Nethra Planning Shape

The plan has two clear sections:

1. **Intent Section**
2. **Implementation Section**

The intent section defines what the product should become. The implementation section turns that intent into MVP stages, bolts, and units.

## Core Job

- define the AI-DLC delivery cycle for Nethra Data Explorer
- keep intent separate from implementation
- express implementation as Stage -> Bolt -> Unit
- identify where humans steer, approve, and validate
- keep the terminology consistent across plans, skills, and sprint trackers
- produce visual representations when asked

## First Read

Before changing the operating model, read:

- `doc/ai-dlc-operating-model.md`
- `doc/ai-dlc/mvp-bolts.md`
- `doc/ai-dlc/task-plan-aidlc.md`
- `doc/scrum-to-aidlc-transition-map.md`
- `doc/conversational-discovery-log.md`
- `doc/aidlc-gap-analysis.md`
- `doc/intent-identification-workflow.md`
- `doc/architecture-decision-records.md`
- `doc/sprint-progress.md`

## Use This Skill To

- define intent types for Nethra Data Explorer
- shape the implementation section into MVP stages
- split each stage into bolts
- split each bolt into units during bolt elaboration
- define human validation gates
- create a new planning cycle that is native to AI-DLC
- rewrite planning artifacts so they reflect the new operating model
- generate or refresh architecture and planning diagrams
- produce text plus visual summaries for intent, stage, bolt, and unit structure

## Planning Rules

- Start from the intent section, not implementation wording.
- Keep intent stable and readable.
- Use elaboration to turn stage-level intent into executable shape.
- Keep humans at the steering points, not in every micro-task.
- Make bolts small enough for an agent to execute and test.
- Derive units only during bolt elaboration.
- Capture assumptions, risks, and decision points explicitly.
- Prefer visible iteration over hidden coordination.
- When the user asks for a diagram, include a Mermaid version by default and a bitmap image when a visual asset is useful.

## Output Shape

When updating plans, produce:

- intent section
- implementation section
- terminology map
- AI-DLC operating cycle
- human/agent responsibility split
- planning artifact updates
- new sprint or phase structure if needed
- open questions that need human steering
- stage -> bolt -> unit breakdown
- visual diagram or image reference when requested

## Default AI-DLC Cycle

1. Intent capture
2. Intent elaboration
3. Stage selection
4. Bolt decomposition
5. Unit elaboration
6. Agent execution
7. Agent testing
8. Human validation
9. Commit / PR / review
10. Learning log update

## Visual Output Rule

When the user asks for a visual representation, prefer:

1. a Mermaid diagram in Markdown for fast review
2. a saved image file when the user wants a shareable diagram or concept graphic

Keep the visual aligned to the current planning model:

- Intent Board
- Elaboration Phase
- Implementation Stage Board
- Bolt Board
- Unit Elaboration
- Validation Gates
- Learning Layer

## ASCII Visual Style

When a compact text visual is enough, use simple ASCII layouts that read well in chat:

### Core flow

```text
Intent
  ↓
Elaboration
  ↓
Implementation Stage
  ↓
Bolt
  ↓
Unit
  ↓
Validation
  ↓
Learning
```

### Stage to bolt structure

```text
Stage 1
  ├─ Architecture Bolt
  ├─ Foundation Bolt
  └─ Import Bolt

Stage 2
  ├─ Interface Bolt
  └─ Visualization Bolt
```

### Bolt to unit structure

```text
Import Bolt
  ├─ upload CSV
  ├─ upload JSON
  ├─ preview rows
  ├─ infer schema
  └─ save metadata
```

## Nethra Intent Types

When planning Nethra, keep the intent section split into:

- Product Intent
- Business Intent
- User Intent
- Functional Intent
- Non-Functional Intent
- Architecture Intent
- Delivery Intent

## Nethra Implementation Stages

When planning implementation, use clear MVP stages:

- Stage 1: Data Onboard & Schema
- Stage 2: Generated UI + Charts
- Stage 3: Basic Analysis & Explainability
- Stage 4: Testable Report + Polish

Each stage may contain multiple bolts, and each bolt is elaborated into units.

Keep ASCII visuals:
- narrow
- readable on mobile
- free of decorative clutter
- aligned to the current AI-DLC plan
