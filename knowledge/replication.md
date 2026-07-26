---
name: Roblox Replication
description: Use when deciding what state should exist on the server, what should be mirrored to clients, and how updates should flow.
---

# Roblox Replication

## Purpose

Use this module for shared game state that appears on more than one machine.

## Procedure

1. Decide whether the state is authoritative, mirrored, or local-only.
2. Choose the owner of the state.
3. Define the minimal data that must be visible to each side.
4. Update clients only when the state actually changes.
5. Test with latency and multiple players.

## Rules

- Keep sensitive state server-only.
- Do not replicate unnecessary detail.
- Prefer explicit state changes over constant chatter.
- Keep replicated values simple and predictable.

## Review checklist

- The owner of each state piece is known.
- Clients only receive what they need.
- The mechanic still works under delay.
- The update path is easy to understand.
