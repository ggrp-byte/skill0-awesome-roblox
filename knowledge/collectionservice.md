---
name: Roblox CollectionService
description: Use when tagging, grouping, or discovering related instances at runtime.
---

# Roblox CollectionService

## Purpose

Use this module for tagging and discovering runtime groups of objects.

## Procedure

1. Decide whether tags are the right grouping tool.
2. Define the tags clearly.
3. Keep tag meaning stable.
4. Use tags to simplify discovery, not to hide architecture.
5. Test additions and removals of tagged instances.

## Rules

- Tags should be descriptive and consistent.
- Do not use tags as a replacement for good data models.
- Keep tag-based logic predictable.
- Clean up tag-linked behavior when instances are removed.

## Review checklist

- The tags have one clear purpose.
- Runtime discovery is reliable.
- Removing a tagged object does not break the game.
- The pattern is easier than manual scanning.
