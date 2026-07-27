---
name: Roblox Cleanup
description: Use when releasing connections, destroying temporary objects, and tearing down runtime state safely.
---

# Roblox Cleanup

## Purpose

Use this module when temporary runtime work must be removed cleanly.

## Procedure

1. Track what the feature creates.
2. Define what must be disconnected, destroyed, or reset.
3. Clean up on completion, cancellation, and failure.
4. Confirm cleanup happens more than once if needed without breaking.
5. Re-test after teardown changes.

## Rules

- Never leave temporary listeners running forever.
- Never keep dead state alive just because it is convenient.
- Cleanup should be predictable and safe to repeat.
- Remove temporary assets from the live game when they are no longer needed.

## Review checklist

- Temporary objects are cleaned up.
- Connections are disconnected.
- Failed flows still clean up.
- Repeated cleanup does not corrupt the system.
