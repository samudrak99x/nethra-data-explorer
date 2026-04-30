# OWID Research Brief

## Purpose

This brief supports research for Nethra Data Explorer by summarizing known Our World in Data capabilities, architecture patterns, APIs, and opportunities for a modern agentic version of the concept.

Use this as a starting point, then verify current facts from official sources when making product or architecture decisions.


## Our World in Data Concept

Our World in Data publishes research and data about major global problems and makes that data accessible through articles, interactive charts, maps, tables, downloads, embeds, and reusable APIs.

Core product pattern:

```text
Research + curated datasets + interactive visualization + source transparency + reuse
```


## Observed OWID Capabilities

### Data Storytelling

- Topic pages combine written research, charts, source context, and interpretation.
- Users can move from narrative explanation into chart exploration.

### Grapher Visualizations

- Interactive visualizations can show multiple views such as chart, map, and table.
- Users can select countries/entities, change time spans, download data, share charts, and use full-screen exploration.
- Charts show source information and deeper metadata through data/source overlays.

### Reuse And Embedding

- Charts can be embedded on other websites.
- Users can choose live embeds that update or archived embeds that remain fixed.
- Download and sharing workflows are first-class product features.

### Chart Data API

- Grapher chart URLs can expose data and metadata through predictable file extensions:
  - `.csv`
  - `.metadata.json`
  - `.zip`
- Data can be accessed directly from chart URLs.

### Search

- OWID provides search across charts and pages.
- Technical docs describe a Search API powered by Algolia.
- OWID also documents semantic search for indicators through the Data API.

### Open Source

- OWID publishes software and data repositories on GitHub.
- Key repositories include:
  - `owid/owid-grapher`
  - `owid/etl`
  - topic datasets such as CO2 and energy data


## Observed Architecture Pattern

OWID technical documentation describes a statically rendered publication model with major codebases:

- `owid-grapher`: TypeScript project for publication, admin tools, and interactive visualizations.
- `etl`: Python data pipeline for loading and transforming datasets.

High-level pattern:

```text
Data sources -> ETL pipeline -> curated datasets -> Grapher configs -> static/public site -> reusable chart/data APIs
```


## Gaps And Agentic Opportunities

OWID is strong at curated, trusted, reusable public data storytelling.

Nethra Data Explorer can go beyond the classic OWID pattern by adding:

- user-imported datasets
- automatic schema detection
- ontology discovery
- semantic tagging
- dynamic UI generation
- explainable pattern discovery
- statistical method recommendation
- hypothesis testing
- forecasting
- natural-language data questions
- agent explanations with evidence
- explainable UI generation
- AI-DLC style audit trail for analysis decisions


## Hypothetical Agentic OWID-Style Architecture

```text
Data ingestion
  -> Schema inference
  -> Ontology discovery
  -> Metadata and source validation
  -> Dynamic visualization planner
  -> Pattern discovery engine
  -> Statistical modeling engine
  -> Agent context builder
  -> Explainable agent interface
  -> Report/story generator
  -> Audit and citation layer
```


## Comparable Product Categories To Research

These are not direct equivalents, but useful comparison categories:

- data storytelling platforms
- BI dashboards
- notebook-based data analysis
- automated insight platforms
- semantic data catalogs
- agentic analytics tools
- chart embedding/API platforms

Examples to research with official sources when needed:

- Datawrapper
- Flourish
- Observable
- Plotly/Dash
- Tableau
- Power BI
- Google Data Commons
- Wolfram Alpha / Wolfram Data Repository
- Data catalogs with semantic metadata
- emerging AI data analyst tools


## Nethra Research Output Template

Use this structure for research findings:

```text
Research question:

Key findings:

Observed product capabilities:

Architecture observations:

Data/API observations:

Agentic opportunity gaps:

Implications for Nethra Data Explorer:

Risks and assumptions:

Recommended next experiments:

Sources:
```


## Initial Sources

- OWID Grapher redesign: https://ourworldindata.org/redesigning-our-interactive-data-visualizations
- OWID data reuse and Chart Data API: https://ourworldindata.org/easier-to-reuse-our-data
- OWID Chart API docs: https://docs.owid.io/projects/etl/api/chart-api/
- OWID Search API docs: https://docs.owid.io/projects/etl/api/search-api/
- OWID GitHub organization: https://github.com/owid
- OWID architecture overview: https://owid-grapher.readthedocs.io/en/docs-revamp-2023/architecture/
- OWID FAQ on embeds: https://ourworldindata.org/faqs
- OWID archived chart embeds: https://ourworldindata.org/new-feature-embed-archived-charts
