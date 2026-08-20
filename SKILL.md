---
name: light-kv
description: Reference-first design system for high-end enterprise technology key visuals. Use when an Agent needs to plan, generate, adapt, recompose, or audit static KV artwork for technology conferences, AI summits, enterprise launches, exhibitions, brand events, or annual meetings while enforcing Beauty First, Copy Whitelist, Canvas Lock, Core Aesthetic Parents, Generative Reference Library, and anti-template quality gates.
---

# LIGHT KV

## Purpose

Create commercially credible enterprise technology key visuals through a maintainable design system rather than a one-off prompt.

Prioritize:

> Beauty First. Reference First. Adapt → Recompose → Explore.

Do not equate technology with robots, chips, future cities, HUD interfaces, code rain, glowing spheres, or particle piles.

## Load the Core Rules

For every LIGHT KV task, read:

1. `core/visual-constitution.md` for the aesthetic boundary.
2. `core/brief-parser.md` for HARD constraints, Copy Whitelist, and Canvas Lock.
3. `core/generation-strategy.md` for Reference First and strategy selection.

Before generation or final approval, also read:

4. `core/failure-library.md` for negative-pattern detection.
5. `core/quality-gate.md` for preflight and postflight audits.

For production-ready or multi-format work, also read:

6. `core/typography-system.md` for deterministic, reusable type hierarchy.
7. `core/extension-readiness.md` for production resolution and extension deliverables.

Do not replace these files with improvised rules.

## Classify the Request

Identify one or more task types:

- `PLAN`: convert a Brief into a visual direction without generating an image;
- `GENERATE`: produce or revise a static KV;
- `AUDIT`: evaluate a KV against LIGHT KV requirements;
- `LIBRARY`: add, classify, or review visual References.

Apply the same Copy Whitelist, Canvas Lock, and aesthetic constitution to every task type.

## Execute the Workflow

### 1. Parse the Brief

Separate:

- `HARD Constraints`: exact copy, date, location, Logo, assets, language, and dimensions;
- `SOFT Preferences`: brand color, mood, industry, visual intensity, and style preferences;
- `SEMANTIC Meaning`: AI, technology, intelligence, innovation, sustainability, or future.

Do not translate semantic meaning directly into literal technology symbols.

If a missing fact can be left blank, leave it blank. If a missing HARD Constraint would materially alter the result, mark the task `BLOCKED` and ask only for that information.

### 2. Lock Copy

Create a closed Copy Whitelist containing only:

- text explicitly provided by the user;
- translations explicitly requested or provided by the user;
- recorded date or location format transformations.

Reject all other text, including Reference copy, slogans, Logo text, credits, dates, watermarks, and pseudo-data.

When no copy is provided, keep the typography zone empty.

### 3. Lock the Canvas

Use this priority:

1. exact user dimensions;
2. user-specified aspect ratio;
3. default 16:9 landscape.

For a final enterprise 16:9 master without specified pixels, use 3840 × 2160. Treat lower-resolution generations as previews or intermediates until the production master is prepared and provenance is recorded.

Never let a Reference ratio override the locked canvas.

### 4. Align with a Core Parent

Read `references/catalogs/core-aesthetic-parents.yaml`. The public package contains metadata-only Reference cards. If the user supplies owned or licensed visual References, inspect those images and map them to the same metadata fields before use.

Select the closest Core Aesthetic Parent to calibrate:

- restraint;
- negative space;
- scale;
- light behavior;
- spatial quality;
- typography hierarchy.

Use the Core Parent as an aesthetic boundary, not as a literal template.

### 5. Retrieve Generative References

Read `references/catalogs/generative-reference-library.yaml`. Use the structural descriptions as the minimum retrieval layer. Inspect user-supplied visual assets only when they are owned, licensed, or explicitly authorized for analysis.

For every selected Reference, record:

- Reference ID;
- structural contribution;
- relationships to preserve;
- content to change;
- prohibited transfers.

Do not assume that visual assets are bundled. Never fetch, reconstruct, or redistribute the private source images represented by the public metadata cards.

### 6. Check Failure Risks

Read `references/catalogs/failure-library.yaml` and compare the candidate direction with relevant failure symptoms.

Never use a Failure entry as a positive parent. Exclude `pending-review` assets from default retrieval.

If a user requests a failure pattern, identify the underlying need and propose a Core- and Generative-based alternative. State clearly when an insisted direction would fall outside LIGHT KV.

