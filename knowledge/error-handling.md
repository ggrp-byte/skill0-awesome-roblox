---
name: Roblox Error Handling
description: Use when designing failure paths, fallbacks, logging, retries, and safe exits.
---

# Roblox Error Handling

## Purpose

Use this module when code can fail due to bad input, missing services, transient network issues, or unavailable data.

## Procedure

1. Identify the failure points before writing the implementation.
2. Decide which failures are recoverable and which are fatal.
3. Add a clear fallback for every recoverable failure.
4. Keep the failure path simple and observable.
5. Re-test the failure path after the fix.

## Rules

- Do not hide errors that affect gameplay correctness.
- Do not continue with partial state when the feature requires full success.
- Prefer explicit fallback behavior over silent failure.
- Keep logs useful but concise.
- Fail safely when input or state is invalid.

## Review checklist

- Failure points are named.
- Recovery is defined.
- Fatal errors stop the dangerous path.
- Recoverable errors have a fallback.
- The user-facing behavior is still understandable.
