---
name: Roblox State Management
description: Use when deciding how runtime state should be stored, updated, reset, and shared across systems.
---

# Roblox State Management

## Purpose

Use this module for runtime state that drives gameplay or UI.

## Procedure

1. Identify the source of truth.
2. Decide whether the state is session-only or persistent.
3. Keep mutations in one place.
4. Use clear state transitions.
5. Reset state cleanly when the session ends.

## Rules

- Do not scatter the same state across many modules.
- Do not let UI create authoritative state.
- Prefer explicit state objects over ad hoc globals.
- Keep state shapes stable and documented.

## Review checklist

- The state owner is clear.
- Transitions are predictable.
- Reset behavior is safe.
- The design is easy to test.
