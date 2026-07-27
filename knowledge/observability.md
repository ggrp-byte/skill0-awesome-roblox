---
name: Roblox Observability
description: Use when adding logging, metrics, debug signals, tracing, or runtime visibility.
---

# Roblox Observability

## Purpose

Use this module when a system needs to be inspected during development or in production-like testing.

## Procedure

1. Decide what must be visible.
2. Choose the smallest useful signal.
3. Log meaningful events and failures.
4. Keep production noise low.
5. Verify that the signals actually help diagnose the problem.

## Rules

- Do not log secrets.
- Do not flood the output with redundant lines.
- Keep messages short and actionable.
- Use the smallest set of observations that answers the real question.

## Review checklist

- Important transitions are visible.
- Failures are diagnosable.
- The logs are not noisy.
- The observability layer does not change game behavior.
