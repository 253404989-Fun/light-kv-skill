# LIGHT KV Extension Readiness

## Contents

- [Purpose](#1-purpose)
- [Set the Production Master](#2-set-the-production-master)
- [Design an Extendable Background](#3-design-an-extendable-background)
- [Choose Crop or Recompose](#4-choose-crop-or-recompose)
- [Deliver the Production Package](#5-deliver-the-production-package)
- [Audit Extension Readiness](#6-audit-extension-readiness)

## 1. Purpose

Ensure a main KV can become an enterprise event system rather than a single locked image.

Apply `R-RES-01`, `R-EXT-01`, and `R-TYPE-02`.

## 2. Set the Production Master

Use this priority for final raster delivery:

1. exact user pixel dimensions;
2. dimensions derived from a provided production specification;
3. 3840 × 2160 for an enterprise 16:9 master;
4. a lower-resolution file only as an explicitly labeled concept preview.

Treat aspect ratio and production resolution as separate locks. Do not claim that interpolation creates new image detail. Record whether the master is native, normalized, upscaled, or outpainted.

For close-view print, oversized LED, or dimensions beyond the validated raster, request the physical specification or deliver an editable production package for specialist output.

For venue LED typography, record physical screen size, playback resolution, pixel pitch, and expected viewing distance when available. When these are missing, approve only the layout master and mark final on-site readability as pending production verification.

## 3. Design an Extendable Background

Build the textless background plate so that:

- the key spatial relationship survives without typography;
- no irreplaceable detail touches the trim edge;
- at least one calm copy-safe field exists;
- peripheral color and light can continue beyond the master;
- the visual focus is not dependent on one exact crop;
- the background contains no generated text, Logo, credit, or watermark.

Prefer continuous fields, large planes, and distributed depth over a centered emblem or a single sealed object.

## 4. Choose Crop or Recompose

Use `CROP` when the target retains the hierarchy and focal relationship without losing essential content.

Use `RECOMPOSE` when the target is extreme, including typical 32:9 screens and 9:16 displays, or when a crop would destroy the title zone or visual focus. Recompose from the same Core Parent, Generative References, color roles, light mechanism, and typography system.

Do not call a mechanically stretched, mirrored, blurred, or content-destructive crop an extension.

## 5. Deliver the Production Package

For an extension-ready enterprise KV, deliver or explicitly plan:

1. production master;
2. textless background plate;
3. standard title composition;
4. separate editable title layer or layout specification;
5. copy-safe and critical-visual-safe zones;
6. representative 32:9, 4:5, and 9:16 extension previews or plans;
7. provenance for normalization, upscale, outpaint, and typography.

Logo and sponsor assets remain separate when supplied.

## 6. Audit Extension Readiness

Fail `H-10` when:

- typography is inseparable from the only background artifact;
- the key visual collapses outside one crop;
- extension relies on stretching or mirrored filler;
- no copy-safe zone exists;
- delivery resolution is insufficient or misrepresented;
- extreme ratios are presented as safe crops when they require recomposition.

Do not claim final venue readability from pixel dimensions alone. Distinguish a passed layout master from venue production sign-off when physical display specifications are unavailable.
