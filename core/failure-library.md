# LIGHT KV Failure Library Rules

## Contents

- [Purpose](#1-purpose)
- [Never Use Failure as a Positive Parent](#2-never-use-failure-as-a-positive-parent)
- [Failure Signatures](#3-failure-signatures)
- [Audit Procedure](#4-audit-procedure)
- [Add a New Failure Entry](#5-add-a-new-failure-entry)
- [Conflict Handling](#6-conflict-handling)

## 1. Purpose

Use failure examples to recognize what not to do and to prescribe a better visual mechanism.

Apply `R-FAIL-01`, `R-VIS-01`, `R-ARCH-01`, `R-LIGHT-01`, `R-COLOR-01`, and `R-COPY-01`.

The canonical entries are stored in `../references/catalogs/failure-library.yaml`.

## 2. Never Use Failure as a Positive Parent

Do not adapt, imitate, or cite a Failure entry as the main generation direction.

When a user points to a Failure entry, identify the underlying need, such as contrast, movement, depth, or energy. Retrieve a Core Parent and a Generative Reference that solve that need without carrying the failed visual language.

## 3. Failure Signatures

### Symbol-Led Technology

Symptoms:

- robots, robot arms, chips, cities, data walls, HUD, code rain;
- direct illustration of AI or “future.”

Corrective direction:

- move meaning back to the Brief layer;
- express futurity through abstract space, light, scale, and color.

### Cheap 3D and Effect Stacking

Symptoms:

- glowing tubes or bars;
- science-fiction spheres;
- excessive bloom;
- Lens flare, speed trails, and random particles.

Corrective direction:

- reduce the object count;
- replace object Glow with illuminated edges, translucent planes, or reflected fields.

### Literal Future Journey

Symptoms:

- doors, corridors, rooms, portals, and distant cities;
- a human silhouette walking toward light;
- “opening the future” narrative imagery.

Corrective direction:

- retain only scale, perspective, interval, and depth;
- remove recognizable architecture and characters.

### Generic Color Treatment

Symptoms:

- blue/orange contrast used without a structural reason;
- rainbow gradients filling the frame;
- brand color covering the entire background;
- saturation used as the main source of impact.

Corrective direction:

- assign color roles;
- limit bright color to focal planes, edges, or intersections;
- restore dark or neutral breathing space.

### Template Typography

Symptoms:

- generic Future, Intelligence, Innovation, or Tomorrow slogans;
- pseudo-data labels and interface frames;
- copied Reference copy, Logo, author credit, or watermark.

Corrective direction:

- enforce the Copy Whitelist;
- use hierarchy, spacing, and alignment instead of decorative labels;
- leave empty space when copy is unavailable.

### Element Accumulation

Symptoms:

- adding particles, grids, lines, icons, and panels to make the image feel “richer”;
- no clear dominant relationship;
- negative space treated as unfinished space.

Corrective direction:

- remove effects and secondary elements;
- establish one dominant spatial or optical relationship;
- compare the result with a Core Aesthetic Parent.

## 4. Audit Procedure

For each candidate direction:

1. Search the Failure catalog for visually similar symptoms.
2. Record matched Failure IDs.
3. State the risk in concrete visual terms.
4. Specify a corrective mechanism.
5. Recheck after generation.

Do not record “avoid low quality” as an audit result. Name the visible symptom.

## 5. Add a New Failure Entry

Add a failure only when it teaches a reusable lesson.

Record:

- stable ID;
- source and crop range;
- rights status;
- failure rationale;
- symptom tags;
- elements to avoid;
- corrective direction;
- copy and canvas policies.

Do not add a case merely because it is unattractive. It must expose a repeatable failure mode relevant to LIGHT KV.

## 6. Conflict Handling

If a user explicitly requests a failure pattern:

1. identify the conflict;
2. explain the visual risk briefly;
3. propose a compatible abstraction;
4. return `BLOCKED` while the replacement remains unapproved;
5. proceed within LIGHT KV only after the user accepts the abstraction;
6. state clearly when an insisted direction falls outside LIGHT KV.

Do not silently ignore explicit user intent, and do not falsely label a conflicting result as LIGHT KV.
