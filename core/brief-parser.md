# LIGHT KV Brief Parser

## Contents

- [Purpose](#1-purpose)
- [Parse Three Layers](#2-parse-three-layers)
- [Build the Copy Whitelist](#3-build-the-copy-whitelist)
- [Apply Canvas Lock](#4-apply-canvas-lock)
- [Assign Color Inputs](#5-assign-color-inputs)
- [Detect Conflicts](#6-detect-conflicts)
- [Required Parser Output](#7-required-parser-output)

## 1. Purpose

Convert a user request into explicit design constraints before selecting References or proposing a visual direction.

Apply `R-COPY-01`, `R-CANVAS-01`, `R-CANVAS-02`, `R-COLOR-01`, `R-TYPE-01`, `R-TYPE-02`, `R-RES-01`, and `R-EXT-01`.

## 2. Parse Three Layers

### HARD Constraints

Record facts that must not change:

- event or product name;
- subtitle;
- date;
- location;
- organizer;
- Logo and locked brand assets;
- exact required copy;
- canvas ratio or pixel dimensions;
- intended display, print, or exhibition use;
- required extension ratios and physical output specifications;
- mandatory language or translation.

Do not silently correct, rewrite, omit, or extend HARD Constraints.

### SOFT Preferences

Record preferences that may be designed:

- brand colors;
- style adjectives;
- industry context;
- mood;
- desired intensity;
- visual references named by the user.

Interpret these through the Visual Constitution. Do not treat them as permission to break HARD Constraints or create unapproved copy.

### SEMANTIC Meaning

Record concepts used only to understand the topic:

- AI;
- technology;
- environmental responsibility;
- intelligence;
- innovation;
- future.

Do not translate semantic meaning directly into robots, chips, leaves, cities, interfaces, or other literal symbols.

## 3. Build the Copy Whitelist

Create a closed list containing only:

1. text explicitly provided by the user;
2. translations explicitly requested or explicitly supplied by the user;
3. recorded date and location format transformations.

For every transformation, record:

- source text;
- output text;
- transformation type;
- user authorization.

Treat all other text as forbidden, including:

- slogans inferred from the theme;
- English subtitles not requested by the user;
- placeholder or decorative pseudo-copy;
- words visible in References;
- Reference logos, dates, names, credits, and watermarks.

If the whitelist is empty, plan blank typography zones. Never fill them with invented words.

## 4. Apply Canvas Lock

Use this priority:

1. exact user pixel dimensions;
2. user-specified ratio;
3. default 16:9 landscape.

Record both the locked canvas and its source.

When an enterprise final master is requested without exact pixels, record 3840 × 2160 as the default 16:9 production resolution. Keep a lower-resolution concept preview distinct from the production master.

Never derive the output canvas from a Reference. Recompose vertical or square reference structures to fit the locked canvas.

## 5. Assign Color Inputs

Record user-specified colors without immediately assigning them to the entire background.

Pass colors to the visual stage as candidate roles:

- Background;
- Dominant;
- Brand Accent;
- Supporting Color;
- Highlight.

Do not infer colors from an industry stereotype when the user has not requested them.

## 6. Detect Conflicts

Mark a conflict when:

- user copy instructions contradict each other;
- dimensions are inconsistent;
- a required visual element violates the Visual Constitution;
- a user asks to copy Reference text, Logo, or watermarks;
- a required asset is mentioned but not provided.

Treat explicitly requested visual elements as intentional user constraints even when they are not content or canvas HARD Constraints. If those elements violate the Visual Constitution, do not silently downgrade or remove them.

Resolve safe, reversible ambiguity with a stated assumption. Block only when an assumption could materially change HARD Constraints or falsely represent compliance with LIGHT KV.

For explicit aesthetic conflicts, propose a compatible abstraction and return `BLOCKED` until the user accepts it. If the user instead insists on the conflicting direction, state that the result falls outside LIGHT KV before proceeding.

## 7. Required Parser Output

Produce this structure before Reference selection:

```text
HARD Constraints:
SOFT Preferences:
SEMANTIC Meaning:

Copy Whitelist:
Copy Transformations:
Forbidden Copy:

Canvas Lock:
Canvas Source:
Production Resolution:
Intended Use:
Extension Targets:

Color Inputs:
Missing Locked Assets:
Conflicts:
Assumptions:
```

Use `../tests/test-briefs.md` to verify edge cases.
