---
name: Roblox Messaging
description: Use when broadcasting events across server systems or coordinating game state changes.
---

# Roblox Messaging

## Purpose

Use this module when multiple server-side systems need to react to the same event.

## Procedure

1. Define the event meaning.
2. Decide who emits it and who consumes it.
3. Keep the payload small and explicit.
4. Avoid using messaging for trivial local logic.
5. Verify that listeners still behave correctly when events arrive in bursts.

## Rules

- Use messages for coordination, not for replacing clean API design.
- Keep event names stable and understandable.
- Do not leak secrets through shared messages.

## Review checklist

- The event has a single purpose.
- The payload is minimal.
- Multiple consumers do not cause side effects.
- The system still works if messages repeat or arrive late.
