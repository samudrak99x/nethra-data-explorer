# Poverty Research Brief

Use this brief to guide research for poverty-tracking datasets and ontology setup.

## Main Goals

- identify a strong test dataset for Nethra Data Explorer
- understand poverty indicators and their schema
- understand how poverty data is usually structured
- find a dataset suitable for import, schema detection, ontology discovery, visualization, and explainability tests

## Strong Candidate Sources

- World Bank Poverty and Equity Database / Poverty and Inequality Platform
  - https://datacatalog.worldbank.org/search/dataset/0038020/poverty-and-equity-database-poverty-and-inequality-platform
- Our World in Data poverty topic
  - https://ourworldindata.org/poverty
  - https://ourworldindata.org/extreme-poverty

## Why These Sources Matter

- clear metadata
- country-year coverage
- downloadable files
- poverty-related indicators
- enough structure to test schema detection and ontology tagging

## Likely Starting Ontology

- entity: country
- time: year
- indicator: poverty headcount
- indicator: poverty gap
- indicator: number of poor
- indicator: income or consumption distribution
- dimension: poverty line
- dimension: region
- unit: percent
- unit: people
- unit: international dollars

## Research Questions

- Which dataset is best for the first product test?
- What columns or fields are likely to appear?
- What caveats affect comparability?
- What indicators should become semantic tags first?
- What visualizations are most useful for early validation?

## Expected Deliverable

The research should end with:

- one recommended dataset for testing
- one fallback dataset
- a likely schema shape
- a likely ontology seed set
- suggested MVP test scenarios
