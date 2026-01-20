# Hytale API Documentation

Welcome to the Hytale modding API documentation by **Hytech**.

## Quick Start

1. **[Plugin System](api/core/plugin-system.md)** - Create your first mod
2. **[Event System](api/core/event-system.md)** - Handle game events
3. **[Messaging](api/core/messaging.md)** - Send messages to players

## API Status Legend

All API documentation uses validation status markers:

| Status | Meaning |
|--------|---------|
| 🟢 **Verified** | Tested in-game, confirmed working |
| 🔴 **Requires Validation** | Discovered from decompilation, not yet tested |

## Documentation Sections

### Core APIs
Essential APIs for mod development:
- [Plugin System](api/core/plugin-system.md) - JavaPlugin base class
- [Event System](api/core/event-system.md) - EventBus and handlers
- [Messaging](api/core/messaging.md) - Player messaging
- [Logging](api/core/logging.md) - HytaleLogger

### Game Systems
- [Commands](api/commands/README.md) - Command system
- [Entities](api/entities/README.md) - Entities and players
- [Items & Inventory](api/items/README.md) - ItemContainer API

### World & NPCs
- [World Generation](api/worldgen/README.md) - Biomes, caves, chunks
- [NPC AI](api/npc/README.md) - NPC behavior
- [Spawning](api/spawning/README.md) - Entity spawning

### Utilities
- [Math](api/math/README.md) - Vectors, shapes, raycasting
- [Common](api/common/README.md) - Shared utilities

## Reference

- **[Complete Class List](complete-class-list.md)** - All 5,218 server classes
- **[File Structure](file-structure.md)** - Hytale installation layout
- **[Server Packages](server-packages.md)** - Package overview

## Important Notes

> **⚠️ Color Codes**: Minecraft-style color codes (`§`) do NOT work in Hytale.

> **⚠️ Deprecated APIs**: Some APIs like `getPlayer()` are deprecated but still functional.

---

*Documentation by [Hytech-Mods](https://github.com/Hytech-Mods)*
