# World Generation Overview

Hytale's procedural world generation system.

## Package: `com.hypixel.hytale.server.worldgen`

### Core Resources

| Class | Description |
|-------|-------------|
| `ChunkGeneratorResource` | Chunk generator resource |
| `BiomeDataSystem` | Biome data ECS system |

### Benchmark

| Class | Description |
|-------|-------------|
| `benchmark.ChunkWorldgenBenchmark` | Performance benchmark |

## Biome System

### Package: `com.hypixel.hytale.server.worldgen.biome`

| Class | Description |
|-------|-------------|
| `Biome` | Base biome definition |
| `CustomBiome` | Custom biome |
| `TileBiome` | Tile-based biome |
| `BiomeInterpolation` | Biome blending |
| `BiomePatternGenerator` | Pattern generation |
| `CustomBiomeGenerator` | Custom biome generator |

## Cave System

### Package: `com.hypixel.hytale.server.worldgen.cave`

| Class | Description |
|-------|-------------|
| `Cave` | Cave definition |
| `CaveGenerator` | Cave generation |
| `CaveType` | Type of cave |
| `CaveNodeType` | Node types |
| `CavePrefabPlacement` | Prefab placement |

### Cave Shapes

| Class | Description |
|-------|-------------|
| `shape.CaveNodeShape` | Cave shape interface |
| `shape.CylinderCaveNodeShape` | Cylinder shape |
| `shape.EllipsoidCaveNodeShape` | Ellipsoid shape |
| `shape.PipeCaveNodeShape` | Pipe shape |
| `shape.PrefabCaveNodeShape` | Prefab-based shape |
| `shape.TetrahedronCaveNodeShape` | Tetrahedron shape |

### Distorted Shapes

| Class | Description |
|-------|-------------|
| `shape.distorted.DistortedShape` | Distorted shape base |
| `shape.distorted.DistortedCylinderShape` | Distorted cylinder |
| `shape.distorted.DistortedEllipsoidShape` | Distorted ellipsoid |
| `shape.distorted.DistortedPipeShape` | Distorted pipe |
| `shape.distorted.ShapeDistortion` | Shape distortion |

## Chunk Generation

### Package: `com.hypixel.hytale.server.worldgen.chunk`

| Class | Description |
|-------|-------------|
| `ChunkGenerator` | Main chunk generator |
| `ChunkGeneratorExecution` | Generation execution |
| `BlockPriorityChunk` | Block priority |
| `HeightThresholdInterpolator` | Height interpolation |

### Populators

| Class | Description |
|-------|-------------|
| `populator.BlockPopulator` | Block population |
| `populator.CavePopulator` | Cave population |
| `populator.PrefabPopulator` | Prefab population |
| `populator.WaterPopulator` | Water population |

## Caching

| Class | Description |
|-------|-------------|
| `cache.ChunkGeneratorCache` | Chunk cache |
| `cache.CaveGeneratorCache` | Cave cache |
| `cache.CoordinateCache` | Coordinate cache |
| `cache.UniquePrefabCache` | Prefab cache |
