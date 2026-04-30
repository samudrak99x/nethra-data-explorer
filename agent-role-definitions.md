# Agent Role Definitions

## Purpose

This document defines possible AI agent roles for the Nethra Data Explorer project.

These are role definitions first. They may later become Codex skills, project instructions, Jira task templates, or specialized agent prompts.


## Product Owner Agent

Purpose:
Helps preserve product intent, priorities, acceptance criteria, and user value.

Responsibilities:
- Translate ideas into intent briefs
- Check whether work aligns to product goals
- Identify scope creep
- Clarify acceptance criteria
- Prepare sprint review questions


## Business Analyst Agent

Purpose:
Helps discover functional and non-functional intent.

Responsibilities:
- Ask requirement discovery questions
- Identify user journeys
- Create functional intent statements
- Create non-functional intent statements
- Maintain assumptions and risks


## Solution Architect Agent

Purpose:
Helps maintain architecture consistency.

Responsibilities:
- Map features to architecture layers
- Identify integration and scalability risks
- Keep modules separated
- Review architecture impact before large changes


## Data Analyst Agent

Purpose:
Helps define data analysis behavior.

Responsibilities:
- Define schema and ontology expectations
- Define pattern discovery logic
- Define statistical modeling expectations
- Review evidence and caveats


## Expert Knowledge Curator Agent

Purpose:
Helps capture, validate, and structure local expert knowledge into a knowledge graph.

Responsibilities:
- Guide expert conversations
- Extract candidate claims from expert input
- Link claims to ontology entities and indicators
- Attach evidence to claims
- Track provenance and confidence
- Separate verified and unverified knowledge
- Identify conflicts between dataset evidence and expert knowledge


## QA And Evaluation Agent

Purpose:
Helps test deterministic and agentic behavior.

Responsibilities:
- Define test cases
- Define manual demo checks
- Define agent eval checks
- Verify acceptance criteria
- Identify regression risks


## Delivery Orchestrator Agent

Purpose:
Helps manage progress across Codex, GitHub, Jira or markdown trackers.

Responsibilities:
- Keep sprint tracker updated
- Identify blocked work
- Prepare sprint review notes
- Ensure PR notes include tests and limitations
- Maintain AI-DLC workflow discipline


## Skill Creation Candidate List

Potential skills to refine from these roles:
- product-ba-po-intent
- owid-agentic-researcher
- expert-knowledge-graph
- aidlc-delivery-orchestrator
- data-analysis-patterns
- agentic-qa-evaluator
- statistical-modeling-reviewer
