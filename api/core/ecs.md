# Entity Component System (ECS)

Hytale uses an Entity Component System architecture for game objects.

## Package: `com.hypixel.hytale.component`

### Core Classes

| Class | Description |
|-------|-------------|
| `Component` | Base component class |
| `ComponentType` | Component type identifier |
| `ComponentRegistry` | Registry of components |
| `ComponentAccessor` | Access component data |
| `Holder` | **Entity holder reference** - safe entity access |
| `Ref` | Reference to entity |
| `WeakComponentReference` | Weak reference to component |

### Archetypes

| Class | Description |
|-------|-------------|
| `Archetype` | Entity archetype (component combination) |
| `ArchetypeChunk` | Chunk of entities with same archetype |

### Queries

| Class | Description |
|-------|-------------|
| `Query` | Base query class |
| `AndQuery` | Match all components |
| `OrQuery` | Match any component |
| `NotQuery` | Exclude components |
| `AnyQuery` | Any match |
| `ExactArchetypeQuery` | Exact archetype match |
| `ReadWriteArchetypeQuery` | Read/write access query |

### Resources

| Class | Description |
|-------|-------------|
| `Resource` | ECS resource (singleton data) |
| `ResourceType` | Resource type identifier |
| `IResourceStorage` | Resource storage interface |

### Systems

| Class | Description |
|-------|-------------|
| `System` | Base system class |
| `ISystem` | System interface |
| `SystemGroup` | Group of systems |
| `SystemType` | System type identifier |
| `QuerySystem` | System with query |
| `EventSystem` | Event-driven system |
| `TickingSystem` | Runs every tick |
| `DelayedSystem` | Delayed execution |
| `HolderSystem` | System using holders |

### Ticking Systems

| Class | Description |
|-------|-------------|
| `TickableSystem` | Can be ticked |
| `EntityTickingSystem` | Per-entity ticking |
| `ArchetypeTickingSystem` | Per-archetype ticking |
| `DelayedEntitySystem` | Delayed entity processing |

### Events

| Class | Description |
|-------|-------------|
| `EcsEvent` | ECS event |
| `CancellableEcsEvent` | Cancellable ECS event |
| `EntityEventSystem` | Entity event handling |
| `WorldEventSystem` | World event handling |

### Dependencies

| Class | Description |
|-------|-------------|
| `Dependency` | System dependency |
| `DependencyGraph` | Dependency ordering |
| `Order` | Execution order |
| `OrderPriority` | Order priority |

### Spatial

| Class | Description |
|-------|-------------|
| `SpatialStructure` | Spatial indexing |
| `SpatialSystem` | Spatial queries |
| `KDTree` | KD-Tree implementation |
| `MortonCode` | Morton code for spatial |
