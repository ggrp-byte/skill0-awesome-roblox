---
name: Roblox Service Lifecycle
description: Use when defining initialization, runtime, shutdown, and reset behavior for services.
---

# Roblox Service Lifecycle

## Purpose

Use this module when a service needs a clear life cycle.

## Lifecycle

- initialize: set up dependencies and static state,
- start: begin runtime work,
- stop: end runtime work,
- reset: clear transient state.

## Procedure

1. Define what happens in each phase.
2. Keep initialization separate from active runtime logic.
3. Make shutdown safe to call.
4. Make reset safe to repeat.
5. Test the service through the full cycle.

## Rules

- Do not start work before the service is ready.
- Do not mix startup and runtime behavior in one unclear block.
- Keep transitions explicit.
- Make teardown predictable.

## Review checklist

- The phases are documented.
- Startup is deterministic.
- Shutdown is safe.
- Reset works without corrupting state.
