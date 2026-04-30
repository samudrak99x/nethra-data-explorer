---
name: expert-knowledge-graph
description: Use when designing, implementing, or reviewing expert-guided knowledge graph enrichment for Nethra Data Explorer, including expert conversations, evidence uploads, claim extraction, provenance, validation, and agent use of expert knowledge.
---

# Expert Knowledge Graph Skill

Use this skill when work involves enriching discovered ontology with local expert knowledge.

## Core Workflow

1. Start from discovered ontology:
   - entities
   - indicators
   - dimensions
   - units
   - relationships

2. Capture expert knowledge:
   - conversation
   - uploaded documents
   - photos
   - videos
   - meeting notes
   - source URLs

3. Extract candidate knowledge:
   - entities
   - relationships
   - claims
   - definitions
   - caveats
   - local context

4. Require human validation:
   - approve
   - reject
   - edit
   - mark uncertain

5. Store with provenance:
   - who provided it
   - when it was captured
   - what evidence supports it
   - confidence level
   - validation status

6. Use in agent answers carefully:
   - separate dataset facts from expert knowledge
   - cite evidence or provenance
   - mark uncertain or unverified knowledge clearly

## Decision Rules

- Never treat extracted expert claims as trusted until approved.
- Never mix dataset-derived facts and expert knowledge without labeling them.
- If evidence is weak, lower confidence or mark the claim for review.
- If expert knowledge contradicts dataset evidence, show the conflict.
- If media evidence is attached, preserve the link between claim and artifact.
- Prefer transparent provenance over confident but unexplained answers.

