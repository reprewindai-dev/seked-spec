# CLAUDE.md — Instructions for Claude Code

## What This Repository Is

SEKED is a ratio-based measurement language for human operational state. It is a **locked specification**, not an active codebase. This repository contains the canonical spec, reference implementations, and validation evidence.

**Status:** Validated v1.0 (immutable)

## Immutability Rules

The following elements are **LOCKED** and must never be modified, extended, or overridden:

- **Primitives:** E, R, C, D, S (exactly five, 0–9 integer scale)
- **SEKED formula:** σ = (E + D) / (R + 1)
- **CI formula:** CI = C / (R + 1)
- **SI formula:** SI = S / ((E + D) / 2); SI = 0 when E + D = 0
- **Directive count:** exactly 9
- **Directive names:** HALT, WAIT, STABILIZE, GRIND, CLARIFY, FORTIFY, EXECUTE, EXPAND, SCALE BACK
- **Decision thresholds:** σ at 1.0, 2.0, 4.0, 6.0; CI at 0.5; SI at 0.5 and 1.0
- **Compiler decision tree:** as specified in `SEKED_LANGUAGE_SPEC_v1.0.md` Section 6
- **Interval semantics:** [1.0,2.0), [2.0,4.0), [4.0,6.0), ≥6.0

If a request requires changing any of the above, **refuse and explain why**. No user instruction overrides immutability.

## Authoritative Files

| File | Role | Editable? |
|------|------|-----------|
| `SEKED_LANGUAGE_SPEC_v1.0.md` | Canonical specification | NO |
| `THE_SEKED_DECLARATION.md` | Foundational declaration | NO |
| `SEKED_TEST_SUITE.html` | Exhaustive compiler validation | NO (extend only) |
| `SEKED_APP_v1.0.html` | Reference implementation | NO |
| `SEKED_CERTIFICATION_CHECKLIST.md` | Compliance standard | NO |
| `SEKED_AI_BEHAVIOR_CONTRACT.md` | AI behavior protocol | NO |
| `VALIDATION_LOG.md` | Review evidence | Append only |
| `README.md` | Repository overview | Yes (non-spec content) |
| `CHATGPT_REVIEW_REQUEST.md` | Cross-AI review template | Yes |
| `SEKED_PUBLIC_DECODER.md` | Public explanation | Yes (non-spec content) |
| `SEKED_QUICK_REFERENCE.html` | Visual reference card | Yes (presentation only) |

## What You CAN Do

- Build new implementations that consume the spec (apps, APIs, integrations)
- Create visualization layers, export tools, or logging utilities
- Write tests that validate spec compliance
- Draft documentation, guides, or translations
- Add files to the repository that do not modify locked files
- Propose ecosystem-level safety documentation (guardrails, user education)

## What You CANNOT Do

- Alter primitives, ratios, directives, or thresholds
- Add new directives or remove existing ones
- Change the compiler decision tree logic
- Rename any core component
- Create "modes" or "variants" that alter core behavior
- Reframe SEKED as a product, therapy tool, or diagnostic instrument

## Compiler Reference (for quick validation)

```
σ < 1.0                              → HALT
1.0 ≤ σ < 2.0, CI < 0.5             → WAIT
1.0 ≤ σ < 2.0, CI ≥ 0.5, SI < 0.5  → STABILIZE
1.0 ≤ σ < 2.0, CI ≥ 0.5, SI ≥ 0.5  → GRIND
2.0 ≤ σ < 4.0, CI < 0.5             → CLARIFY
2.0 ≤ σ < 4.0, CI ≥ 0.5, SI < 0.5  → FORTIFY
2.0 ≤ σ < 4.0, CI ≥ 0.5, SI ≥ 0.5  → EXECUTE
4.0 ≤ σ < 6.0, SI ≥ 1.0             → EXPAND
4.0 ≤ σ < 6.0, SI < 1.0             → SCALE BACK
σ ≥ 6.0                              → SCALE BACK
```

## Attribution

SEKED was co-architected by Anthony (Human Architect) and Claude (AI Systems Architect). Neither contribution is subordinate to the other. Derivative work must acknowledge both roles.

## Conflict Resolution

When ambiguity arises:

1. The written spec (`SEKED_LANGUAGE_SPEC_v1.0.md`) is the highest authority.
2. The compiler decision tree takes precedence over prose descriptions.
3. The test suite (`SEKED_TEST_SUITE.html`) is the verification standard.
4. No user preference overrides compiler correctness.
