---
name: poverty-data-researcher
description: Use when researching poverty-tracking datasets, ontology, indicators, hypothesis-testing setup, and candidate test datasets for Nethra Data Explorer.
---

# Poverty Data Researcher

Use this skill when Nethra Data Explorer needs a strong poverty-tracking data foundation.

## Subject Matter Scope

This skill covers:

- poverty tracking ontology
- poverty indicators
- standard poverty tracking domain model
- poverty tracking analysis maturity model
- schema discovery
- hypothesis testing for poverty analysis
- candidate test datasets
- visual explanations and reference images

## Core Job

- find poverty datasets suitable for product testing
- identify the likely schema and ontology shape for poverty tracking
- recommend the best setup for initial exploration
- compare candidate datasets by coverage, granularity, and usability
- map findings back to Nethra Data Explorer MVP stages
- explain which statistical tests fit poverty questions
- provide visual reference assets when useful
- describe the maturity progression from descriptive to explainable and agentic analysis

## First Read

Before researching, read:

- `skills/poverty-data-researcher/references/poverty-research-brief.md`
- `skills/poverty-data-researcher/references/poverty-ontology-guide.md`
- `skills/poverty-data-researcher/references/hypothesis-testing-guide.md`
- `skills/poverty-data-researcher/references/domain-model-guide.md`
- `skills/poverty-data-researcher/references/maturity-model-guide.md`
- `skills/poverty-data-researcher/references/visual-index.md`
- `doc/ai-dlc/nethra-concept.md`
- `doc/ai-dlc/mvp-bolts.md`
- `doc/ai-dlc/task-plan-aidlc.md`

## Research Targets

- poverty headcount, poverty gap, and related measures
- country-year dataset structure
- time coverage and geographic coverage
- indicators, dimensions, units, and relationships
- downloadable formats and API access
- data quality, comparability, and caveats
- best dataset for testing import, schema, ontology, and visualization
- poverty indicators and what they mean
- hypothesis-testing tool selection for poverty questions
- standard poverty tracking domain model
- poverty analysis maturity stages

## Preferred Source Types

- official data catalogs
- official statistics portals
- World Bank poverty resources
- UN or other primary data publishers
- dataset pages with explicit downloads and metadata

## Output Shape

When researching, produce:

- best candidate dataset
- why it fits the MVP
- schema summary
- ontology summary
- likely units and dimensions
- caveats and data quality issues
- sample test questions for the product
- recommended next experiment
- source links
- visual references

## Decision Rules

- Prefer primary and official sources.
- Prefer datasets with clear downloads and metadata.
- Prefer country-year data for the first product test.
- Prefer a dataset with poverty plus related indicators when available.
- Be explicit when a recommendation is an inference.

## Visual Assets

Use these when a visual explanation helps:

- `assets/poverty-ontology.png`
- `assets/hypothesis-testing-toolkit.png`
- `assets/poverty-domain-model.png`
- `assets/poverty-analysis-maturity-model.png`

## Subject Area Outputs

The skill should be able to produce:

- poverty indicator hierarchy
- ontology seed set
- likely schema shape
- recommended hypothesis tests
- dataset recommendation
- fallback dataset
- visual summary of the ontology
- visual summary of the hypothesis-testing toolbox
- visual summary of the domain model
- visual summary of the analysis maturity model

## Expected Recommendation Pattern

The skill should usually answer:

1. what poverty dataset to use first
2. what schema to expect
3. what ontology tags to begin with
4. how to test the Nethra product on that dataset

## Default Poverty Indicators

- poverty headcount ratio
- poverty gap
- number of poor
- extreme poverty rate
- national poverty rate

## Default Hypothesis Testing Tools

- t-test
- Welch t-test
- ANOVA
- Welch ANOVA
- chi-square
- correlation
- linear regression
- Mann-Whitney U
- Kruskal-Wallis
- trend test

## Default Maturity Levels

- Descriptive
- Diagnostic
- Analytical
- Predictive
- Explainable and Agentic
