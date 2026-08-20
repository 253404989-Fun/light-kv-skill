# LIGHT KV Typography System

## Contents

- [Purpose](#1-purpose)
- [Default Type Character](#2-default-type-character)
- [Build Hierarchy](#3-build-hierarchy)
- [Separate Type from Imagery](#4-separate-type-from-imagery)
- [Adapt Across Canvases](#5-adapt-across-canvases)
- [Reject Decorative Technology Type](#6-reject-decorative-technology-type)

## 1. Purpose

Make enterprise KV typography accurate, reusable, and portable across event formats.

Apply `R-TYPE-01` and `R-TYPE-02`.

## 2. Default Type Character

Use a neutral contemporary sans-serif with verified Chinese glyph coverage and an appropriate production license. Prefer regular, medium, or semibold weights.

Keep the default title treatment simple:

- no glyph distortion, slicing, outline, bevel, extrusion, Glow, or pseudo-digital treatment;
- normal tracking or only slight positive tracking;
- one clear alignment system;
- contrast created through scale, weight, placement, and negative space.

Do not use widely spaced individual Chinese characters as the default expression of sophistication.

When the user supplies no brand typeface, record the actual fallback used. For local prototypes, a system Chinese sans-serif such as PingFang SC is acceptable; do not package or redistribute the font file.

## 3. Build Hierarchy

Use no more levels than the Copy Whitelist requires:

1. primary title;
2. optional subtitle;
3. optional date and location;
4. optional organizer or required legal line.

Keep secondary information subordinate. Do not create labels, indices, coordinates, English aliases, or decorative microcopy.

## 4. Separate Type from Imagery

Generate a textless background plate by default. Add authorized copy through a deterministic layout layer whenever the available workflow supports it.

Deliver typography separately from the generated background when producing an extension-ready KV. This separation protects:

- exact Copy Whitelist compliance;
- typeface consistency;
- repositioning across ratios;
- later Logo and sponsor updates;
- clean background extension.

If the image generator must render text directly, treat the result as provisional until every character and hierarchy is verified.

## 5. Adapt Across Canvases

Preserve the typographic system, not absolute coordinates.

For each ratio:

- recalculate margins from the canvas;
- keep a stable title scale relationship;
- reposition the title into a verified copy-safe zone;
- avoid collisions with the visual focus;
- allow line breaks only when they preserve the exact text.

Do not mechanically scale one finished title layer into every format.

## 6. Reject Decorative Technology Type

Reject:

- HUD frames and interface labels;
- code-like monospaced decoration without a content reason;
- arbitrary English subtitles;
- extreme tracking used only to look futuristic;
- illegible low-contrast type over active light fields;
- text baked into a background when editable separation is required.

Typography does not manufacture technology. It establishes accurate information hierarchy.
