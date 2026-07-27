---
name: Roblox Dependency Management
description: Use when deciding how modules depend on each other, how services are wired, and how initialization order works.
---

# Roblox Dependency Management

## Purpose

Use this module when one system needs another system to function.

## Procedure

1. List the dependencies the feature truly needs.
2. Decide which dependency is mandatory and which is optional.
3. Keep the dependency graph as flat as possible.
4. Prefer explicit wiring over hidden lookup tricks.
5. Test startup and shutdown order.

## Rules

- Avoid circular require chains.
- Avoid loading everything just because it exists.
- Keep dependencies stable and minimal.
- Prefer passing dependencies in explicitly when that keeps the design cleaner.
- Load only what the current task needs.

## Review checklist

- Dependencies are intentional.
- The graph does not contain avoidable cycles.
- Optional dependencies fail safely.
- Startup order is defined.
- The design is easy to reason about.
