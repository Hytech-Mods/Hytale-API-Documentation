# Server Package Structure

This document describes the class package structure found in `HytaleServer.jar`.

## Top-Level Packages

| Package | Description |
|---------|-------------|
| `com.hypixel.hytale.assetstore` | Asset storage and caching |
| `com.hypixel.hytale.builtin` | Built-in game functionality |
| `com.hypixel.hytale.codec` | Data encoding/decoding |
| `com.hypixel.hytale.common` | Shared common utilities |
| `com.hypixel.hytale.component` | ECS component system |
| `com.hypixel.hytale.event` | Event system |
| `com.hypixel.hytale.function` | Functional utilities |
| `com.hypixel.hytale.logger` | Logging (HytaleLogger) |
| `com.hypixel.hytale.math` | Math utilities |
| `com.hypixel.hytale.metrics` | Performance metrics |
| `com.hypixel.hytale.plugin` | Plugin/mod system |
| `com.hypixel.hytale.procedurallib` | Procedural generation library |
| `com.hypixel.hytale.protocol` | Network protocol |
| `com.hypixel.hytale.registry` | Game registries |
| `com.hypixel.hytale.server` | Server implementation |
| `com.hypixel.hytale.sneakythrow` | Exception handling utilities |
| `com.hypixel.hytale.storage` | Data storage |
| `com.hypixel.hytale.unsafe` | Low-level operations |

## Server Subsystems

Key packages under `com.hypixel.hytale.server`:

| Package | Description |
|---------|-------------|
| `server.core` | Core server API (commands, plugins, entities) |
| `server.npc` | NPC AI and behavior systems |
| `server.spawning` | Entity spawning systems |
| `server.worldgen` | World generation (biomes, caves, prefabs) |
| `server.flock` | Flocking/group behavior |
| `server.migrations` | Data migrations |

## Entry Points

| Class | Purpose |
|-------|---------|
| `com.hypixel.hytale.Main` | Server entry point |
| `com.hypixel.hytale.LateMain` | Late initialization |

## Plugin System

| Class | Purpose |
|-------|---------|
| `plugin.early.EarlyPluginLoader` | Early plugin loading |
| `plugin.early.ClassTransformer` | Bytecode transformation |
| `plugin.early.TransformingClassLoader` | Custom class loading |
