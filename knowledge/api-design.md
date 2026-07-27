---
name: Roblox API Design
description: Use when exposing functions, services, modules, and public interfaces to other parts of the project.
---

# Roblox API Design

## Purpose

Use this module when a system needs a public interface.

## Procedure

1. Define the smallest useful interface.
2. Identify the inputs, outputs, and failure modes.
3. Keep public surface area narrow.
4. Make names self-explanatory.
5. Separate public calls from internal helpers.

## Rules

- Do not expose more than the consumer needs.
- Do not return mutable state unless that is intentional and safe.
- Keep signatures stable when possible.
- Make error behavior predictable.

## Review checklist

- The API is minimal.
- The API is obvious to use.
- Internal details stay hidden.
- The interface stays stable across refactors.
