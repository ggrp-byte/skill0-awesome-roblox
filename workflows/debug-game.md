---
name: Debug Roblox Game Workflow
description: Use when diagnosing errors, broken systems, or unexpected gameplay behavior.
---

# Debug Roblox Game Workflow

## Goal

Find the real cause of a failure and fix it without creating new issues.

## Procedure

1. Reproduce the problem.
2. Narrow the scope.
3. Inspect logs, code paths, and data flow.
4. Identify the smallest broken assumption.
5. Fix the cause, not only the symptom.
6. Re-test the original issue and nearby paths.

## Rules

- Do not guess at the fix before finding the cause.
- Do not change unrelated systems unless the evidence demands it.
- Record what was broken and what was changed.

## Output expectation

State the symptom, the cause, the fix, and the verification step.
