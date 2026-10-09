# Larp

Strengthen real professional experience without exaggerating it.

Larp is an agent skill for CV bullets, portfolios, cover letters, and professional profiles. It turns accurate but understated material into precise technical writing while treating evidence fidelity as a hard constraint.

## What This Is

Larp helps surface the value already present in genuine work:

- Technical contribution rather than a bare task list
- System context, constraints, and validation work
- Accurate collaboration and ownership boundaries
- Transferable capability matched to the requested artifact

It does not create experience, invent metrics, or turn participation into leadership.

## Pipeline

```text
Evidence → Scope check → Artifact route → Rewrite → Verification → Delivery
```

1. Extract the facts, tools, actions, constraints, and supported outcomes.
2. Check ownership, collaboration, and uncertainty.
3. Select the requested professional artifact.
4. Rewrite around the strongest truthful technical angle.
5. Verify evidence fidelity, scope accuracy, clarity, and usefulness.

## How It Differs from a Generic Resume Booster

| Generic approach | Larp |
|---|---|
| Optimizes for impressive language | Optimizes for a strong, defensible claim |
| May add metrics or impact by default | Uses only supported results and metrics |
| Can flatten team contributions into ownership | Preserves collaboration and role scope |
| Treats thin input as a complete story | Produces a cautious draft and focused question |

## Installation

For a repository-scoped Codex skill, keep this directory intact:

```text
.agents/
└── skills/
    └── larp/
        ├── SKILL.md
        ├── README.md
        ├── examples.md
        ├── test-results.md
        └── agents/
            └── openai.yaml
```

Commit the entire `larp` directory. `SKILL.md` is required. The other Markdown files document use cases and validation, while `agents/openai.yaml` retains the user-facing metadata.

## Usage

Invoke the skill explicitly:

```text
Use $larp to strengthen this CV bullet without adding unsupported claims.
```

Or provide material naturally:

```text
Larp this portfolio description. Keep it technically specific, but do not claim that I led the project.
```

## Examples and Tests

- [examples.md](examples.md) contains seven evidence-backed transformations.
- [test-results.md](test-results.md) records the guardrail scenarios used to review the skill design.

## Security and Scope

This skill contains Markdown instructions and YAML metadata only. It has no scripts, network calls, executable payloads, or data collection behavior. The user remains the source of truth for professional claims.

## License

No license has been selected for this skill yet.
