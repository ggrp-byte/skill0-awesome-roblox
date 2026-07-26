---
name: Roblox Service Boundaries
description: Use when deciding how server services, client controllers, and shared modules should interact.
---

# Roblox Service Boundaries

## Purpose

Use this module to keep the project divided into clear responsibilities.

## Boundaries

- Server services own authority, validation, and persistent state.
- Client controllers own input, local presentation, and temporary view state.
- Shared modules own definitions, constants, and safe utility code.

## Procedure

1. Identify the responsibility.
2. Assign a single owner.
3. Expose a minimal public API.
4. Keep side effects inside the owning layer.
5. Document what may and may not call the service.

## Rules

- A module should have one primary owner.
- Do not mix UI and server authority in the same file.
- Keep shared code free of hidden game decisions.
- Make the public API smaller than the internal implementation.

## Review checklist

- Ownership is clear.
- The API is narrow.
- The module does not leak responsibilities.
- The boundary matches the container it lives in.
