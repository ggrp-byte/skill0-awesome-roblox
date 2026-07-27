---
name: Roblox Compatibility
description: Use when preserving behavior across older clients, older saves, or mixed project versions.
---

# Roblox Compatibility

## Purpose

Use this module when a change must keep older behavior working or fail safely.

## Procedure

1. Identify what older clients or data still exist.
2. Decide what must stay stable.
3. Add compatibility handling before removing old paths.
4. Test old and new shapes together.
5. Remove old support only when it is safe.

## Rules

- Prefer additive changes.
- Keep compatibility explicit.
- Never assume the whole player base updates at once.
- Keep migration logic separate from the main happy path.

## Review checklist

- Old behavior is accounted for.
- The new path does not break old data.
- Compatibility code is documented.
- The system fails safely when it must reject old data.
