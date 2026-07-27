---
name: Roblox Feature Flags
description: Use when gating incomplete, experimental, or risky behavior behind explicit enablement.
---

# Roblox Feature Flags

## Purpose

Use this module when behavior must be switched on gradually or kept behind a controlled gate.

## Procedure

1. Identify the risky or incomplete behavior.
2. Decide who can enable it.
3. Keep the default state safe.
4. Make the flag name obvious.
5. Test both flag states.

## Rules

- A disabled flag must leave the game in a safe state.
- Flag logic should be easy to remove later.
- Do not hide fundamental gameplay decisions behind ambiguous flags.
- Keep flag access controlled and documented.

## Review checklist

- The default state is safe.
- Both branches were tested.
- The flag is easy to find.
- The feature can be removed cleanly later.
