# Acceptance Criteria Catalog

This catalog collects reusable acceptance criteria for the project.

## Dataset Import

- User can import a valid CSV file.
- User can import a valid JSON file.
- User can preview imported rows.
- Invalid files show a clear error.


## Schema Detection

- Numeric columns are detected.
- Categorical columns are detected.
- Time columns are detected.
- Geography columns are detected where possible.
- User can correct detected roles.


## Ontology Discovery

- Entities are identified.
- Indicators are identified.
- Dimensions are identified.
- Units are identified where possible.
- Semantic tags include confidence and reason.
- User can correct semantic tags.


## Dynamic UI

- Measures create measure selectors.
- Dimensions create filters.
- Time fields create time controls.
- Generated UI elements have explainable reasons.


## Pattern Discovery

- Detected patterns include evidence.
- Patterns include confidence and importance.
- Missing data reduces confidence.
- Pattern explanation avoids unsupported causal claims.


## Statistical Modeling

- Method recommendation is visible.
- Statistical result includes assumptions.
- p-value is explained where applicable.
- Effect size or practical importance is shown where applicable.
- Forecasts include uncertainty or caveats.


## Agent Explanation

- Agent answers are grounded in selected data.
- Agent does not invent values.
- Agent cites evidence where appropriate.
- Agent mentions missing data when relevant.
- Agent separates observation from interpretation.


## Delivery

- Sprint tracker is updated.
- Review notes are updated.
- Tests or manual verification are recorded.
- PR notes are prepared when GitHub is connected.
