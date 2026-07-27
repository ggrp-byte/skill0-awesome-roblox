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
6. Choose the correct write API for the job.

## Rules

- Treat save data as untrusted until validated.
- Keep the stored shape predictable.
- Never rely on a single save attempt.
- Keep rewards idempotent so they cannot be granted twice.
- Use `pcall` around live DataStore operations.
- Prefer `UpdateAsync` when the change must merge safely with the current stored value.
- Use `SetAsync` only when replacing the stored value is the intended behavior.
- Respect request budgets and back off when the budget is low.
- Do not spam writes from frequent state changes.

## DataStore API notes

- `GetRequestBudgetForRequestType` can help you check remaining budget before a burst of operations.
- `UpdateAsync` is the safer default for server-side state that can be changed concurrently.
- `SetAsync` is simpler, but it overwrites the stored value directly.
- `pcall` is required so transient failures do not crash the workflow.
- Schema validation should happen before writing and after reading.

## Review checklist

- The schema is versioned.
- Loads are validated.
- Failed writes do not erase valid data.
- The system can recover after a partial failure.
- The budget-aware write strategy matches the feature.
