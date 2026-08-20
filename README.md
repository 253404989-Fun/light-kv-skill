# LIGHT KV

LIGHT KV is a maintainable, reference-first AI design Skill for high-end enterprise technology key visuals.

It is a design decision system, not a single prompt. It helps compatible Agents parse a Brief, lock authorized copy and canvas dimensions, retrieve visual structures, choose `Adapt → Recompose → Explore`, avoid low-quality template technology aesthetics, and audit production or extension readiness.

Current public release: `1.0.0-rc.1`.

## Principles

- Beauty First
- Reference First
- Adapt → Recompose → Explore
- Core Aesthetic Parents
- Generative Reference Library
- Copy Whitelist: do not add text the user did not provide
- Canvas Lock: obey the requested output dimensions
- No “淘宝科技感”: avoid HUD, code rain, glowing chips, random particles, future cities, portals, cheap 3D, and generic future slogans

## Public Package Scope

This repository is the public-safe edition. Its Reference Library is metadata-only: it retains composition, light, material, color, preserve, avoid, and failure-pattern logic, but excludes the private third-party source images and internal high-resolution test outputs.

This distinction matters:

- `PLAN` and `AUDIT` remain fully usable.
- Copy, canvas, strategy, typography, and extension gates remain fully usable.
- `GENERATE` requires an image-generation capability on the host Agent.
- Visual calibration is strongest when the user also supplies owned or licensed References through a local Reference Profile.

See `references/reference-profile-guide.md` before adding images.

## Install

### Codex from GitHub

Place this repository at `~/.codex/skills/light-kv`, or install it from your GitHub repository with the Codex skill installer. Private repositories require the recipient to have repository access and authenticated Git credentials.

Start a new Codex task after installation, then invoke:

```text
Use $light-kv to plan a 3840 × 2160 enterprise AI conference KV.
Only use this copy: “先进计算论坛”.
```

### Other Agent Platforms

Use a platform that supports an Agent Skill directory or can load `SKILL.md` plus its relative files. The host must preserve the directory structure. Image generation and local image inspection are optional capabilities; without them, use `PLAN` or `AUDIT` mode.

## Structure

```text
light-kv/
├── SKILL.md
├── agents/openai.yaml
├── core/
├── references/
└── tests/
```

## Rights and Safety

No private third-party Reference images are included. Do not add artwork unless you own it, hold a suitable license, or have explicit permission for the intended use. Reference copy, logos, credits, and watermarks never enter the Copy Whitelist.

Generated-output rights and usage restrictions depend on the generation service, user inputs, and applicable law. Review them before commercial publication.

## License

The Skill instructions, metadata, and repository documentation are released under the MIT License. User-supplied and generated visual assets are not automatically covered by that license.
