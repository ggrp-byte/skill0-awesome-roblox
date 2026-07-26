---
name: Roblox Project Architecture
description: Use when deciding folder layout, module boundaries, service ownership, and how the project is organized overall.
---

# Roblox Project Architecture

## Purpose

Use this module for the overall structure of the project before feature work begins.

## Core layout

- `ServerScriptService` for server authority and sensitive logic.
- `StarterPlayer` for client-side control and presentation.
- `StarterGui` for UI entry points.
- `ReplicatedStorage` for safe shared modules, definitions, and non-secret assets.
- `ServerStorage` for server-only assets and hidden implementation details.
- `Workspace` for live world instances and runtime objects.

## Procedure

1. Identify which side owns the truth for the feature.
2. Decide where the code should live.
3. Separate presentation, shared definitions, and authority.
4. Keep each module focused on one job.
5. Avoid circular dependencies.
6. Group related systems into named folders.

## Rules

- Do not put secrets in replicated locations.
- Do not let client code decide server ownership.
- Keep the tree easy to navigate.
- Prefer clear names over clever names.
- Use consistent patterns across systems.

## Review checklist

- Ownership is obvious.
- Folders match the architecture.
- Shared code is actually safe to share.
- Nothing critical lives in the wrong container.
