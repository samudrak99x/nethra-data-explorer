# Initial OWID Agentic Product Research

## Research Question

How should Nethra Data Explorer learn from Our World in Data, and what would a modern agentic version of the OWID concept look like?


## Key Findings

Our World in Data is best understood as a trusted data-publication and data-storytelling platform. Its strength is not only charts, but the combination of research narrative, curated datasets, reusable visualizations, transparent sources, downloads, embeds, and open-source tooling.

Nethra Data Explorer should not copy OWID page-for-page. It should adopt OWID's trust, source transparency, data reuse, and visualization patterns, then extend them into an agentic experience where user-imported datasets are understood dynamically through schema inference, ontology discovery, pattern detection, statistical modeling, and explainable AI.


## Observed Product Capabilities

### 1. Research And Data Storytelling

OWID combines articles, datasets, charts, and source context into topic pages. This lets users read interpretation and then inspect the underlying data visually.

Implication for Nethra:
Nethra should support narrative report generation, but its first differentiator should be dynamic analysis from imported data rather than manually authored topic pages.


### 2. Grapher Visualizations

OWID's Grapher supports interactive visualizations with different views such as chart, map, and table. Users can select entities, change time ranges, download data, share charts, and explore in full-screen mode.

Implication for Nethra:
Nethra should treat chart, table, ranking, and future map views as generated views from data schema and ontology, not as manually built pages.


### 3. Source Transparency

OWID emphasizes visible data sources and deeper metadata. This is central to trust.

Implication for Nethra:
Every generated insight, pattern, statistical result, and agent answer should expose evidence, assumptions, metadata, and caveats.


### 4. Data Reuse

OWID supports chart downloads, data downloads, metadata downloads, and embeds. Its Chart Data API makes chart data and metadata addressable through predictable URLs.

Implication for Nethra:
Even in the MVP, exports should be a first-class product concern. Later, Nethra can expose analysis packages: dataset slice, metadata, schema, ontology tags, pattern results, statistical results, and report output.


### 5. Search And Semantic Search

OWID provides search across charts and pages, and its technical docs describe semantic search for indicators through the Data API.

Implication for Nethra:
Nethra's future data discovery layer should support natural-language search over datasets, indicators, ontology tags, and generated findings.


### 6. Open-Source Architecture

OWID publishes its major tools and datasets through GitHub. Important references include `owid/owid-grapher` and `owid/etl`.

Implication for Nethra:
The architecture should be modular and transparent enough that each capability can be tested and evolved separately: parser, schema detector, ontology engine, visualization planner, pattern engine, statistics engine, and agent layer.


## Architecture Observations

OWID technical documentation describes a statically rendered publication model with two primary codebases:

- TypeScript Grapher/publication/admin tooling
- Python ETL pipeline for data loading and transformation

The basic architecture pattern is:

```text
External data sources
  -> ETL pipeline
  -> curated datasets
  -> chart configuration
  -> static/public site
  -> reusable visualizations and chart/data APIs
```

This is a strong model for a publication with curated public datasets.

Nethra needs a different center of gravity:

```text
User-imported dataset
  -> parser
  -> schema inference
  -> ontology discovery
  -> metadata confirmation
  -> dynamic UI generation
  -> visualization and analysis engines
  -> explainable agent
  -> report and export layer
```


## Data/API Observations

OWID's Chart API pattern is especially useful:

- a chart page is available at a Grapher URL
- `.csv` returns chart data
- `.metadata.json` returns chart metadata
- `.zip` returns a package with data and documentation

This suggests a future Nethra export/API pattern:

```text
/datasets/{id}.csv
/datasets/{id}.schema.json
/datasets/{id}.ontology.json
/datasets/{id}.patterns.json
/datasets/{id}.statistics.json
/reports/{id}.md
```

This would make Nethra's analysis reusable, inspectable, and easier to integrate with notebooks or external systems.


## Agentic Opportunity Gaps

OWID is excellent at curated public knowledge, but it is not primarily a user-imported agentic analysis system.

Nethra can go beyond OWID by adding:

- schema inference for arbitrary datasets
- ontology discovery and semantic tagging
- explainable UI generation
- pattern discovery with evidence and confidence
- statistical method recommendation
- hypothesis testing and ANOVA
- forecasting with uncertainty
- natural-language analysis questions
- agentic report generation
- audit trail of AI/analysis decisions
- human correction loops for schema and ontology


## Hypothetical Modern Agentic Version

A modern agentic OWID-like product would include:

```text
Data onboarding agent
  -> understands uploaded data and metadata

Ontology agent
  -> identifies entities, dimensions, indicators, units, and relationships

Visualization planner
  -> creates charts, tables, filters, rankings, and maps from data meaning

Pattern discovery engine
  -> detects trends, gaps, outliers, shifts, convergence, and volatility

Statistical reasoning engine
  -> recommends tests, runs models, explains assumptions and uncertainty

Explanation agent
  -> answers questions with evidence, caveats, and citations

Report agent
  -> turns selected findings into a narrative output

Audit layer
  -> records assumptions, user corrections, decisions, and generated outputs
```


## Implications For Nethra Data Explorer

### Adopt From OWID

- Source transparency
- Reusable data/metadata downloads
- Multiple views of the same data
- Entity selection and comparison
- Chart/table/map view pattern
- Strong citation and caveat discipline
- Open and inspectable architecture


### Improve Beyond OWID

- Make the interface generated from imported datasets.
- Add ontology discovery.
- Add explainable pattern detection.
- Add statistical analysis and prediction.
- Add agentic questions and answers.
- Add human correction loops.
- Add analysis audit trail.


### Avoid

- Hardcoding one topic page per dataset.
- Producing unexplained charts.
- Letting the agent invent facts.
- Treating forecasts as facts.
- Hiding schema or ontology assumptions.


## Risks And Assumptions

### Risks

- OWID is curated by expert humans; Nethra must not imply imported data has the same quality automatically.
- Agentic explanations may overstate weak data.
- Statistical outputs can be misunderstood without clear caveats.
- Dynamic UI generation can become confusing if explanations are weak.
- External APIs and OWID internals may change over time.


### Assumptions

- MVP starts with user-uploaded CSV/JSON.
- Poverty tracking remains the first domain.
- Deterministic engines come before LLM integration.
- OWID is a product inspiration, not a system to clone exactly.
- Nethra's differentiator is explainable agentic analysis over imported datasets.


## Recommended Next Experiments

1. Build a small OWID-style dataset fixture for poverty tracking.
2. Create a schema and ontology detection proof of concept.
3. Generate three views from the same dataset: line chart, ranking table, summary cards.
4. Add "why this UI was generated" explanations.
5. Add a first pattern card with evidence.
6. Add an export package format inspired by OWID's chart data package.
7. Research comparable tools in more depth: Datawrapper, Flourish, Observable, Google Data Commons, Tableau/Power BI AI features, and emerging AI data analyst tools.


## Sources

- Our World in Data Grapher redesign: https://ourworldindata.org/redesigning-our-interactive-data-visualizations
- OWID data reuse and Chart Data API announcement: https://ourworldindata.org/easier-to-reuse-our-data
- OWID Chart API docs: https://docs.owid.io/projects/etl/api/chart-api/
- OWID Search API docs: https://docs.owid.io/projects/etl/api/search-api/
- OWID GitHub organization: https://github.com/owid
- OWID architecture overview: https://owid-grapher.readthedocs.io/en/docs-revamp-2023/architecture/
- OWID FAQ on embeds: https://ourworldindata.org/faqs
- OWID archived chart embeds: https://ourworldindata.org/new-feature-embed-archived-charts
