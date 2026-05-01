# Agent Evaluation Plan

This plan defines how we will evaluate agentic behavior in the product.

## Purpose

Normal unit and UI tests are not enough for agentic features. The product must also check whether agent responses are grounded, explainable, and safe.


## Evaluation Areas

### Data Grounding

Checks:
- Does the answer only use available dataset values?
- Does the answer cite evidence values when making a claim?
- Does it avoid invented countries, columns, years, or measures?


### Ontology Explanation

Checks:
- Can the agent explain what the dataset measures?
- Can it explain entities, indicators, dimensions, and units?
- Can it explain uncertainty in semantic tagging?


### Interface Explanation

Checks:
- Can the agent explain why a filter was generated?
- Can it explain why a chart was recommended?
- Can it explain why a measure selector exists?


### Pattern Explanation

Checks:
- Can the agent explain a detected pattern?
- Does it include evidence?
- Does it separate confidence from importance?
- Does it mention caveats?


### Statistical Explanation

Checks:
- Can the agent explain why a statistical method was selected?
- Can it explain p-values in plain language?
- Can it separate statistical significance from practical importance?
- Can it avoid causal claims unless supported?
- Can it explain prediction uncertainty?


## Initial Eval Questions

- What does this dataset measure?
- Why did the app create these filters?
- What are the strongest patterns in this dataset?
- What evidence supports this pattern?
- Are rural and urban poverty rates significantly different?
- Predict poverty rate for the next three years.
- What data quality issues should I worry about?


## Pass Criteria

An agent response passes when:
- It is grounded in the provided context.
- It does not invent values.
- It includes evidence or caveats for analytical claims.
- It is understandable to a non-technical user.
- It avoids overstating predictions or statistics.
