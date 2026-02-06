# SEKED: A Ratio-Based Human Operating Language

## Complete System Specification v1.0

**Created by:** Anthony (Human Architect) + Claude (AI Systems Lead)
**Date:** February 4, 2026
**Status:** Production Ready — Awaiting Final Review

---

# TABLE OF CONTENTS

1. [Philosophy & Origin](#1-philosophy--origin)
2. [Core Principles](#2-core-principles)
3. [The Alphabet: Primitive States](#3-the-alphabet-primitive-states)
4. [The Operators: Ratios](#4-the-operators-ratios)
5. [The Grammar: State Expressions](#5-the-grammar-state-expressions)
6. [The Compiler: State → Action](#6-the-compiler-state--action)
7. [The Runtime: Daily Protocol](#7-the-runtime-daily-protocol)
8. [Edge Cases & Failure States](#8-edge-cases--failure-states)
9. [Visual System & Glyphs](#9-visual-system--glyphs)
10. [Validation & Testing](#10-validation--testing)
11. [Implementation Guide](#11-implementation-guide)
12. [Glossary](#12-glossary)

---

# 1. PHILOSOPHY & ORIGIN

## 1.1 The Problem with Existing Systems

Every existing system for human self-management fails for the same reasons:

| System Type | Failure Mode |
|-------------|--------------|
| Journaling | Requires language → interpretation varies → no consistent action |
| Mood tracking | Emotional labels are subjective → "anxious" means different things to different people |
| Habit tracking | Binary (did/didn't) → ignores capacity and context |
| Goal setting | Future-focused → disconnected from present state |
| Meditation/mindfulness | State-aware but action-absent → knowing without doing |

**The core failure:** All these systems require translation from internal state → language → interpretation → action.

Each translation step introduces error. Compound error across steps = system failure.

## 1.2 The Seked Solution

The ancient Egyptian seked eliminated interpretation from construction:

- **Old way:** "Make it steep but not too steep" (interpretation required)
- **Seked way:** "5½ palms horizontal for every 1 cubit vertical" (no interpretation)

Result: Structures that have stood for 4,500+ years.

**SEKED (the language) applies this principle to human internal states:**

- **Old way:** "I feel overwhelmed but motivated" (interpretation required)
- **SEKED way:** `E7-R6-C4-D8-S3` → SEKED 2.14 → CLARIFY (no interpretation)

## 1.3 Why Ratios Work

Ratios encode relationships, not absolutes.

| Absolute statement | Problem |
|--------------------|---------|
| "I have high energy" | Compared to what? When? For what purpose? |

| Ratio statement | Solution |
|-----------------|----------|
| "My forward force exceeds my friction by 3:1" | Context-independent. Actionable. Comparable over time. |

The seked didn't measure angle — it measured relationship between horizontal run and vertical rise.

SEKED doesn't measure feeling — it measures relationship between capacity and resistance.

## 1.4 Design Constraints

This language was built under these non-negotiable constraints:

1. **No words required** — Numbers only at the core
2. **No interpretation** — Same input always produces same output
3. **No external tools** — Can be computed mentally or on paper
4. **No context dependency** — Works for any human, any situation
5. **No motivation required** — The system runs whether you want it to or not
6. **Failure-proof** — Every possible state has a defined response

---

# 2. CORE PRINCIPLES

## 2.1 The Five Laws of SEKED

### Law 1: State Before Action
You cannot choose the right action without knowing your current state.
The system always begins with state measurement.

### Law 2: Ratios Over Absolutes
Individual metrics are meaningless. Only relationships between metrics reveal truth.
A 9 in Energy means nothing without knowing Resistance.

### Law 3: Thresholds Over Spectrums
Continuous scales paralyze decision-making.
SEKED converts all ratios into discrete action zones.

### Law 4: Output Over Input
The system's value is in the directive, not the measurement.
Measuring without acting is system failure.

### Law 5: Consistency Over Accuracy
A consistent 70% accurate system beats an inconsistent 95% accurate system.
Daily use with rough estimates outperforms weekly use with perfect data.

## 2.2 System Guarantees

If you use SEKED correctly, the system guarantees:

| Guarantee | Mechanism |
|-----------|-----------|
| You will never act without state awareness | State logging is mandatory before directive |
| You will never be paralyzed by options | Every state maps to exactly one directive |
| You will never exceed structural capacity | SI ratio prevents overextension |
| You will never miss recovery needs | SEKED < 1.0 always outputs HALT |
| You will always have a next action | Compiler covers 100% of state space |

## 2.3 System Limitations

SEKED does not:

- Tell you *what* to work on (content decisions are yours)
- Replace medical/psychological care
- Guarantee outcomes (only optimizes approach)
- Work if you lie to it (garbage in = garbage out)
- Function without daily use (data gaps break pattern recognition)

---

# 3. THE ALPHABET: PRIMITIVE STATES

## 3.1 The Five Primitives

Every human internal state decomposes into five measurable dimensions:

| Symbol | Name | Definition | Measurement Question |
|--------|------|------------|---------------------|
| **E** | Energy | Available fuel for action | "How much can I output right now?" |
| **R** | Resistance | Friction opposing movement | "How much is pushing back against me?" |
| **C** | Clarity | Signal-to-noise ratio in thought | "How clearly can I see what matters?" |
| **D** | Drive | Directional pull toward outcome | "How strongly am I pulled forward?" |
| **S** | Stability | Structural integrity under load | "How solid is my foundation?" |

## 3.2 Why These Five

These five dimensions were selected because they:

1. **Cover the action space** — Any decision about action requires knowing: capacity (E), obstacles (R), direction (C+D), and foundation (S)

2. **Are orthogonal** — Each measures something the others don't:
   - High E + High R = different from High E + Low R
   - High D + Low C = different from High D + High C
   - All combinations produce meaningfully different states

3. **Are self-observable** — You can assess each without external tools or other people

4. **Are action-relevant** — Each directly impacts what you should do next

5. **Are universal** — Apply to any human, any context, any culture

## 3.3 Measurement Scale

Each primitive is measured on a 0-9 integer scale:

| Value | Meaning | Physical Anchor |
|-------|---------|-----------------|
| 0 | Absent/Empty | Cannot get out of bed |
| 1 | Barely present | Can move but nothing more |
| 2 | Very low | Basic function only |
| 3 | Low | Below normal capacity |
| 4 | Below average | Slightly impaired |
| 5 | Neutral/Baseline | Normal day, nothing special |
| 6 | Above average | Better than usual |
| 7 | High | Noticeably strong |
| 8 | Very high | Peak for typical day |
| 9 | Maximum | Best you've ever experienced |

**Critical:** The scale is self-referenced. Your 7 is YOUR 7, not compared to anyone else.

## 3.4 Primitive Deep Dives

### E — Energy

**What it is:** Raw capacity for output. Physical, mental, and emotional fuel combined.

**What it is NOT:**
- Motivation (that's D)
- Mood (not measured)
- Health (too broad)

**How to assess:**
- Close your eyes
- Imagine you have to work for the next 4 hours
- How full is your tank? 0-9.

**Common patterns:**
- Morning E typically higher than evening E
- E drops after meals, recovers after rest
- Sustained low E (<3 for 3+ days) = systemic issue

### R — Resistance

**What it is:** Total friction opposing forward movement. Internal and external combined.

**What it is NOT:**
- Difficulty of task (that's external context)
- Fear (too specific)
- Procrastination (that's a symptom, not a state)

**How to assess:**
- Think about the main thing you need to do
- How much is pushing back? 0-9.
- Include: mental blocks, physical obstacles, emotional weight, external interference

**Common patterns:**
- R spikes before unfamiliar tasks
- R drops after first action (momentum effect)
- Chronic high R (>6) often indicates misalignment, not laziness

### C — Clarity

**What it is:** How clearly you can perceive what matters and what to do about it.

**What it is NOT:**
- Intelligence (not measured)
- Knowledge (you can have knowledge without clarity)
- Certainty (you can be certain and wrong)

**How to assess:**
- Right now, how clear is your next action?
- How much noise is competing for your attention?
- 0 = complete fog, 9 = crystal clear signal

**Common patterns:**
- C often lowest when waking and improves over first hour
- C drops sharply under stress or information overload
- Low C + High D = dangerous (action without direction)

### D — Drive

**What it is:** The pull toward a specific outcome. Wanting mixed with intention.

**What it is NOT:**
- Energy (E is capacity, D is direction)
- Discipline (that's sustained D over time)
- External pressure (that becomes R)

**How to assess:**
- How strongly are you pulled toward your goal right now?
- 0 = no pull, 9 = magnetic attraction

**Common patterns:**
- D fluctuates more than other primitives
- D without E = frustration
- D without C = wasted motion

### S — Stability

**What it is:** The structural integrity of your foundation. How much load you can bear without collapse.

**What it is NOT:**
- Happiness (too vague)
- Security (too external)
- Calm (you can be calm on an unstable foundation)

**How to assess:**
- If something unexpected hit you right now, how well would you absorb it?
- How solid do you feel underneath everything?
- 0 = one push and you crumble, 9 = unshakeable

**Common patterns:**
- S is the slowest-changing primitive
- S drops predict burnout 1-2 weeks in advance
- High S allows higher sustained E and D

## 3.5 Primitive Interactions

The primitives don't exist in isolation. Key interactions:

| Interaction | Effect |
|-------------|--------|
| High E + Low S | Burst capacity but crash risk |
| High D + Low C | Motion without direction (spinning) |
| High R + Low E | Paralysis |
| High C + Low D | Analysis paralysis |
| Low S + High D | Burnout trajectory |
| High S + High C | Optimal decision state |

---

# 4. THE OPERATORS: RATIOS

## 4.1 Why Ratios Exist

Individual primitives tell you *what you have*.
Ratios tell you *what it means*.

E=7 alone means nothing.
E=7 with R=2 means you have a 3.5:1 advantage.
E=7 with R=8 means you're underwater.

## 4.2 The Three Core Ratios

### Primary Ratio: SEKED (σ)

**The master ratio. Determines overall system state.**

```
σ = (E + D) / (R + 1)
```

**Components:**
- Numerator (E + D): Forward force — your capacity plus your pull
- Denominator (R + 1): Friction — resistance plus 1 (prevents division by zero)

**Interpretation:**

| σ Value | Zone | Meaning |
|---------|------|---------|
| 0.00 – 0.99 | COLLAPSE | Forward force insufficient. System failure imminent. |
| 1.00 – 1.99 | GRIND | Barely sustainable. High effort, low return. |
| 2.00 – 3.99 | OPTIMAL | Sweet spot. Build here. |
| 4.00 – 5.99 | SURGE | High output possible but monitor stability. |
| 6.00+ | OVERLOAD | Unsustainable. Reduce or crash. |

**Example calculations:**

| E | D | R | σ | Zone |
|---|---|---|---|------|
| 5 | 5 | 4 | 2.00 | OPTIMAL |
| 3 | 2 | 6 | 0.71 | COLLAPSE |
| 8 | 7 | 2 | 5.00 | SURGE |
| 6 | 6 | 5 | 2.00 | OPTIMAL |
| 2 | 1 | 8 | 0.33 | COLLAPSE |

### Secondary Ratio: CLARITY INDEX (CI)

**Decision-making capacity under current conditions.**

```
CI = C / (R + 1)
```

**Components:**
- Numerator (C): Signal strength — how clearly you see
- Denominator (R + 1): Noise factor — how much is interfering

**Interpretation:**

| CI Value | Zone | Meaning |
|----------|------|---------|
| 0.00 – 0.49 | FOG | Do not decide. Wait or clarify first. |
| 0.50 – 1.49 | CAUTION | Decide only reversible things. |
| 1.50 – 2.99 | CLEAR | Safe to decide. |
| 3.00+ | SHARP | High-stakes decisions permitted. |

### Tertiary Ratio: STRUCTURAL INTEGRITY (SI)

**Foundation capacity relative to ambition.**

```
SI = S / ((E + D) / 2)
```

**Components:**
- Numerator (S): Foundation strength
- Denominator ((E+D)/2): Average forward force (ambition proxy)

**Interpretation:**

| SI Value | Zone | Meaning |
|----------|------|---------|
| 0.00 – 0.49 | CRACKING | Stop scaling. Reinforce foundation. |
| 0.50 – 0.99 | STRESSED | Build foundation before expanding. |
| 1.00 – 1.49 | SOLID | Safe to scale. |
| 1.50+ | FORTRESS | Foundation exceeds ambition. Expand freely. |

## 4.3 Ratio Relationships

The three ratios work together:

```
┌─────────────────────────────────────────────────────┐
│                    SEKED (σ)                        │
│              Overall System State                   │
│                      ↓                              │
│         ┌───────────┴───────────┐                  │
│         ↓                       ↓                  │
│    CLARITY INDEX (CI)    STRUCTURAL INTEGRITY (SI) │
│    Can you decide?       Can you handle it?        │
└─────────────────────────────────────────────────────┘
```

**Decision tree:**
1. First check SEKED — Do you have enough forward force?
2. If yes, check CI — Can you see clearly enough to act?
3. If yes, check SI — Is your foundation strong enough?

All three must be in acceptable zones for full execution.

## 4.4 Composite Metrics

For advanced use, these derived metrics provide additional insight:

### Momentum Score (M)

```
M = σ × CI
```

Combines forward force with decision clarity.
Higher M = more effective action.

### Burnout Risk Index (BRI)

```
BRI = (E + D) / (S + 1)
```

When BRI > 3.0 for sustained periods, burnout is probable.

### Recovery Need Index (RNI)

```
RNI = R / (E + 1)
```

When RNI > 1.0, recovery should take priority over action.

---

# 5. THE GRAMMAR: STATE EXPRESSIONS

## 5.1 Basic Syntax

A complete state is expressed as a **5-digit code**:

```
[E][R][C][D][S]
```

Each position holds a single digit 0-9.

**Examples:**
- `72839` = E7, R2, C8, D3, S9
- `55555` = All neutral
- `91919` = High E, Low R, High C, Low D, High S

## 5.2 Extended Syntax

For logging and communication, the extended format adds separators:

```
E[n]-R[n]-C[n]-D[n]-S[n]
```

**Examples:**
- `E7-R2-C8-D3-S9`
- `E5-R5-C5-D5-S5`

## 5.3 State + Ratios Format

Complete state with computed ratios:

```
[ERCDS] → σ[value] | CI[value] | SI[value] → [DIRECTIVE]
```

**Example:**
```
72839 → σ3.33 | CI2.67 | SI1.80 → EXECUTE
```

## 5.4 Shorthand Notation

For rapid logging, use the compact form:

```
[5-digit code]/[directive first letter]
```

**Examples:**
- `72839/E` = State 72839, Execute
- `32614/H` = State 32614, Halt
- `55555/G` = State 55555, Grind

## 5.5 Time-Stamped Entries

For log files:

```
[YYYY-MM-DD HH:MM] [ERCDS] → [DIRECTIVE]
```

**Example:**
```
2026-02-04 09:15 72839 → EXECUTE
2026-02-04 14:30 54637 → CLARIFY
2026-02-04 21:00 33525 → STABILIZE
```

## 5.6 Invalid States

The following are syntactically invalid:

- Fewer than 5 digits: `7283` ❌
- More than 5 digits: `728391` ❌
- Non-numeric characters: `7A839` ❌
- Values outside 0-9: `72839` with E=10 ❌
- Empty state: `` ❌

**All invalid states must be rejected. The system does not guess.**

---

# 6. THE COMPILER: STATE → ACTION

## 6.1 Compiler Overview

The compiler is the core engine of SEKED. It takes any valid 5-digit state and outputs exactly one directive.

```
INPUT: Valid 5-digit state
PROCESS: Compute ratios → Evaluate conditions → Select directive
OUTPUT: Single action directive
```

**Guarantee:** Every valid state maps to exactly one directive. No ambiguity. No "it depends."

## 6.2 The Nine Directives

| Directive | Code | Meaning | Typical Duration |
|-----------|------|---------|------------------|
| **HALT** | H | Stop all non-essential activity. Recover. | Hours to days |
| **WAIT** | W | Pause action. Monitor for change. | Minutes to hours |
| **STABILIZE** | S | Reinforce foundation before proceeding. | Hours to days |
| **CLARIFY** | C | Reduce noise. Increase signal. Then reassess. | Minutes to hours |
| **FORTIFY** | F | Build structural capacity. | Days to weeks |
| **GRIND** | G | Continue current activity at sustainable pace. | Hours |
| **EXECUTE** | X | Full output. Build. Ship. Do. | Hours |
| **EXPAND** | E | Scale up. Add scope. Increase ambition. | Days |
| **SCALE BACK** | B | Reduce scope. Lower ambition. Shed load. | Hours to days |

## 6.3 Compiler Decision Tree

The compiler evaluates in this exact order:

```
START
  │
  ▼
[σ < 1.0?]──YES──► HALT
  │ NO
  ▼
[σ > 6.0?]──YES──► SCALE BACK (immediate overload)
  │ NO
  ▼
[σ 4.0-6.0 AND SI < 1.0?]──YES──► SCALE BACK
  │ NO
  ▼
[σ 4.0-6.0 AND SI ≥ 1.0?]──YES──► EXPAND
  │ NO
  ▼
[σ 2.0-4.0 AND CI < 0.5?]──YES──► CLARIFY
  │ NO
  ▼
[σ 2.0-4.0 AND CI ≥ 0.5 AND SI < 0.5?]──YES──► FORTIFY
  │ NO
  ▼
[σ 2.0-4.0 AND CI ≥ 0.5 AND SI ≥ 0.5?]──YES──► EXECUTE
  │ NO
  ▼
[σ 1.0-2.0 AND CI < 0.5?]──YES──► WAIT
  │ NO
  ▼
[σ 1.0-2.0 AND CI ≥ 0.5 AND SI < 0.5?]──YES──► STABILIZE
  │ NO
  ▼
[σ 1.0-2.0 AND CI ≥ 0.5 AND SI ≥ 0.5?]──YES──► GRIND
  │
  ▼
END
```

## 6.4 Complete Compiler Truth Table

| σ Range | CI Range | SI Range | Directive |
|---------|----------|----------|-----------|
| 0.00–0.99 | any | any | **HALT** |
| 1.00–1.99 | 0.00–0.49 | any | **WAIT** |
| 1.00–1.99 | 0.50–1.49 | 0.00–0.49 | **STABILIZE** |
| 1.00–1.99 | 0.50–1.49 | 0.50+ | **GRIND** |
| 1.00–1.99 | 1.50+ | 0.00–0.49 | **STABILIZE** |
| 1.00–1.99 | 1.50+ | 0.50+ | **GRIND** |
| 2.00–3.99 | 0.00–0.49 | any | **CLARIFY** |
| 2.00–3.99 | 0.50+ | 0.00–0.49 | **FORTIFY** |
| 2.00–3.99 | 0.50+ | 0.50+ | **EXECUTE** |
| 4.00–5.99 | any | 0.00–0.99 | **SCALE BACK** |
| 4.00–5.99 | any | 1.00+ | **EXPAND** |
| 6.00+ | any | any | **SCALE BACK** |

## 6.5 Directive Specifications

### HALT (H)

**Trigger:** σ < 1.0

**Meaning:** Your forward force is less than your friction. Continuing action will accelerate collapse.

**Required actions:**
1. Stop all non-essential output immediately
2. Cancel or postpone commitments if possible
3. Prioritize: sleep, nutrition, safety
4. Do not make decisions
5. Reassess in 4-8 hours minimum

**Exit condition:** σ ≥ 1.0 on reassessment

### WAIT (W)

**Trigger:** σ 1.0–1.99 AND CI < 0.5

**Meaning:** You have minimal capacity and cannot see clearly. Action now would be misdirected.

**Required actions:**
1. Pause current task
2. Do not start new tasks
3. Allow fog to clear naturally (walk, rest, change environment)
4. Reassess in 30-60 minutes

**Exit condition:** CI ≥ 0.5 or σ changes zone

### STABILIZE (S)

**Trigger:** σ 1.0–1.99 AND CI ≥ 0.5 AND SI < 0.5

**Meaning:** You have low capacity and your foundation is cracking. Shore up the base.

**Required actions:**
1. Identify what's destabilizing (relationships, finances, health, environment)
2. Address ONE destabilizing factor
3. Avoid adding ANY new load
4. Reassess after stabilizing action

**Exit condition:** SI ≥ 0.5

### CLARIFY (C)

**Trigger:** σ 2.0–3.99 AND CI < 0.5

**Meaning:** You have good capacity but can't see clearly. Remove noise before acting.

**Required actions:**
1. List everything competing for attention
2. Identify the ONE thing that matters most right now
3. Eliminate, delegate, or defer everything else
4. Reassess once clarity improves

**Exit condition:** CI ≥ 0.5

### FORTIFY (F)

**Trigger:** σ 2.0–3.99 AND CI ≥ 0.5 AND SI < 0.5

**Meaning:** You have capacity and clarity but your foundation needs work. Build structure.

**Required actions:**
1. Pause expansion/scaling activities
2. Invest time in foundation: systems, health, relationships, finances
3. Create buffer/margin
4. Reassess after fortifying action

**Exit condition:** SI ≥ 0.5

### GRIND (G)

**Trigger:** σ 1.0–1.99 AND CI ≥ 0.5 AND SI ≥ 0.5

**Meaning:** Low capacity but stable and clear. Sustainable slow progress is possible.

**Required actions:**
1. Continue current work at reduced pace
2. Focus on ONE priority only
3. Protect energy — no new commitments
4. Accept slower output as appropriate

**Exit condition:** σ ≥ 2.0 (upgrade to EXECUTE) or σ < 1.0 (downgrade to HALT)

### EXECUTE (X)

**Trigger:** σ 2.0–3.99 AND CI ≥ 0.5 AND SI ≥ 0.5

**Meaning:** Optimal zone. All systems green. Build.

**Required actions:**
1. Commit fully to primary objective
2. Minimize distractions
3. Push output
4. Ship/deliver/complete

**Exit condition:** Reassess at end of work block or when state feels changed

### EXPAND (E)

**Trigger:** σ 4.0–5.99 AND SI ≥ 1.0

**Meaning:** High capacity with strong foundation. Scale up.

**Required actions:**
1. Add scope if valuable
2. Take on stretch goals
3. Make bold decisions
4. Use the surplus wisely — this state is temporary

**Exit condition:** σ < 4.0 (return to EXECUTE) or SI < 1.0 (SCALE BACK)

### SCALE BACK (B)

**Trigger:** σ 4.0–5.99 AND SI < 1.0, OR σ ≥ 6.0

**Meaning:** Ambition exceeds foundation, or total overload. Reduce before you break.

**Required actions:**
1. Immediately reduce commitments
2. Postpone non-critical items
3. Say no to new requests
4. Focus only on what's essential

**Exit condition:** σ < 4.0 or SI ≥ 1.0

## 6.6 Compiler Edge Cases

### All Zeros: 00000

```
E=0, R=0, C=0, D=0, S=0
σ = (0+0)/(0+1) = 0.00
CI = 0/(0+1) = 0.00
SI = 0/((0+0)/2) = undefined → treat as 0

Directive: HALT
```

This represents complete system collapse. Emergency protocols apply.

### All Nines: 99999

```
E=9, R=9, C=9, D=9, S=9
σ = (9+9)/(9+1) = 1.80
CI = 9/(9+1) = 0.90
SI = 9/((9+9)/2) = 1.00

Directive: GRIND
```

Counterintuitively, all-9s is GRIND not EXECUTE. Why? Because R=9 means massive friction, which caps forward movement despite high energy and drive.

### Maximum Forward: 99090

```
E=9, R=9, C=0, D=9, S=0
σ = (9+9)/(9+1) = 1.80
CI = 0/(9+1) = 0.00
SI = 0/((9+9)/2) = 0.00

Directive: WAIT
```

High energy and drive with no clarity, stability, or relief from resistance. Cannot see, cannot sustain. Must wait.

### Maximum Clarity with No Energy: 09900

```
E=0, R=9, C=9, D=0, S=0
σ = (0+0)/(9+1) = 0.00
CI = 9/(9+1) = 0.90
SI = 0/0 = undefined → 0

Directive: HALT
```

You can see everything perfectly but have nothing to work with. HALT.

---

# 7. THE RUNTIME: DAILY PROTOCOL

## 7.1 Minimum Viable Protocol

The simplest implementation that still works:

**Once per day, any time:**
1. Rate E, R, C, D, S (0-9)
2. Write the 5-digit code
3. Compute SEKED: (E+D)/(R+1)
4. If σ < 1: HALT
5. If σ 1-2: GRIND or WAIT (check clarity)
6. If σ 2-4: EXECUTE or CLARIFY
7. If σ > 4: EXPAND or SCALE BACK (check stability)
8. Do the directive

**Time required:** 60-90 seconds

## 7.2 Standard Protocol

Recommended for consistent results:

**Morning (within 30 min of starting work):**
1. Log state: ERCDS
2. Compute all three ratios
3. Receive directive
4. Execute until next check

**Midday (around 5-6 hours after morning):**
1. Re-log state
2. Recompute
3. Adjust based on new directive

**Evening (end of work):**
1. Final state log
2. Note: Did directive match what you actually did?
3. Note: What changed E, R, C, D, S during the day?

**Time required:** 5 minutes total

## 7.3 Intensive Protocol

For high-performance periods or recovery:

**Every 2-3 hours:**
1. Quick state check (can be rapid: "Still 72839 or changed?")
2. Recompute only if changed significantly (±2 in any primitive)
3. Re-execute directive

**Daily review:**
1. Plot the day's states
2. Identify patterns
3. Note correlations (what raised E? What increased R?)

**Weekly review:**
1. Average state for the week
2. Dominant directive
3. Trend direction (improving, declining, stable)

## 7.4 Logging Methods

### Paper Method

```
Date: ________
Time: ________

E: [0][1][2][3][4][5][6][7][8][9]  (circle one)
R: [0][1][2][3][4][5][6][7][8][9]
C: [0][1][2][3][4][5][6][7][8][9]
D: [0][1][2][3][4][5][6][7][8][9]
S: [0][1][2][3][4][5][6][7][8][9]

Code: __ __ __ __ __

σ = (E+D)/(R+1) = _____
Directive: __________
```

### Digital Shorthand

Text file, one line per entry:
```
2026-02-04 0915 72839 X
2026-02-04 1430 54637 C
2026-02-04 2100 33525 S
```

### Spreadsheet

| Date | Time | E | R | C | D | S | σ | CI | SI | Directive |
|------|------|---|---|---|---|---|---|----|----|-----------|
| 2026-02-04 | 09:15 | 7 | 2 | 8 | 3 | 9 | 3.33 | 2.67 | 1.80 | EXECUTE |

## 7.5 Common Mistakes

| Mistake | Problem | Fix |
|---------|---------|-----|
| Rating mood instead of state | Mood ≠ capacity | Use measurement questions from 3.4 |
| Skipping when "feeling fine" | Misses baseline and trends | Log even when neutral |
| Overriding directive | System becomes advisory, loses power | Trust the math for 30 days |
| Rating what you wish, not what is | Garbage in = garbage out | Be honest or don't bother |
| Computing without acting | Measurement without action is useless | Directive is mandatory |

---

# 8. EDGE CASES & FAILURE STATES

## 8.1 Extreme State Handling

### Total Collapse (σ < 0.5)

When σ drops below 0.5, standard HALT may be insufficient.

**Enhanced protocol:**
1. Contact trusted person immediately
2. Do not be alone if possible
3. Focus only on: safety, hydration, rest
4. Do not reassess for 24+ hours
5. If σ < 0.5 persists 48+ hours: seek professional help

### Sustained Overload (σ > 5.0 for 3+ days)

**Warning signs:**
- Sleep disruption
- Irritability increase
- Physical symptoms (headache, tension)

**Protocol:**
1. Forced SCALE BACK regardless of SI
2. Cancel non-essential commitments
3. Reintroduce recovery activities (didn't ask, just do)
4. Recheck after 48 hours of reduced load

### Unstable Oscillation

When state swings wildly (e.g., 91919 → 19191 → 91919 within hours):

**Indicates:** External volatility or internal dysregulation

**Protocol:**
1. Recognize pattern after 3 swings
2. Default to most conservative directive from recent states
3. Prioritize STABILIZE regardless of ratios
4. Identify volatility source

## 8.2 System Contradictions

### High E + High R + High D + Low S

"I have energy and drive but everything is fighting me and my foundation is cracking."

**Resolution:** SI takes precedence. FORTIFY.

### High C + Low E + Low D

"I see everything clearly but have no energy or desire to act."

**Resolution:** This is valid clarity — you're clear that now is not the time. WAIT or HALT depending on σ.

### All Primitives at 5

The perfectly neutral state: `55555`

```
σ = (5+5)/(5+1) = 1.67
CI = 5/6 = 0.83
SI = 5/5 = 1.00
```

**Directive:** GRIND

This is baseline sustainable operation. Neither pushing nor recovering.

## 8.3 Invalid Input Handling

The system must reject:

| Invalid Input | Response |
|---------------|----------|
| Non-numeric values | "Invalid: digits only" |
| Values outside 0-9 | "Invalid: range 0-9" |
| Wrong length | "Invalid: exactly 5 digits required" |
| Empty input | "Invalid: state required" |
| Null/undefined | "Invalid: state required" |

**No guessing. No defaults. Invalid input = no output.**

## 8.4 Missing Data

If a primitive cannot be assessed:

1. **Try harder** — The question is simple. If you're alive and conscious, you can rate 0-9.
2. **Use last known** — If truly unable, use most recent value for that primitive (mark as estimate)
3. **Default to 5** — Only if no data exists at all (mark as assumed)

Missing data must be flagged. Decisions on flagged states carry lower confidence.

## 8.5 Conflicting Directives

If two assessments within a short period produce different directives:

**Rule:** More conservative directive wins.

Hierarchy (most to least conservative):
1. HALT
2. WAIT
3. STABILIZE
4. CLARIFY
5. FORTIFY
6. GRIND
7. SCALE BACK
8. EXECUTE
9. EXPAND

---

# 9. VISUAL SYSTEM & GLYPHS

## 9.1 Color Coding

### Directive Colors

| Directive | Color | Hex | Meaning |
|-----------|-------|-----|---------|
| HALT | Red | #E63946 | Stop |
| WAIT | Orange | #F4A261 | Pause |
| STABILIZE | Yellow | #E9C46A | Caution |
| CLARIFY | Light Blue | #A8DADC | Think |
| FORTIFY | Purple | #9B5DE5 | Build foundation |
| GRIND | Gray | #6C757D | Sustain |
| EXECUTE | Green | #2A9D8F | Go |
| EXPAND | Bright Green | #00F5D4 | Full speed |
| SCALE BACK | Dark Orange | #D62828 | Reduce |

### Zone Colors

| σ Zone | Color |
|--------|-------|
| 0.0–0.99 (Collapse) | Deep Red |
| 1.0–1.99 (Grind) | Amber |
| 2.0–3.99 (Optimal) | Green |
| 4.0–5.99 (Surge) | Bright Blue |
| 6.0+ (Overload) | Magenta |

## 9.2 Glyphs

Simple visual symbols for each primitive:

| Primitive | Glyph | Representation |
|-----------|-------|----------------|
| E (Energy) | ⚡ | Lightning bolt |
| R (Resistance) | ◆ | Diamond (pressure) |
| C (Clarity) | ◎ | Target/focus |
| D (Drive) | ► | Arrow (direction) |
| S (Stability) | ▣ | Solid square (foundation) |

### State Glyph

A complete state can be represented as:

```
⚡7 ◆2 ◎8 ►3 ▣9
```

Or in a compact visual block:

```
┌─────────────┐
│ ⚡7  ◆2  ◎8 │
│    ►3  ▣9   │
│   σ: 3.33   │
│  [EXECUTE]  │
└─────────────┘
```

## 9.3 Numeric Display Bars

For interfaces, display each primitive as a bar:

```
E ████████░░ 7
R ██░░░░░░░░ 2
C █████████░ 8
D ███░░░░░░░ 3
S ██████████ 9
```

## 9.4 Ratio Dial

The SEKED ratio can be displayed as a dial:

```
     COLLAPSE  GRIND  OPTIMAL  SURGE  OVERLOAD
        │        │       │       │        │
   0────1────────2───────3───────4────────5────6+
                         ▲
                       3.33
```

## 9.5 Historical Trend Line

For tracking over time:

```
σ
5│                    ·
4│              ·  ·     ·
3│     ·  ·  ·                ·  ·
2│  ·                              ·
1│·                                    ·
0└──────────────────────────────────────
  Day 1                          Day 14
```

---

# 10. VALIDATION & TESTING

## 10.1 Self-Consistency Tests

The compiler must pass these tests:

### Test 1: Determinism
Same input → same output, always.

```
Input: 72839
Run 1: EXECUTE
Run 2: EXECUTE
Run 3: EXECUTE
Pass: ✓
```

### Test 2: Complete Coverage
Every valid state produces a directive.

```
For all E in [0-9]:
  For all R in [0-9]:
    For all C in [0-9]:
      For all D in [0-9]:
        For all S in [0-9]:
          Assert: compile(ERCDS) returns valid directive

Total states: 10^5 = 100,000
All must return one of 9 directives.
```

### Test 3: Boundary Accuracy
Threshold transitions are correct.

```
Test: σ at exactly 1.00
State: E=0, R=0, C=5, D=1, S=5
σ = (0+1)/(0+1) = 1.00
Expected: NOT HALT (σ ≥ 1.00)
Actual: GRIND (CI=5.00, SI=5.00)
Pass: ✓
```

### Test 4: Conservative Hierarchy
Lower states don't produce less conservative directives.

```
If state A has lower σ than state B:
  directive(A) must be ≤ directive(B) in hierarchy
  (where HALT < WAIT < STABILIZE < ... < EXPAND)
```

## 10.2 Real-World Validation

### Scenario Tests

**Scenario 1: Morning after poor sleep**
- E=3, R=4, C=4, D=5, S=6
- Expected: Low energy, moderate resistance, okay clarity
- σ = 8/5 = 1.60 → GRIND zone
- CI = 0.80 → CAUTION
- SI = 1.50 → FORTRESS
- Directive: GRIND ✓ (matches intuition: sustainable slow work)

**Scenario 2: Big deadline day**
- E=7, R=6, C=7, D=9, S=4
- Expected: High energy and drive, high resistance, shaky foundation
- σ = 16/7 = 2.29 → OPTIMAL
- CI = 1.00 → CAUTION
- SI = 0.50 → STRESSED
- Directive: FORTIFY ✓ (matches intuition: don't push, stabilize)

**Scenario 3: Post-vacation**
- E=8, R=1, C=8, D=6, S=9
- Expected: Recharged, low friction, high stability
- σ = 14/2 = 7.00 → OVERLOAD
- CI = 4.00 → SHARP
- SI = 1.29 → SOLID
- Directive: SCALE BACK ✓ (matches intuition: don't overcommit immediately)

Wait — that doesn't feel right. Let's check.

Actually, this highlights an important edge case: High capacity post-recovery still triggers SCALE BACK at σ > 6.0. This is correct because:
- σ > 6.0 is unsustainable regardless of how you got there
- Post-vacation surge often leads to overcommitment
- The directive is protective

### User Calibration Test

New users should run this calibration:

1. Log state for 7 consecutive days without acting on directives
2. Note what you actually did each day
3. Compare: Did your actions match what the compiler would have said?
4. Adjust rating calibration if systematic mismatch

## 10.3 Compiler Test Suite

Full test vectors:

| # | E | R | C | D | S | σ | CI | SI | Expected |
|---|---|---|---|---|---|---|----|----|----------|
| 1 | 0 | 0 | 0 | 0 | 0 | 0.00 | 0.00 | 0.00 | HALT |
| 2 | 5 | 5 | 5 | 5 | 5 | 1.67 | 0.83 | 1.00 | GRIND |
| 3 | 9 | 0 | 9 | 9 | 9 | 18.00 | 9.00 | 1.00 | SCALE BACK |
| 4 | 9 | 9 | 9 | 9 | 9 | 1.80 | 0.90 | 1.00 | GRIND |
| 5 | 7 | 2 | 8 | 3 | 9 | 3.33 | 2.67 | 1.80 | EXECUTE |
| 6 | 3 | 7 | 2 | 4 | 3 | 0.88 | 0.25 | 0.86 | HALT |
| 7 | 5 | 3 | 2 | 6 | 7 | 2.75 | 0.50 | 1.27 | EXECUTE |
| 8 | 6 | 4 | 1 | 7 | 4 | 2.60 | 0.20 | 0.62 | CLARIFY |
| 9 | 8 | 2 | 7 | 8 | 3 | 5.33 | 2.33 | 0.38 | SCALE BACK |
| 10 | 4 | 6 | 6 | 3 | 8 | 1.00 | 0.86 | 2.29 | GRIND |

---

# 11. IMPLEMENTATION GUIDE

## 11.1 Paper Implementation

**Requirements:**
- Paper or notebook
- Pen
- Basic arithmetic ability

**Daily flow:**
1. Draw 5-box grid labeled E R C D S
2. Fill each with 0-9
3. Calculate σ = (E+D)/(R+1)
4. Look up directive in simplified table
5. Do it

**Simplified table for paper use:**

| σ | Directive |
|---|-----------|
| < 1 | HALT |
| 1–2 | GRIND (or WAIT if can't think) |
| 2–4 | EXECUTE (or CLARIFY if foggy) |
| > 4 | SCALE BACK |

## 11.2 Spreadsheet Implementation

**Setup:**
1. Columns: Date, Time, E, R, C, D, S
2. Computed columns:
   - σ: =(E+D)/(R+1)
   - CI: =C/(R+1)
   - SI: =S/((E+D)/2)
3. Directive column: Nested IF formula or lookup table

**Formula for directive (Excel/Sheets):**
```
=IF(σ<1,"HALT",
 IF(σ<2,IF(CI<0.5,"WAIT",IF(SI<0.5,"STABILIZE","GRIND")),
 IF(σ<4,IF(CI<0.5,"CLARIFY",IF(SI<0.5,"FORTIFY","EXECUTE")),
 IF(SI<1,"SCALE BACK","EXPAND"))))
```

## 11.3 Mobile App Specification

**MVP Features:**
1. State input: 5 sliders or number pickers (0-9)
2. Compute button: Calculates all ratios
3. Directive display: Large, colored, unmissable
4. Log: Saves timestamp + state + directive

**Advanced Features:**
1. Historical chart (σ over time)
2. Pattern detection ("Your R spikes on Mondays")
3. Reminder notifications
4. Export to CSV

**Technical Requirements:**
- iOS compatible (iPhone-first per user constraint)
- No external dependencies
- No auth required
- Works offline
- Local storage only

## 11.4 API Specification

For integration with other systems:

**Endpoint:** `/compile`

**Request:**
```json
{
  "state": {
    "E": 7,
    "R": 2,
    "C": 8,
    "D": 3,
    "S": 9
  }
}
```

**Response:**
```json
{
  "input": "72839",
  "ratios": {
    "seked": 3.33,
    "clarity_index": 2.67,
    "structural_integrity": 1.80
  },
  "zones": {
    "seked": "OPTIMAL",
    "clarity": "SHARP",
    "stability": "FORTRESS"
  },
  "directive": "EXECUTE",
  "directive_code": "X"
}
```

---

# 12. GLOSSARY

| Term | Definition |
|------|------------|
| **C (Clarity)** | Primitive measuring signal-to-noise ratio in thought. Range 0-9. |
| **CI (Clarity Index)** | Ratio: C/(R+1). Measures decision-making capacity. |
| **Compiler** | The function that converts state → directive. |
| **D (Drive)** | Primitive measuring directional pull toward outcome. Range 0-9. |
| **Directive** | Output action from compiler. One of 9 possible commands. |
| **E (Energy)** | Primitive measuring available fuel for action. Range 0-9. |
| **Grammar** | The rules for expressing state (5-digit code format). |
| **Operator** | A ratio that combines primitives to reveal meaning. |
| **Primitive** | One of five base states (E, R, C, D, S). |
| **R (Resistance)** | Primitive measuring friction opposing movement. Range 0-9. |
| **Ratio** | Relationship between primitives that reveals actionable truth. |
| **Runtime** | The daily protocol for using the system. |
| **S (Stability)** | Primitive measuring structural integrity under load. Range 0-9. |
| **SEKED (σ)** | Primary ratio: (E+D)/(R+1). Master system state. |
| **SI (Structural Integrity)** | Tertiary ratio: S/((E+D)/2). Foundation capacity. |
| **State** | Complete 5-digit code representing current internal condition. |
| **Zone** | Range of ratio values that share meaning and response. |

---

# APPENDIX A: Quick Reference Card

```
┌────────────────────────────────────────────────────────┐
│                    SEKED QUICK REF                     │
├────────────────────────────────────────────────────────┤
│  STATE: [E][R][C][D][S]    (each 0-9)                 │
│                                                        │
│  SEKED (σ) = (E + D) / (R + 1)                        │
│                                                        │
│  σ < 1.0  →  HALT (stop, recover)                     │
│  σ 1-2    →  GRIND / WAIT / STABILIZE                 │
│  σ 2-4    →  EXECUTE / CLARIFY / FORTIFY              │
│  σ > 4    →  EXPAND / SCALE BACK                      │
│                                                        │
│  CI = C/(R+1)    |  < 0.5 = fog  |  ≥ 0.5 = clear    │
│  SI = S/((E+D)/2)|  < 0.5 = weak |  ≥ 0.5 = solid    │
├────────────────────────────────────────────────────────┤
│  DAILY: Rate → Compute → Execute → Repeat             │
└────────────────────────────────────────────────────────┘
```

---

# APPENDIX B: First 30-Day Protocol

**Days 1-7: Calibration**
- Log state 1x daily
- Do NOT act on directives
- Just observe and calibrate your rating accuracy

**Days 8-14: Testing**
- Log state 2x daily (morning + evening)
- Follow directives loosely
- Note when directive feels wrong (recalibrate)

**Days 15-21: Commitment**
- Log state 2x daily
- Follow directives strictly
- Override only with documented reason

**Days 22-30: Integration**
- Log state 3x daily
- Directives are now default behavior
- Begin noticing patterns

**After Day 30:** System is installed. Continue as needed.

---

# DOCUMENT END

**Version:** 1.0
**Status:** Production Ready
**Next Step:** Review with secondary AI (ChatGPT), then build iOS app
