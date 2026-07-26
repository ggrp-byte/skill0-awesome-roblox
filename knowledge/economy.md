---
name: Roblox Economy
description: Use when designing currencies, shops, rewards, sinks, progression pacing, or monetization loops.
---

# Roblox Economy

## Purpose

Use this module for any system that gives, spends, or balances value.

## Procedure

1. Define the resource.
2. Define how the player earns it.
3. Define how the player spends it.
4. Define what prevents runaway inflation.
5. Test the loop with a small progression path.

## Rules

- Keep currencies simple.
- Make rewards server-authoritative.
- Balance sinks against sources.
- Avoid confusing multiple currencies unless the design truly needs them.
- Tie progression pacing to the intended session length.

## Review checklist

- The resource has a clear purpose.
- The loop is understandable.
- The server controls the critical state.
- Progression does not explode too quickly.
