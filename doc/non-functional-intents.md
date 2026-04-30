# Non-Functional Intents

## N1: Explainability

The product must explain how it interpreted data, why it generated UI elements, why it detected patterns, and how statistical results should be understood.

Acceptance criteria:
- UI generation reasons are visible.
- Pattern evidence is inspectable.
- Statistical assumptions are shown.
- Agent separates observation from interpretation.


## N2: Trust And Grounding

Agent answers must be grounded in available data and computed facts.

Acceptance criteria:
- Agent does not invent dataset values.
- Agent mentions missing data when relevant.
- Agent cites evidence values for patterns.
- Forecasts include uncertainty and caveats.


## N3: Human Control

The user must be able to correct AI or heuristic interpretations.

Acceptance criteria:
- User can correct schema roles.
- User can correct semantic tags.
- User can review assumptions.
- User can approve sprint/demo outcomes.


## N3.5: Expert Knowledge Provenance

Expert-provided knowledge must be traceable and distinguishable from dataset-derived facts.

Acceptance criteria:
- Expert claims include provenance.
- Expert claims include validation status.
- Agent identifies when it is using expert knowledge.
- Unverified expert claims are not treated as facts.
- Evidence attachments remain linked to the claims they support.


## N4: Testability

Each sprint must produce something testable.

Acceptance criteria:
- Unit tests exist for deterministic engines where practical.
- Manual demo checklist exists for each sprint.
- Agentic features have eval-style checks before LLM integration is considered complete.


## N5: Maintainability

The codebase should remain modular and understandable.

Acceptance criteria:
- Data parsing, schema detection, ontology, analysis, statistics, agent, charts, and reports are separate modules.
- Shared types are explicit.
- Large features are built in small reviewable steps.


## N6: Performance

The MVP should work well for small to medium local datasets.

Acceptance criteria:
- App remains responsive with MVP fixture datasets.
- Large datasets show warnings or limits.
- Heavy processing can later move server-side.


## N7: Privacy And Data Safety

Uploaded datasets are user-provided input and must be handled carefully.

Acceptance criteria:
- Uploaded data is not executed.
- Invalid files show safe errors.
- LLM integration should send summaries and computed facts where possible, not full datasets by default.


## N8: Cost Control

LLM usage should be controlled.

Acceptance criteria:
- Rule-based fallback exists.
- Structured summaries are preferred over sending raw data.
- API failures produce useful fallback messages.
- Token/API usage should be reviewed during LLM integration.


## N9: Accessibility And Usability

The app should be understandable and usable.

Acceptance criteria:
- Controls have clear labels.
- Empty states are useful.
- Chart interactions are understandable.
- Text does not overlap or overflow in core flows.


## N10: Auditability

Planning, assumptions, implementation progress, and AI decisions should be traceable.

Acceptance criteria:
- Sprint progress is tracked.
- Review notes are tracked.
- AI-DLC decisions are logged.
- Pull requests include tests and known limitations.
