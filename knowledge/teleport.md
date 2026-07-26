---
name: Roblox Teleportation
description: Use when moving players between places, servers, or experiences.
---

# Roblox Teleportation

## Purpose

Use this module for server travel and cross-place flow.

## Procedure

1. Decide the travel reason.
2. Preserve the state the player needs after travel.
3. Validate the destination.
4. Handle failure cleanly.
5. Test the journey from start to finish.

## Rules

- Do not teleport without a clear purpose.
- Keep the destination predictable.
- Ensure data needed after travel is stored safely.
- Handle disconnects and retries gracefully.

## Review checklist

- The destination is valid.
- State survives the travel path.
- Failures are handled.
- The user can understand what happened.
