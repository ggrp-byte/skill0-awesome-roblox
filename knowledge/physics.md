---
name: Roblox Physics
description: Use when working with assemblies, constraints, network ownership, or physically simulated gameplay.
---

# Roblox Physics

## Purpose

Use this module for physically simulated objects and interactions.

## Procedure

1. Decide whether the mechanic needs physics at all.
2. Keep assemblies simple.
3. Control ownership intentionally.
4. Test under load and with multiple players.
5. Separate visual polish from simulation correctness.

## Rules

- Do not rely on client-owned physics for critical rewards.
- Keep assemblies lightweight.
- Avoid excessive loose parts when a simpler setup works.
- Treat physics as shared state that needs careful authority choices.

## Review checklist

- The simulation is stable.
- Ownership is correct.
- The mechanic cannot be abused through physics tricks.
- The cost is acceptable in multiplayer.
