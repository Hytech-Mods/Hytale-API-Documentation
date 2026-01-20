# Spawning System

Entity spawning and spawn control.

## Package: `com.hypixel.hytale.server.spawning`

### Core Classes

| Class | Description |
|-------|-------------|
| `SpawningPlugin` | Spawning plugin |
| `SpawningContext` | Spawn context |
| `ISpawnable` | Spawnable interface |
| `ISpawnableWithModel` | Spawnable with model |
| `SpawnTestResult` | Spawn test result |
| `SpawnRejection` | Spawn rejection |
| `LoadedNPCEvent` | NPC loaded event |

### Commands

| Class | Description |
|-------|-------------|
| `commands.SpawnCommand` | Spawn command |
| `commands.SpawnBeaconsCommand` | Beacon spawns |
| `commands.SpawnMarkersCommand` | Spawn markers |
| `commands.SpawnPopulateCommand` | Populate spawn |
| `commands.SpawnStatsCommand` | Spawn stats |
| `commands.SpawnSuppressionCommand` | Suppression |

### Beacons

| Class | Description |
|-------|-------------|
| `beacons.SpawnBeacon` | Spawn beacon |
| `beacons.SpawnBeaconSystems` | Beacon systems |
| `beacons.InitialBeaconDelay` | Initial delay |

### Controllers

| Class | Description |
|-------|-------------|
| `controllers.SpawnController` | Main controller |
| `controllers.BeaconSpawnController` | Beacon controller |
| `controllers.SpawnControllerSystem` | Controller ECS system |
| `controllers.SpawnJobSystem` | Job system |

### Managers

| Class | Description |
|-------|-------------|
| `managers.SpawnManager` | Spawn manager |
| `managers.BeaconSpawnManager` | Beacon manager |

### Spawn Markers

| Class | Description |
|-------|-------------|
| `spawnmarkers.SpawnMarkerEntity` | Marker entity |
| `spawnmarkers.SpawnMarkerSystems` | Marker systems |
| `blockstates.SpawnMarkerBlockState` | Block state |

### NPC Spawns

| Class | Description |
|-------|-------------|
| `assets.spawns.config.NPCSpawn` | NPC spawn config |
| `assets.spawns.config.BeaconNPCSpawn` | Beacon NPC spawn |
| `assets.spawns.config.WorldNPCSpawn` | World NPC spawn |

### Suppression

| Class | Description |
|-------|-------------|
| `suppression.component.SpawnSuppressionComponent` | Suppression component |
| `suppression.component.ChunkSuppressionEntry` | Chunk suppression |
