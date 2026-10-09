# Larp Validation Notes

## Method

This file records manual reviews of the skill design. It is not an executable test suite and does not report an independent model run. Each review checks whether the written workflow preserves evidence fidelity in a fictional example.

## RED: Risks Identified

| Risk | Failure pattern | Guardrail added |
|---|---|---|
| Inflated ownership | Team contribution becomes sole ownership or leadership | Scope Accuracy verification and contribution verbs |
| Invented impact | Technical task gains an unsupported metric or business result | Evidence Fidelity verification and explicit metric prohibition |
| False expertise | Tool exposure becomes deep proficiency | Evidence-to-Claim Map for tools and context |
| Unsafe thin-input rewrite | Vague source becomes an authoritative claim | Cautious-draft output with focused question |

## Manual Scenario Reviews

| ID | Scenario | Review criterion |
|---|---|---|
| LRP-01 | Volunteer shift tracker | Names the tracker and updates without claiming program ownership or time savings |
| LRP-02 | Online booking-form testing | Preserves collaboration and does not claim the form was built or fixed |
| LRP-03 | New-staff guide | Distinguishes documentation from ownership of the underlying system |
| LRP-04 | Class-project survey data | Avoids implying formal research findings or advanced analytics |
| LRP-05 | Customer-facing store work | Avoids sales, satisfaction, or supervisory claims |
| LRP-06 | Canva exposure | Uses cautious wording and asks one question before extending scope |
| LRP-07 | Community-event meetings | Rejects unsupported planning ownership and leadership |
| LRP-08 | Workplace safety training | Avoids certification and compliance-authority claims |

The fictional inputs, outputs, and rationale for these reviews are in [examples.md](examples.md).

## REFACTOR: Changes Made After Review

| Observation | Change |
|---|---|
| The initial skill had a clear safety boundary but no artifact-selection aid | Added the Artifact Router |
| The initial workflow did not make evidence categories visible | Added the Evidence-to-Claim Map |
| Thin evidence needed a consistent response | Added cautious-draft and focused-question outputs |
| Examples and verification detail would make the entrypoint too long | Moved full cases and results to companion Markdown files |
| Earlier examples resembled the author's technical history | Replaced them with fictional, general-public scenarios |

## Validation

### What Has Been Checked

- The local workspace copy passed `quick_validate.py` structural validation.
- The documented scenarios were manually reviewed against the written constraints.

### What Has Not Been Implemented

- No executable test harness is committed in this repository.
- No test fixtures, CI workflow, or independent model execution log is committed.
- The external `quick_validate.py` helper is not bundled in this repository.
