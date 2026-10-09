# Larp Test Results

## Method

These are instruction-level forward checks for the current skill. Each case evaluates whether the documented workflow produces useful professional framing while preserving evidence fidelity. They do not measure model quality across all possible prompts.

## RED: Risks Identified

| Risk | Failure pattern | Guardrail added |
|---|---|---|
| Inflated ownership | Team contribution becomes sole ownership or leadership | Scope Accuracy verification and contribution verbs |
| Invented impact | Technical task gains an unsupported metric or business result | Evidence Fidelity verification and explicit metric prohibition |
| False expertise | Tool exposure becomes deep proficiency | Evidence-to-Claim Map for tools and context |
| Unsafe thin-input rewrite | Vague source becomes an authoritative claim | Cautious-draft output with focused question |

## GREEN: Scenario Checks

| ID | Scenario | Expected invariant | Result |
|---|---|---|---|
| LRP-01 | Sensor board CV bullet | Names design and testing, no performance claim | Pass |
| LRP-02 | Team controller testing | Preserves collaboration and avoids leadership | Pass |
| LRP-03 | PCB portfolio text | Distinguishes manufacturing handoff from manufactured hardware | Pass |
| LRP-04 | MATLAB analysis | States applied analysis without inflating domain expertise | Pass |
| LRP-05 | Vague PLC experience | Produces cautious wording and a targeted question | Pass |
| LRP-06 | Autonomous vehicle meeting attendance | Rejects unsupported leadership claim | Pass |
| LRP-07 | Turkish internship wording | Preserves Turkish and uses professional passive voice | Pass |

The concrete inputs and outputs for these checks are in [examples.md](examples.md).

## REFACTOR: Changes Made After Review

| Observation | Change |
|---|---|
| The initial skill had a clear safety boundary but no artifact-selection aid | Added the Artifact Router |
| The initial workflow did not make evidence categories visible | Added the Evidence-to-Claim Map |
| Thin evidence needed a consistent response | Added cautious-draft and focused-question outputs |
| Examples and verification detail would make the entrypoint too long | Moved full cases and results to companion Markdown files |

## Validation

### Latest Validation Run

Run date: 2026-10-09

- Structural validation: Pass. `quick_validate.py` accepted the skill directory.
- Package validation: Pass. All five required package files are present.
- Documentation validation: Pass. Seven examples, seven scenario checks, and the README links were checked.
- Scope limitation: these checks validate the written skill design, not independent execution by another model.
