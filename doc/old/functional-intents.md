# Functional Intents

## Product Functional Intent

The product must help a user turn an imported dataset into an explainable, interactive, agentic data analysis experience.


## F1: Dataset Import

The system must allow users to import CSV and JSON datasets.

Acceptance criteria:
- User can select a local CSV file.
- User can select a local JSON file.
- User can preview imported rows.
- Invalid files show a clear error.


## F2: Schema Detection

The system must infer column structure.

Acceptance criteria:
- Numeric columns are detected.
- Categorical columns are detected.
- Time columns are detected.
- Geography columns are detected when possible.
- User can correct detected roles.


## F3: Ontology Discovery

The system must identify semantic meaning in the dataset.

Acceptance criteria:
- Entities are identified.
- Indicators are identified.
- Dimensions are identified.
- Units are identified where possible.
- Semantic tags are shown with confidence and reason.
- User can correct semantic tags.


## F4: Dynamic UI Generation

The system must generate the interface from schema, metadata, and ontology.

Acceptance criteria:
- Measures create measure selectors.
- Dimensions create filters.
- Time fields create time controls.
- Geography fields create entity selectors or ranking views.
- The app can explain why each UI element was generated.


## F4.5: Expert-Guided Knowledge Graph Enrichment

The system must let users and local experts enrich the discovered ontology with validated knowledge, relationships, and evidence.

Acceptance criteria:
- User can add entities to the knowledge graph.
- User can add relationships between entities.
- User can capture expert knowledge through conversation.
- User can attach documents, photos, videos, notes, and URLs as evidence.
- Extracted expert claims require human approval before becoming trusted knowledge.
- Claims include provenance and confidence.
- Agent answers distinguish dataset facts from expert knowledge.


## F5: Visualization

The system must create useful data views.

Acceptance criteria:
- Line chart works for time series.
- Bar chart works for category comparison.
- Ranking table works for latest values.
- Summary cards show key metrics.
- Empty states are understandable.


## F6: Pattern Discovery

The system must discover useful patterns.

Acceptance criteria:
- Trends are detected.
- Outliers are detected.
- Group gaps are detected.
- Convergence/divergence can be detected where data supports it.
- Each pattern includes evidence.
- Each pattern includes confidence, importance, and caveats.


## F7: Statistical Modeling

The system must run basic statistical analysis where appropriate.

Acceptance criteria:
- Method recommender suggests a suitable test/model.
- Descriptive statistics work.
- t-test baseline works for two-group comparisons.
- ANOVA baseline works for multi-group comparisons.
- Correlation works for two numeric indicators.
- Basic forecast works for time-series data.
- Statistical output explains assumptions and uncertainty.


## F8: Agentic Explanation

The system must answer natural-language questions using grounded data context.

Acceptance criteria:
- Agent explains selected charts.
- Agent explains dataset ontology.
- Agent explains why UI controls were generated.
- Agent explains patterns with evidence.
- Agent explains statistical results with caveats.
- Agent avoids inventing values.


## F9: Report Generation

The system must generate narrative reports.

Acceptance criteria:
- Report includes dataset summary.
- Report includes key findings.
- Report includes pattern evidence.
- Report includes statistical findings where available.
- Report includes data quality caveats.
- Markdown export works.


## F10: Delivery Tracking

The project must track implementation progress.

Acceptance criteria:
- Sprint tracker exists.
- Backlog exists.
- Review notes exist.
- Jira can be used if available.
- Markdown fallback remains usable.
