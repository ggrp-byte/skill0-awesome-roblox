---
name: Roblox DataStore
description: Use when saving player progress, settings, inventory, or persistent game state.
---

# Roblox DataStore

## Purpose

Use this module for persistent server-side data.

## Procedure

1. Define the save schema before writing code.
2. Version the data.
3. Validate data before load or save.
4. Handle failure paths with care.
5. Protect the good save from being replaced by bad data.

## Rules

- Treat save data as untrusted until validated.
- Keep the stored shape predictable.
- Never rely on a single save attempt.
- Keep rewards idempotent so they cannot be granted twice.

## Review checklist

- The schema is versioned.
- Loads are validated.
- Failed writes do not erase valid data.
- The system can recover after a partial failure.
