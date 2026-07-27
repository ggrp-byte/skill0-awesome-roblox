---
name: Roblox Configuration
description: Use when defining tunable values, environment switches, feature flags, and project settings.
---

# Roblox Configuration

## Purpose

Use this module for values that should be changed without rewriting the code logic.

## Procedure

1. List the values that are truly configurable.
2. Decide which values are shared, server-only, or client-visible.
3. Put related settings together.
4. Provide defaults.
5. Validate the configuration before use.

## Rules

- Do not scatter constants across unrelated files.
- Keep configuration predictable and documented.
- Do not expose secret values to the client.
- Avoid configuration that changes behavior without a clear reason.

## Review checklist

- The settings have one home.
- Defaults are clear.
- Invalid settings fail safely.
- The module does not become a dumping ground for arbitrary constants.
