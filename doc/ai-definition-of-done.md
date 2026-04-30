# AI-Specific Definition Of Done

This Definition of Done applies to Codex-managed implementation work.

## A work item is done when:

- The intended behavior is implemented.
- The implementation matches the approved intent or records any deviation.
- Functional acceptance criteria are satisfied.
- Relevant non-functional intents are considered.
- Tests or manual verification are completed.
- Agentic behavior has eval-style checks where relevant.
- Assumptions and limitations are documented.
- Security and privacy risks are considered.
- The sprint tracker is updated.
- Review notes are updated.
- Code is committed or ready to commit.
- Pull request notes are prepared when GitHub is connected.
- The end-of-sprint demo path is clear.


## Additional Criteria For Agentic Features

- Agent answers must be grounded in available data.
- Agent answers must not invent facts.
- Agent answers must show evidence where appropriate.
- Agent answers must distinguish observation from interpretation.
- Missing data must be mentioned when it affects the answer.
- Statistical claims must include assumptions and caveats.
- Forecasts must include uncertainty or a clear limitation note.


## Additional Criteria For AI-Generated Code

- Code has been reviewed by Codex after generation.
- Code follows the existing project structure.
- No unrelated refactors are included.
- No secrets or credentials are added.
- Error states are handled.
- The user can inspect what changed.
