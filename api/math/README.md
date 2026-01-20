# Math Utilities

Mathematical utilities, vectors, shapes, and raycasting.

## Package: `com.hypixel.hytale.math`

### Core Types

| Class | Description |
|-------|-------------|
| `Mat4f` | 4x4 float matrix |
| `Quatf` | Float quaternion |
| `Vec2f` | 2D float vector |
| `Vec3f` | 3D float vector |
| `Vec4f` | 4D float vector |
| `Axis` | Axis enum |

### Vectors

| Class | Description |
|-------|-------------|
| `vector.Vector2d` | 2D double vector |
| `vector.Vector2i` | 2D int vector |
| `vector.Vector3d` | 3D double vector |
| `vector.Vector3f` | 3D float vector |
| `vector.Vector3i` | 3D int vector |
| `vector.Vector3l` | 3D long vector |
| `vector.Vector4d` | 4D double vector |
| `vector.Location` | World location |
| `vector.Transform` | Position + rotation |

### Relative Vectors

| Class | Description |
|-------|-------------|
| `vector.relative.RelativeVector2d` | Relative 2D double |
| `vector.relative.RelativeVector3d` | Relative 3D double |
| `vector.relative.RelativeVector3i` | Relative 3D int |

### Shapes

| Class | Description |
|-------|-------------|
| `shape.Shape` | Base shape |
| `shape.Box` | 3D box |
| `shape.Box2D` | 2D box |
| `shape.Cylinder` | Cylinder |
| `shape.Ellipsoid` | Ellipsoid |
| `shape.Rectangle` | 2D rectangle |
| `shape.Quad2d` | 2D quad |
| `shape.Triangle2d` | 2D triangle |

### Block Shapes

| Class | Description |
|-------|-------------|
| `block.BlockUtil` | Block utilities |
| `block.BlockSphereUtil` | Sphere blocks |
| `block.BlockCubeUtil` | Cube blocks |
| `block.BlockCylinderUtil` | Cylinder blocks |
| `block.BlockConeUtil` | Cone blocks |
| `block.BlockDomeUtil` | Dome blocks |
| `block.BlockPyramidUtil` | Pyramid blocks |
| `block.BlockTorusUtil` | Torus blocks |

### Raycasting

| Class | Description |
|-------|-------------|
| `raycast.RaycastAABB` | AABB raycasting |
| `hitdetection.HitDetectionBuffer` | Hit detection buffer |
| `hitdetection.HitDetectionExecutor` | Hit detection |
| `hitdetection.LineOfSightProvider` | LOS checking |
| `hitdetection.MatrixProvider` | Matrix provider |

### Iterators

| Class | Description |
|-------|-------------|
| `iterator.BlockIterator` | Block iteration |
| `iterator.BoxBlockIterator` | Box block iteration |
| `iterator.LineIterator` | Line iteration |
| `iterator.CircleIterator` | Circle iteration |
| `iterator.SpiralIterator` | Spiral iteration |

### Ranges

| Class | Description |
|-------|-------------|
| `Range` | Base range |
| `range.IntRange` | Integer range |
| `range.FloatRange` | Float range |

### Utilities

| Class | Description |
|-------|-------------|
| `util.MathUtil` | Math utilities |
| `util.ChunkUtil` | Chunk math |
| `util.FastRandom` | Fast RNG |
| `util.TrigMathUtil` | Trigonometry |
| `util.NumberUtil` | Number utilities |
| `matrix.Matrix4d` | 4x4 double matrix |
