---
name: Roblox Remote Patterns
description: Use when designing RemoteEvents, RemoteFunctions, and request/response patterns between client and server.
---

# Roblox Remote Patterns

## Purpose

Use this module for structured client-server communication.

## Procedure

1. Define the action.
2. Define the allowed input.
3. Define the server checks.
4. Define the minimal response.
5. Add a throttle or cooldown.

## Rules

- One remote should represent one clear action.
- Never trust the client to provide the final truth.
- Keep payloads small and explicit.
- Avoid generic catch-all remotes when a narrow one is possible.

## Review checklist

- The remote is narrow.
- Validation exists.
- Cooldowns exist.
- The response is minimal.
- The server remains authoritative.