Treat explicitly requested banned elements as an unresolved user-intent conflict, not as preferences that may be silently removed. After presenting the compatible alternative, return `BLOCKED` until the user accepts that alternative or explicitly chooses to proceed outside LIGHT KV. Do not mark preflight `PASS` based only on an unapproved reinterpretation.

### 7. Choose the Strategy

Choose `Adapt` when one mature Generative Reference can solve the Brief.

Choose `Recompose` only when one Reference is insufficient. Assign one dominant structural parent and give every additional Reference a limited role.

Choose `Explore` only after recording why both Adapt and Recompose fail. Continue to obey the Visual Constitution, Copy Whitelist, Canvas Lock, and Failure Library.

Do not choose Explore merely to appear original.

### 8. Define the Visual System

Describe:

- composition and spatial hierarchy;
- dominant scale relationships;
- light mechanism;
- material behavior;
- color roles: Background, Dominant, Brand Accent, Supporting Color, Highlight;
- typography zone and hierarchy;
- negative constraints.

For production-ready work, also define:

- textless background plate;
- copy-safe and critical-visual-safe zones;
- typography layer and fallback typeface;
- target extension ratios;
- crop versus recompose decisions.

Build complexity through scale, occlusion, distance, transparency, and light-color relationships. Prefer simple forms.

### 9. Run Preflight

Before generating, verify:

- the Brief is parsed;
- the Copy Whitelist is closed;
- the Canvas Lock is explicit;
- Reference IDs and contributions are recorded;
- strategy escalation is justified;
- Failure risks are named;
- no unresolved HARD Constraint remains.

Do not generate after a preflight hard failure.

### 10. Generate or Deliver the Plan

For a `PLAN` task, return the structured design direction and preflight status.

For a `GENERATE` task, use an available image-generation capability only after preflight passes. If no such capability is available, return a `PLAN` and state the limitation instead of pretending an image was generated. Preserve the locked canvas and whitelist. Use authorized visual assets only as analysis references; do not reproduce source identity, text, Logo, credit, or watermark.

Generate the background without text by default, then add authorized copy through a deterministic typography layer when available. Keep the background and typography as separate deliverables for extension-ready work.

Treat the generator's native file as an intermediate artifact until its pixel dimensions and aspect ratio are measured. If the native file is only approximately equal to the Canvas Lock, preserve it as evidence and create a deterministic crop or pad that matches the lock exactly. Do not distort the artwork, silently change the target ratio, or mark the native near-match as `PASS`.

For an `AUDIT` task, do not modify the artwork unless the user asks for revision.

### 11. Run Postflight

Apply `core/quality-gate.md`.

Audit the normalized delivery artifact rather than relying on the generator's requested ratio. Record both native and final dimensions whenever normalization was required.

For production-ready work, audit the complete delivery package and representative extension ratios. Do not approve a single flattened composition as extension-ready when its text, focus, or safe zones cannot adapt.

Return exactly one status:

- `PASS`;
- `FAIL-HARD`;
- `FAIL-QUALITY`;
- `BLOCKED`.

Treat one unauthorized word or a wrong canvas as a hard failure. Do not allow aesthetic quality to compensate for a hard failure.

## Use the Output Contract

For planning and Dry Run tasks, return:

```text
HARD Constraints:
SOFT Preferences:
SEMANTIC Meaning:

Copy Whitelist:
Copy Transformations:
Forbidden Copy:

Canvas Lock:

Core Aesthetic Parent:
Generative References:
Reference Contributions:

Strategy:
Strategy Rationale:

Visual Structure:
Color Roles:
Typography Plan:
Production Resolution:
Background Plate:
Safe Zones:
Extension Targets:
Crop / Recompose Plan:
Negative Constraints:

Preflight Result:
```

Keep the user-facing answer concise while retaining the complete internal decision record when auditing or testing.

## Maintain the Library

For `LIBRARY` tasks, read:

- `references/reference-metadata-schema.md`;
- `references/visual-library-index.md`;
- all affected catalogs;
- `core/failure-library.md`.

Assign a stable ID, record provenance, set rights status, and explain preserve/avoid logic. Record a file and crop range only when an authorized local asset exists. Do not add a Reference merely because it is attractive.

## Validate Changes

When changing the Skill or core rules:

1. run the relevant cases in `tests/test-briefs.md` as no-image Dry Runs;
2. apply `tests/acceptance-criteria.md`;
3. record material results before accepting the change.

Do not weaken a hard gate to make a test pass.
