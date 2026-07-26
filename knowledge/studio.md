---
name: Roblox Studio Workflow
description: Use when operating Roblox Studio, organizing project structure, or editing game content.
---

# Roblox Studio Workflow

## Purpose

Use this module when the work happens inside Roblox Studio.

## Procedure

1. Inspect the current place and identify the affected systems.
2. Keep the project structure predictable.
3. Place reusable logic in ModuleScripts and service scripts in the correct containers.
4. Separate UI, gameplay, and shared data.
5. Run a quick playtest after each meaningful change.

## Layout rules

- Server-owned logic belongs in server-side containers.
- UI and input logic belong in client-side containers.
- Shared definitions belong in shared modules only when they are safe for clients to see.
- Avoid mixing prototype code with production folders.

## Studio habits

- Name instances clearly.
- Group related assets together.
- Keep temporary experiments isolated.
- Reuse existing folders before creating new ones.

## Finish criteria

The job is not done until the project still opens cleanly, the modified systems run, and the file tree remains understandable.
