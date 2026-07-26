---
name: Roblox Testing
description: Use when playtesting, regression testing, validating remotes, and checking game stability.
---

# Roblox Testing

## Purpose

Use this module before a feature is considered done.

## Procedure

1. Test the happy path.
2. Test failure paths.
3. Test spam, latency, disconnects, and repeated input where relevant.
4. Test with the intended number of players.
5. Re-run the test after fixes.

## Coverage

- gameplay flows,
- security checks,
- UI behavior,
- network behavior,
- save/load behavior,
- performance-sensitive features.

## Rules

- A feature is not finished until it survives the intended use and the common abuse paths.
- Do not trust a single successful playtest.
- Re-test after every meaningful change.

## Review checklist

- Core flow works.
- Edge cases were exercised.
- Failures are handled cleanly.
- The fix did not break another system.
