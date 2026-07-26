---
name: Roblox Security
description: Use when validating remotes, server authority, anti-exploit logic, or secure data handling.
---

# Roblox Security

## Purpose

Use this module for any system that could be abused by a client.

## Core rule

The server decides the truth for gameplay, rewards, currency, inventory, ownership, and progression.

## Required checks

1. Validate type and shape of every client message.
2. Validate player identity, distance, state, and cooldown.
3. Reject impossible values immediately.
4. Rate-limit repeated requests.
5. Never trust the client to grant itself value or access.

## Remote design

- Keep payloads small.
- Use one remote for one action.
- Do not expose secrets in replicated storage.
- Never let the client choose a server module path.
- Keep server responses minimal and explicit.

## Data safety

- Guard every save and load with validation.
- Never overwrite a valid save with empty failure data.
- Treat malformed data as hostile.
- Version every save schema.

## Anti-exploit review

Check for:

- duplicated rewards,
- spammed remotes,
- client-side authority,
- hidden script entry points,
- unsafe dynamic requires,
- trust in UI state.

## Completion rule

If a mechanic can be abused, it is not finished until the abuse path is closed.
