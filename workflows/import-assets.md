---
name: Import Roblox Assets Workflow
description: Use when importing models, meshes, audio, textures, or plugins into a project.
---

# Import Roblox Assets Workflow

## Goal

Bring an external asset into the project safely and intentionally.

## Procedure

1. Identify the asset category and purpose.
2. Choose the lightest acceptable asset.
3. Import into a staging area first.
4. Inspect scripts, hierarchy, naming, and dependencies.
5. Remove anything unnecessary or suspicious.
6. Move the cleaned asset into the real project structure.

## Rules

- Never trust an imported asset before inspection.
- Never leave hidden scripts unexplained.
- Prefer editable project-owned assets over opaque bundles.

## Output expectation

State what was imported, what was removed, what remains to verify, and where the asset now lives.
