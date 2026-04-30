# Assumptions And Risks

## Assumptions

- MVP starts with local CSV and JSON datasets.
- Poverty tracking is the first domain.
- The app should be dataset-driven, not hardcoded by topic page.
- Local browser storage is acceptable for early MVP.
- Rule-based analysis should come before LLM integration.
- LLM integration should use structured summaries and computed facts where possible.
- Jira is optional; markdown tracking is acceptable until Jira MCP is available.
- GitHub workflow should be added before serious implementation work.


## Product Risks

- Dynamic UI generation may produce confusing interfaces.
- Schema detection may be wrong.
- Ontology tagging may be wrong.
- Pattern discovery may overstate weak signals.
- Statistical results may be misinterpreted.
- Forecasts may be treated as facts rather than estimates.
- Agent explanations may overreach without strong guardrails.


## Delivery Risks

- No Git repository is initialized yet.
- No GitHub remote is connected yet.
- Jira MCP is not available in the current session.
- The product scope is broad and needs careful sprint boundaries.
- Agent roles and skills are still early drafts.


## Mitigations

- Keep Sprint 0 conversational and iterative.
- Use markdown tracking until Jira is available.
- Initialize or connect Git before implementation.
- Add human approval gates.
- Require evidence for patterns and agent answers.
- Separate confidence, importance, and caveats.
- Build deterministic engines before LLM integration.
