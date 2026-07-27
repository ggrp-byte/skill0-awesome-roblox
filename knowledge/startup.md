---
name: Roblox Startup
description: Use when defining initialization order, bootstrap logic, service startup, and runtime readiness.
---

# Roblox Startup

## Purpose

Use this module when the project needs a predictable startup sequence.

## Procedure

1. Identify the boot entrypoint.
2. Initialize dependencies in a known order.
3. Separate setup from runtime behavior.
4. Confirm readiness before exposing the feature.
5. Re-test startup after each structural change.

## Rules

- Startup must be deterministic.
- Do not rely on hidden side effects.
- Fail early when a required system is missing.
- Keep initialization small and readable.

## Review checklist

- The startup order is documented.
- Required dependencies are ready before use.
- The feature can report readiness clearly.
- Startup still works after refactors.
