---
name: Creator Store Asset Selection
description: Use when searching, evaluating, or importing Roblox Creator Store and Toolbox assets.
---

# Creator Store Asset Selection

## Purpose

Use this module whenever the task needs an external Roblox asset.

## Procedure

1. Define the asset type first: model, mesh, animation, sound, UI component, plugin, or reference material.
2. Search the Creator Store or Toolbox for the simplest asset that satisfies the requirement.
3. Prefer assets that are clean, lightweight, and easy to inspect.
4. Reject assets that depend on hidden behavior, unnecessary scripts, or unnecessary complexity.
5. After import, inspect every script, module, and object tree before the asset is trusted.

## Selection rules

- Prefer official or well-maintained assets when available.
- Prefer fewer parts, fewer scripts, and clearer naming.
- Prefer assets that can be replaced with custom code later.
- Avoid assets that bundle unrelated gameplay logic.
- Avoid anything that introduces unclear remote traffic or opaque dependencies.

## Import rules

- Strip unneeded scripts before the asset reaches production.
- Reparent imported content into the correct project folder.
- Convert placeholder assets into project-owned assets when needed.
- Document every imported asset and why it was chosen.

## Safety review

Before the asset is accepted:

- inspect for suspicious requires,
- inspect for hidden connections,
- inspect for unwanted server code,
- inspect for performance cost,
- confirm the asset still matches the game design.

## Output expectation

The final answer should say what was selected, why it was selected, what was removed, and what still needs manual review.
