---
name: larp
description: |
  Strengthen real CV, portfolio, cover-letter, and professional-profile material
  without exaggeration. Use when the user asks to larp, sharpen, position, or make
  genuine experience sound more technically compelling.
---

# Larp

Turn genuine experience into clear, technical, and consequential professional writing.
Preserve the truth. Strengthen the framing. Never invent the work.

## When to Use

```text
User asks to strengthen professional material
  ├─ Evidence is specific enough → Rewrite with a claim check when needed
  └─ Evidence is too thin → Draft cautiously and ask focused questions
```

- User asks to larp, sharpen, position, or strengthen professional material.
- A CV bullet, portfolio page, cover letter, LinkedIn profile, or project summary is accurate but undersells technical work.
- A user wants help expressing a real contribution without crossing into exaggeration.

## When NOT to Use

- The user asks to invent experience, results, credentials, seniority, or ownership.
- The requested text is unrelated to professional positioning.
- The user wants a verbatim transcription or explicitly does not want wording changed.
- The user needs factual research, reference checking, or a recommendation rather than a rewrite.

## Quick Reference

### Evidence-to-Claim Map

| Evidence available | Strongest defensible framing | Do not imply |
|---|---|---|
| A completed technical task | Designed, implemented, integrated, or verified the stated task | Scope beyond the described work |
| Collaborative contribution | Contributed to, supported, or worked within a team on the stated area | Sole ownership or leadership |
| Bench or simulation testing | Validated, tested, analyzed, or investigated the stated behavior | Production qualification or final performance |
| A tool or technology used | Applied, used, or worked with it in the stated context | Deep expertise, certification, or ownership |
| A stated result | Report the result with its condition or context | Generalized business impact or unverified metrics |

### Artifact Router

| Artifact | Prioritize | Format |
|---|---|---|
| CV | Contribution, technical context, supported purpose or result | Concise bullet |
| Portfolio | Problem, scope, decisions, contribution, validation, status | Structured narrative |
| Cover letter | Transferable capability matched to the role | Role-specific paragraph |
| Professional profile | Technical identity and evidence-backed focus areas | Short summary |

### Claim-Risk Check

| Signal | Action |
|---|---|
| The wording adds a named role, metric, or outcome | Remove it unless the user provided it |
| The wording turns team work into "led" or "owned" | Use a contribution verb or ask for confirmation |
| The input says "tested" | State what was tested and avoid implying certification |
| The source is vague | Use narrow wording and ask one focused question |

## Implementation

### Step 0: Extract Evidence

Separate what is known from what is only plausible.

1. Identify the system, domain, and technical context.
2. Identify the user's actual actions, decisions, tools, and validation work.
3. Mark ownership, collaboration, outcomes, and metrics only when directly supported.
4. Keep uncertainties visible. Do not convert an inference into a claim.

### Step 1: Select the Strongest Truthful Angle

Favor details that show engineering judgment:

- Design choices and constraints
- Integration between components or disciplines
- Debugging, testing, analysis, and verification
- Tradeoffs, interfaces, and technical scope

Turn a task list into a contribution statement where the evidence allows it:

```text
contribution → technical context → method or decision → supported purpose or result
```

### Step 2: Route and Rewrite

Use the Artifact Router. Match the requested language, grammatical person, level of formality, and length.

- Preserve collaboration accurately.
- Prefer precise verbs that fit the evidence, such as contributed, designed, integrated, implemented, verified, analyzed, or supported.
- Replace generic verbs only when the source identifies a more specific action.
- Do not add a result merely because a strong bullet appears to need one.

### Step 3: Verify

Before delivery, run four checks:

| Test | Pass criterion | Fail action |
|---|---|---|
| Evidence fidelity | Every substantive claim appears in the supplied evidence | Remove or narrow the claim |
| Scope accuracy | Ownership and collaboration match the source | Use a weaker role verb or ask |
| Technical clarity | The wording makes the relevant technical context visible | Add supported context |
| Professional usefulness | The result fits the requested artifact and length | Reformat or tighten |

### Step 4: Deliver

If the evidence is clear, provide the rewritten copy first. Add a short explanation only if the user asks for one.

If evidence is thin, provide a cautious draft and one or two questions that could unlock stronger wording.

For high-stakes or ambiguous material, append:

```text
Supported claims: [claims grounded in the source]
Questions to unlock stronger wording: [only essential questions]
Claims to avoid: [wording that would overstate the evidence]
```

See [examples.md](examples.md) for complete transformations and [test-results.md](test-results.md) for evaluated guardrail cases.

## Common Mistakes

| Mistake | Fix |
|---|---|
| Replacing a weak verb with a stronger but unsupported one | Recover the specific action from the evidence first |
| Treating tool exposure as expertise | State the tool and context, not an unsupported proficiency level |
| Making collaboration invisible | Name the contribution without claiming team-level ownership |
| Hiding uncertainty with polished language | Keep conditions, scope, and status explicit |
| Adding metrics for impact | Ask for a metric or state the supported qualitative outcome |

## Constraints

- Preserve facts, scope, and uncertainty.
- Never invent experience, ownership, results, credentials, seniority, or metrics.
- Match the input language unless the user requests another language.
- Match complexity to the artifact. A CV bullet should not become a portfolio paragraph.
- Ask only questions whose answers would materially improve accuracy or positioning.

## Output

**Clear evidence:**

```text
Rewritten copy: [final text]
```

**Thin or ambiguous evidence:**

```text
Cautious draft: [final text]

Question: [one focused fact needed for a stronger version]
```
