---
name: product-ba-po-intent
description: Use when working on the Nethra Data Explorer product and needing BA/PO context, product intent, functional and non-functional requirements, acceptance criteria, or AI-DLC intent framing before implementation.
---

# Product BA/PO Intent Skill

Use this skill when implementing or planning Nethra Data Explorer work.

## Core Workflow

1. Read the relevant intent files before making implementation choices:
   - `product-intent-knowledge-base.md`
   - `functional-intents.md`
   - `non-functional-intents.md`
   - `intent-identification-workflow.md`
   - `aidlc-gap-analysis.md`

2. Before implementation, identify:
   - business intent
   - user intent
   - functional intent
   - non-functional intent
   - acceptance criteria
   - risks and assumptions

3. Preserve these product principles:
   - dataset-driven, not page-driven
   - explainable by default
   - human-correctable
   - evidence-backed
   - deterministic analysis before LLM reasoning
   - no invented data
   - uncertainty shown for predictions

4. Update sprint tracking files after meaningful work:
   - `sprint-progress.md`
   - `sprint-review-notes.md`

## Decision Rules

- If a feature hides assumptions, add an explanation surface.
- If an agent answer uses data, include evidence or caveats.
- If a statistical result is shown, include assumptions and uncertainty.
- If schema or ontology inference is uncertain, let the user correct it.
- If implementation scope grows, record the assumption or risk before proceeding.
