---
name: Roblox Ultimate Agent
description: Entry point for a modular Roblox skill. Route tasks to the smallest matching module, then follow its procedure exactly.
---

# Roblox Ultimate Agent

Use this file only as the router.

## Operating rules

1. Read the user request and identify the narrowest matching module.
2. Load only the relevant knowledge, workflow, checklist, or example files.
3. Prefer the safest and simplest implementation that satisfies the request.
4. Keep Roblox authority on the server for gameplay, rewards, currency, inventory, and progress.
5. When asset usage is needed, route to `knowledge/creator-store.md` and apply its evaluation procedure.
6. When code is changed, validate against the security and testing checklists before finishing.

## Modules

- knowledge/
- workflows/
- checklists/
- examples/
- templates/
- scripts/

## Priority routing

- Luau code -> `knowledge/luau.md`
- Studio/project structure -> `knowledge/studio.md`
- Asset import or marketplace selection -> `knowledge/creator-store.md`
- Security, remotes, or data handling -> `knowledge/security.md`
- Networking and replication -> `knowledge/networking.md`
- UI work -> `knowledge/ui.md` and `workflows/build-ui.md`
- Building or level layout -> `knowledge/building.md`
- Terrain and natural spaces -> `knowledge/terrain.md`
- Animation -> `knowledge/animation.md`
- NPCs and AI -> `knowledge/npc.md`
- Performance -> `knowledge/optimization.md` and `workflows/optimize-game.md`
- Saving data -> `knowledge/datastore.md`
- Lighting and mood -> `knowledge/lighting.md`
- Input and controls -> `knowledge/input.md`
- Audio -> `knowledge/audio.md`
- Camera -> `knowledge/camera.md`
- Physics -> `knowledge/physics.md`
- Game design and pacing -> `knowledge/game-design.md`
- Economy and progression -> `knowledge/economy.md`
- Messaging -> `knowledge/messaging.md`
- Pathfinding -> `knowledge/pathfinding.md`
- Teleportation -> `knowledge/teleport.md`
- Tag-based discovery -> `knowledge/collectionservice.md`
- Remote patterns -> `knowledge/remote-patterns.md`
- Plugins -> `knowledge/plugins.md`
- Game creation -> `workflows/create-game.md`
- Debugging -> `workflows/debug-game.md`
- Publishing -> `knowledge/publishing.md` and `workflows/publish.md`
