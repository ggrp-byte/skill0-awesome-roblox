---
name: Roblox UI
description: Use when building menus, HUDs, inventories, dialogs, and responsive interfaces.
---

# Roblox UI

## Purpose

Use this module for any player-facing interface.

## UI goals

- make the action obvious,
- make the state readable,
- make the layout responsive,
- make the interaction easy on keyboard, mouse, touch, and controller.

## Procedure

1. Define the exact player task.
2. Choose the smallest UI that supports that task.
3. Build from reusable components.
4. Keep spacing, text sizes, and alignment consistent.
5. Test the UI at multiple resolutions.

## Rules

- Never hide critical gameplay state behind tiny or unclear controls.
- Avoid over-animated interfaces that delay input.
- Keep UI data separate from gameplay logic.
- Use clear labels instead of guessing.
- Handle empty states, loading states, and errors.

## Review checklist

- Inputs are reachable.
- Text is readable.
- Layout does not break on smaller screens.
- Buttons do not overlap.
- UI state resets correctly.
