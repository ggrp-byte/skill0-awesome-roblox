---
name: Roblox Plugins
description: Use when building or using Studio plugins that automate editing, importing, or validation.
---

# Roblox Plugins

## Purpose

Use this module for Studio automation tools and reusable editor extensions.

## Procedure

1. Define the editor job the plugin must solve.
2. Keep the plugin narrow and predictable.
3. Validate all inputs and UI actions.
4. Avoid destructive actions without confirmation.
5. Test the plugin on a small project first.

## Rules

- Do not build a plugin that hides dangerous actions.
- Do not let a plugin silently rewrite unrelated content.
- Keep plugin UI simple and clear.
- Prefer explicit buttons over hidden automation.

## Review checklist

- The plugin solves one clear problem.
- The UI is understandable.
- The plugin does not corrupt unrelated content.
- The plugin behaves safely in Studio.
