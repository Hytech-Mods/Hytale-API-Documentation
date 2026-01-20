# NPC System Overview

Hytale uses a sophisticated AI system for NPCs with builders, blackboards, and behavior trees.

## Package: `com.hypixel.hytale.server.npc`

### Events

| Class | Description |
|-------|-------------|
| `AllNPCsLoadedEvent` | Fired when all NPCs are loaded |

### Animations

| Class | Description |
|-------|-------------|
| `animations.NPCAnimationSlot` | NPC animation slot |

## Builder System

### Package: `com.hypixel.hytale.server.npc.asset.builder`

The builder system creates NPC components from configuration.

| Class | Description |
|-------|-------------|
| `Builder` | Base builder interface |
| `BuilderBase` | Base builder implementation |
| `BuilderManager` | Manages builders |
| `BuilderContext` | Builder context |
| `BuilderFactory` | Creates builders |
| `BuilderComponent` | Component builder |
| `BuilderDescriptor` | Describes builder |
| `BuilderParameters` | Builder parameters |
| `Feature` | Feature definition |

### Expressions

| Class | Description |
|-------|-------------|
| `expression.BuilderExpression` | Base expression |
| `expression.BuilderExpressionDynamic` | Dynamic expression |
| `expression.BuilderExpressionDynamicBoolean` | Dynamic boolean |
| `expression.BuilderExpressionDynamicNumber` | Dynamic number |
| `expression.BuilderExpressionDynamicString` | Dynamic string |
| `expression.BuilderExpressionStaticBoolean` | Static boolean |
| `expression.BuilderExpressionStaticNumber` | Static number |

### Holders

| Class | Description |
|-------|-------------|
| `holder.AssetHolder` | Asset holder |
| `holder.BooleanHolder` | Boolean holder |
| `holder.IntHolder` | Integer holder |
| `holder.FloatHolder` | Float holder |
| `holder.DoubleHolder` | Double holder |
| `holder.EnumHolder` | Enum holder |

## Subsystems

- **Blackboard**: AI state storage and sharing
- **Decision Maker**: AI decision logic
- **Movement**: NPC pathfinding and movement
- **State Machine**: Behavior state management
- **Sensors**: Environment perception
