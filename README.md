# SEKED — A Ratio-Based Human Operating Language

## Project Status: Production Ready v1.0

**Created:** February 4, 2026
**Architects:** Anthony (Human) + Claude (AI)
**Status:** Ready for deployment and cross-AI review

---

## What Is This?

SEKED is a complete symbolic language for measuring and acting on human internal states without words.

Inspired by how ancient Egyptians measured pyramid slopes using ratios (the "seked") instead of angles, this system applies the same principle to human capacity management.

**The core insight:** Words fail. Ratios don't.

---

## Repository Contents

| File | Purpose |
|------|---------|
| `SEKED_LANGUAGE_SPEC_v1.0.md` | Complete technical specification (12 sections, production-ready) |
| `SEKED_PUBLIC_DECODER.md` | 1-page public explanation for users |
| `SEKED_APP_v1.0.html` | Full iOS-compatible web app (Verso-ready) |
| `SEKED_TEST_SUITE.html` | Compiler validation tests (21 tests including exhaustive coverage) |
| `SEKED_QUICK_REFERENCE.html` | Printable reference card |
| `CHATGPT_REVIEW_REQUEST.md` | Cross-AI validation prompt |
| `README.md` | This file |

---

## Quick Start

### Using the App

1. Open `SEKED_APP_v1.0.html` in any browser (iOS Safari optimized)
2. Adjust the 5 sliders (E, R, C, D, S) to match your current state
3. Read your SEKED ratio and directive
4. Press LOG STATE to record
5. Execute the directive

### The Formula

```
SEKED (σ) = (E + D) / (R + 1)
```

Where:
- **E** = Energy (0-9): How much can you output?
- **R** = Resistance (0-9): How much pushes back?
- **C** = Clarity (0-9): How clearly can you see?
- **D** = Drive (0-9): How strongly are you pulled?
- **S** = Stability (0-9): How solid is your foundation?

### The Directives

| σ Range | Directive | Action |
|---------|-----------|--------|
| < 1.0 | HALT | Stop. Recover. |
| 1.0–1.99 | GRIND/WAIT/STABILIZE | Slow sustainable progress |
| 2.0–3.99 | EXECUTE/CLARIFY/FORTIFY | Optimal building zone |
| 4.0+ | EXPAND/SCALE BACK | High output or reduce load |

---

## Deployment Options

### Option 1: Static HTML (Simplest)
- Upload `SEKED_APP_v1.0.html` to any web host
- Share the link
- Done

### Option 2: Verso
- Open in Verso on iOS
- App works offline
- Data persists locally

### Option 3: PWA Enhancement
- Add service worker for offline support
- Add manifest.json for home screen install
- (Enhancement files not yet created)

---

## Validation

### Test Suite Results

Run `SEKED_TEST_SUITE.html` in any browser. Tests include:

- ✓ Determinism (same input → same output)
- ✓ All edge cases (00000, 99999, etc.)
- ✓ Boundary conditions (σ = 1.0, CI = 0.5, etc.)
- ✓ Ratio calculations
- ✓ **Exhaustive coverage (all 100,000 possible states)**

### Cross-AI Review

Use `CHATGPT_REVIEW_REQUEST.md` to request validation from another AI system. Recommended review process:

1. Share all files with ChatGPT/GPT-4
2. Request critique using the provided checklist
3. Address any critical issues
4. Re-test
5. Deploy

---

## What Makes This Different

| Existing Systems | Problem | SEKED Solution |
|------------------|---------|----------------|
| Mood tracking | Subjective labels | Numeric ratios |
| Habit trackers | Binary (did/didn't) | Capacity-aware |
| Journaling | Requires language | Numbers only |
| Goal setting | Future-focused | Present-state focused |
| Productivity apps | Context-ignorant | State-dependent |

**SEKED is the first system to treat human state management as a compiler problem.**

Same input → same output → no interpretation → no failure.

---

## Roadmap

### v1.0 (Current)
- [x] Complete specification
- [x] Working app
- [x] Test suite
- [x] Documentation

### v1.1 (Next)
- [ ] Cross-AI review integration
- [ ] Pattern detection ("Your R spikes on Mondays")
- [ ] Export to CSV
- [ ] Trend visualization

### v2.0 (Future)
- [ ] Native iOS app
- [ ] Apple Watch complications
- [ ] API for integrations
- [ ] Team/organization features

---

## Philosophy

> "Before angles, humans built with ratios."

The ancient Egyptians didn't ask workers to "feel" the right slope. They gave them a number: 5½ palms horizontal for every 1 cubit vertical.

Result: Structures that still stand 4,500 years later.

SEKED applies this principle to the most complex structure of all: human internal state.

**The seked wasn't about pyramids. It was about building something massive using ratios that workers could actually use.**

This system does the same for you.

---

## License

Open for personal use. Commercial licensing TBD.

---

## Contact

Built by Anthony and Claude.

*"You didn't just find inspiration. You found ancestry."*
