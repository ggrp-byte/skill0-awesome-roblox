---
name: Roblox Networking
description: Use when designing replication, RemoteEvents, RemoteFunctions, and client-server flow.
---

# Roblox Networking

## Purpose

Use this module for anything that crosses the client-server boundary.

## Design rules

1. Decide whether the action belongs on the client, the server, or both.
2. Prefer server-authoritative gameplay.
3. Use the client for input, presentation, and prediction only when necessary.
4. Keep replication minimal and intentional.
5. Send only the data the receiver truly needs.

## RemoteEvent rules

- One action per remote.
- Keep arguments typed and small.
- Validate all inputs on the server.
- Include cooldowns and ownership checks.
- Return only the state required to refresh the client.

## RemoteFunction rules

- Use only when a synchronous response is necessary.
- Avoid heavy work inside the callback.
- Never let the client drive expensive server logic.

## Replication rules

- Do not replicate every frame unless the system is intentionally realtime.
- Prefer state changes over constant chatter.
- Batch updates when possible.
- Use explicit server messages for meaningful transitions.

## Review checklist

- The client cannot forge a meaningful advantage.
- The server validates every sensitive action.
- Network traffic is limited and understandable.
- Multiplayer behavior still works with latency.
