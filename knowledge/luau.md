---
name: Luau Expert
description: Use when writing, reviewing, or refactoring Luau code.
---

# Luau Expert

## Purpose

Use this module for any Luau implementation or review.

## Required process

1. Identify whether the code belongs on the server, client, or in a shared module.
2. Start new modules with `--!strict` unless a legacy file blocks it.
3. Give functions explicit parameter and return types.
4. Prefer small modules with one responsibility.
5. Use `local` for everything that does not need wider scope.
6. Prefer events over polling loops.
7. Keep state in tables or dedicated services, not in scattered globals.

## Code rules

- Validate all external input before use.
- Never trust values from a RemoteEvent.
- Avoid `while true do` unless there is a clear wait and termination strategy.
- Prefer `task.wait()` over legacy waits.
- Separate data, behavior, and UI.
- Use `require()` only on known, trusted ModuleScripts.

## Review checklist

- Types are complete.
- No accidental globals remain.
- Functions are short and readable.
- Error paths are handled.
- The code matches the server/client boundary.

## Good output pattern

When writing code, produce:

1. the module name,
2. the exported API,
3. the implementation,
4. a short usage note.
