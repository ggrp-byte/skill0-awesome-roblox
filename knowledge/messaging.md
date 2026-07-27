---
name: Roblox Messaging
description: Use when coordinating events across server systems or when using MessagingService between servers.
---

# Roblox Messaging

## Purpose

Use this module for event-based coordination. It covers both internal server event buses and Roblox `MessagingService` when cross-server delivery is needed.

## Procedure

1. Decide whether the event is only inside one server or must cross server boundaries.
2. Choose the lightest mechanism that matches the scope.
3. Keep the payload small and explicit.
4. Verify repeat delivery, delayed delivery, and listener behavior.
5. Avoid using messaging for trivial local logic.

## Rules

- Use messages for coordination, not for replacing clean API design.
- Keep event names stable and understandable.
- Do not leak secrets through shared messages.
- If the feature uses `MessagingService`, respect its delivery and payload constraints.

## MessagingService notes

- `MessagingService` is for cross-server communication, not for local-only events.
- Payloads should be small; large payloads are not appropriate.
- Delivery can be delayed or duplicated in practical workflows, so handlers must be safe to repeat.
- For local server event buses, use the simplest internal event pattern available instead of `MessagingService`.

## Review checklist

- The event has a single purpose.
- The payload is minimal.
- Multiple consumers do not cause side effects.
- The system still works if messages repeat or arrive late.
- The scope matches the chosen transport.
