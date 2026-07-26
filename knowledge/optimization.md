---
name: Roblox Optimization
description: Use when improving FPS, memory use, streaming, physics cost, or runtime performance.
---

# Roblox Optimization

## Purpose

Use this module for performance work.

## Procedure

1. Find the real bottleneck before changing code.
2. Measure the impact of the change.
3. Remove unnecessary work first.
4. Reduce allocations, replication, and overdraw.
5. Recheck after the change.

## Common targets

- too many parts,
- too many active scripts,
- too many remote calls,
- expensive loops,
- unnecessary physics,
- oversized UI trees,
- wasteful asset use.

## Rules

- Optimize the hot path, not guesswork.
- Prefer structural improvements over micro-tuning.
- Use streaming and asset discipline when the map is large.
- Keep expensive work out of per-frame code unless absolutely necessary.

## Review checklist

- The bottleneck was identified.
- The fix is measurable.
- The system still behaves correctly.
- The performance improvement is stable under playtest.
