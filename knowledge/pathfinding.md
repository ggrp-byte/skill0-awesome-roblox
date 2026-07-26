---
name: Roblox Pathfinding
description: Use when moving NPCs or agents around obstacles using navigation logic.
---

# Roblox Pathfinding

## Purpose

Use this module when an agent must move intelligently through the world.

## Procedure

1. Define the movement goal.
2. Check whether simple movement is enough.
3. Use pathfinding only when the navigation problem needs it.
4. Recompute paths only when the environment or goal changes.
5. Handle blocked paths and fallback states.

## Rules

- Do not overcompute paths.
- Keep path logic server-aware when movement matters for gameplay.
- Add stuck recovery for long routes.
- Keep navigation behavior understandable.

## Review checklist

- The agent reaches the destination reliably.
- Blocked paths are handled.
- The system is not recalculating too often.
- The movement looks stable in playtest.
