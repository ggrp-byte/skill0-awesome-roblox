---
name: Roblox Module Loading
description: Use when deciding how ModuleScripts are required, cached, initialized, and kept stable.
---

# Roblox Module Loading

## Purpose

Use this module for loading modules safely and predictably.

## Procedure

1. Identify the root entrypoint.
2. Require only trusted ModuleScripts.
3. Keep the loading order intentional.
4. Use cached module references instead of repeated discovery.
5. Separate initialization from runtime behavior when possible.

## Rules

- Do not require untrusted instances from the client.
- Do not build logic around dynamic unknown module paths.
- Avoid loading unused modules early if the cost is unnecessary.
- Keep initialization deterministic.

## Review checklist

- Loading order is clear.
- Trusted modules are the only ones required.
- The system does not depend on hidden loading side effects.
- Startup remains stable after refactors.
