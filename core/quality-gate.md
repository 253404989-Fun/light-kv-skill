# LIGHT KV Quality Gate

## Contents

- [Purpose](#1-purpose)
- [Use Two Audit Moments](#2-use-two-audit-moments)
- [Apply Hard Gates](#3-apply-hard-gates)
- [Score Aesthetic Quality](#4-score-aesthetic-quality)
- [Inspect Content](#5-inspect-content)
- [Inspect Format](#6-inspect-format)
- [Inspect Extension Readiness](#7-inspect-extension-readiness)
- [Inspect Visual Failure Modes](#8-inspect-visual-failure-modes)
- [Return One Status](#9-return-one-status)

## 1. Purpose

Prevent a visually attractive result from passing when it violates content, canvas, strategy, or LIGHT KV identity.

Apply `R-QA-01` and all requirements referenced by `../tests/acceptance-criteria.md`.

## 2. Use Two Audit Moments

### Preflight

Audit before generation:

- Brief parsing is complete.
- Copy Whitelist is closed.
- Canvas Lock is recorded.
- Reference IDs and contributions are recorded.
- Strategy escalation is justified.
- visual risks are checked against the Failure Library.

Do not generate when a HARD Constraint remains materially ambiguous.

### Postflight

Audit the rendered result:

- compare all visible copy with the whitelist;
- verify dimensions and aspect ratio;
- inspect for banned symbols and template effects;
- compare aesthetic quality with the selected Core Parent;
- verify that the selected Reference relationships survived adaptation;
- confirm that no source identity or watermark transferred.
- verify typography separation, production provenance, safe zones, and extension targets when the work is production-ready.

## 3. Apply Hard Gates

Use the ten gates defined in `../tests/acceptance-criteria.md`:

- `H-01` Copy Whitelist;
- `H-02` Canvas Lock;
- `H-03` Reference First;
- `H-04` strategy priority;
- `H-05` visual exclusions;
- `H-06` color roles;
- `H-07` light mechanism;
- `H-08` audit completeness.
- `H-09` Typography Production;
- `H-10` Extension Readiness.

Any hard-gate violation produces `FAIL-HARD`. Do not average hard failures into a quality score.

## 4. Score Aesthetic Quality

Score each item from 0 to 2:

- `Q-01` Beauty First;
- `Q-02` Simple Forms, Sophisticated Relationships;
- `Q-03` space and negative space;
- `Q-04` light and material;
- `Q-05` color architecture;
- `Q-06` restrained Typography.

Require:

- at least 9 of 12 total points;
- no item scored 0;
- no material departure from the selected Core Parent.

If hard gates pass but the score is insufficient, return `FAIL-QUALITY` and revise the visual relationships rather than adding effects.

## 5. Inspect Content

Compare visible text character by character when possible.

Check:

- exact event name;
- subtitle;
- date;
- location;
- organizer;
- requested translation;
- absence of all forbidden copy.

Treat one unauthorized word as a hard failure.

## 6. Inspect Format

Verify:

- pixel dimensions;
- aspect ratio;
- required orientation;
- sufficient resolution for intended use;
- protected Logo and copy safe areas when provided.

Do not approve a visually strong result in the wrong format.

Do not infer format compliance from the generation prompt. Measure the rendered file. A native generator output that only approximates the locked ratio fails `H-02` as a delivery artifact. Preserve that native output, then use a deterministic, non-distorting crop or pad to create an exact locked-canvas artifact and audit that final file separately.

## 7. Inspect Extension Readiness

For production-ready or multi-format work, verify:

- the production master and its resolution provenance;
- a textless background plate;
- a separate title layer or deterministic layout specification;
- copy-safe and critical-visual-safe zones;
- representative crop and recompose decisions for 32:9, 4:5, and 9:16;
- absence of stretching, mirrored filler, or destructive cropping.

Do not treat a 4K interpolation as native detail. Do not require `H-10` for an explicitly labeled concept-only task, but do require it for exhibition, campaign system, or production-master requests.

## 8. Inspect Visual Failure Modes

Look specifically for:

- generic technology stock appearance;
- object-led futurism;
- door, corridor, city, or human-journey metaphors;
- particle and Glow accumulation;
- flat brand-color coverage;
- pseudo-interface typography;
- Reference text or brand contamination.

Use `failure-library.md` for correction patterns.

## 9. Return One Status

Return exactly one:

- `PASS`;
- `FAIL-HARD`;
- `FAIL-QUALITY`;
- `BLOCKED`.

For failure, list:

```text
Failed Gate:
Evidence:
Required Correction:
Reference to Recheck:
```

Do not use “partially passed” when a hard gate failed.
