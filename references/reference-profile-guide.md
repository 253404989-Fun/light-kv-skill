# Local Reference Profile Guide

The public LIGHT KV package deliberately ships without private third-party source images. Add a local Reference Profile when stronger visual calibration is needed.

## Add only authorized assets

Use an image only when the user owns it, holds a suitable license, or has explicit permission for the intended analysis and production workflow. Unknown rights permit visual analysis only; they do not permit redistribution or production reuse.

Store private assets under `references/local/`. This path is ignored by Git and must not be uploaded with the public package.

## Describe relationships, not style names

For each local asset, create a metadata record with:

```yaml
id: LOCAL-001
title: Structural description
file: ../local/example.jpg
classification: generative-reference
rights_status: owned
allowed_use: visual-analysis
contribution: spatial structure
preserve:
  - relationship worth adapting
avoid:
  - identity or surface feature that must not transfer
copy_policy: reject-all-reference-copy
canvas_policy: obey-canvas-lock
```

Use `licensed`, `owned`, `permission-granted`, or `unknown` only when supported by a record. Never infer permission from online availability.

## Retrieval order

1. Use the bundled metadata-only Core Aesthetic Parents to establish the quality boundary.
2. Match the Brief to bundled Generative Reference capabilities.
3. Use an authorized local image to calibrate a chosen capability when appropriate.
4. Read the Failure Library before confirming the direction.
5. Record Reference IDs and contributions in the preflight result.

Never move local images into the public catalogs unless their publication rights have been independently confirmed.
