---
name: Roblox Versioning
description: Use when evolving save schemas, module contracts, or project structure without breaking older data or workflows.
---

# Roblox Versioning

## Purpose

Use this module when a change must remain compatible with older data or older project assumptions.

## Procedure

1. Assign a version number or version field.
2. Define what changes are backward-compatible.
3. Define how old data will be upgraded.
4. Keep migrations explicit.
5. Test both old and new shapes.

## Rules

- Never assume all data is new.
- Never silently change a schema without a migration path.
- Keep compatibility behavior documented.
- Prefer additive changes when possible.

## Review checklist

- Versions are tracked.
- Migrations exist where needed.
- Old data still loads or fails safely.
- The new contract is documented.
