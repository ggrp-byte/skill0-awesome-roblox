---
name: NPC Systems
description: Use when creating NPC behavior, pathfinding, dialogue, combat AI, or companion logic.
---

# NPC Systems

## Purpose

Use this module for non-player characters, enemies, companions, and scripted actors.

## Procedure

1. Define the NPC's job.
2. Choose the simplest behavior model that fits the job.
3. Separate movement, decision-making, animation, and dialogue.
4. Keep server control over impactful NPC actions.
5. Test behavior in a crowded environment.

## Patterns

- Use state machines for straightforward behavior.
- Use pathfinding for navigation when needed.
- Use dialogue trees for conversation-heavy NPCs.
- Use cooldowns and range checks for combat actions.

## Rules

- NPCs should not consume excessive CPU.
- Avoid recalculating path data more often than needed.
- Keep interaction prompts clear and safe.
- Do not let NPCs grant rewards without server validation.

## Review checklist

- NPC behavior is understandable.
- Movement is stable.
- The NPC cannot get stuck forever.
- Combat and rewards are server-controlled.
