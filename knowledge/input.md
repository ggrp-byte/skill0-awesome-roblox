---
name: Roblox Input
description: Use when handling keyboard, mouse, touch, controller, or action bindings.
---

# Roblox Input

## Purpose

Use this module for player control and interaction input.

## Procedure

1. Identify the supported input devices.
2. Map the action to clear controls.
3. Keep input handling separated from gameplay effects.
4. Respect accessibility and platform differences.
5. Test the action with every supported device type.

## Rules

- Do not hard-code only one device when the game supports more.
- Keep input feedback immediate.
- Avoid conflicting binds.
- Keep client input as a request, not a final authority.

## Review checklist

- The control scheme is understandable.
- All intended devices work.
- The interaction feels responsive.
- The input path does not bypass validation.
