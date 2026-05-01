# Nethra Data Explorer AI-DLC Operating Model

## Intent Board

The source of truth for:
- product intent
- business intent
- user intent
- functional intent
- non-functional intent
- architecture intent

Each intent defines:
- outcome
- value
- constraints
- success criteria
- validation needs

## Elaboration Phase

This phase turns intent into delivery-ready shape through:
- intent briefs
- acceptance criteria
- assumptions
- risks
- dependencies
- architecture direction
- bolt candidates
- validation points

## Stage -> Bolt -> Unit Model

The MVP is organized as stages.
Each stage contains bolts.
Each bolt is elaborated into units.

## Bolt Board

The execution surface.

Each bolt has:
- one outcome
- one owner agent
- one input set
- one output set
- one validation check
- one steering point if needed

The first bolt is the Architecture Bolt, which creates the initial system skeleton, Azure mapping, container workflow, auth, and deployment baseline before other bolts begin.

## Agent Roles

- Architect Agent
- Design Agent
- Coding Agent
- Testing Agent
- Research Agent
- Knowledge Graph Agent
- Explanation Agent

## Validation Gates

Human validation happens at:
- intent approval
- elaboration approval
- architecture approval
- bolt approval
- integration review
- demo review
- release approval

## Execution Loop

Intent -> Elaboration -> Stage Selection -> Bolt Decomposition -> Unit Elaboration -> Agent Execution -> Agent Testing -> Human Validation -> Commit / PR / Merge -> Learning Log -> Next Intent

## Learning Layer

Retain:
- learning log
- AI decision log
- assumptions and risks
- architecture decision records
- review notes
- validation notes

## Final Delivery Structure

- Intent Board
- Elaboration Phase
- Stage Board
- Bolt Board
- Validation Gates
- Learning Layer