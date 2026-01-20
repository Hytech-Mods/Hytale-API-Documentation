# Plugin System

The plugin system allows mods to extend Hytale server functionality.

## Package: `com.hypixel.hytale.plugin.early`

Early-stage plugin loading and class transformation.

| Class | Description |
|-------|-------------|
| `ClassTransformer` | Bytecode transformation for mods |
| `EarlyPluginLoader` | Loads plugins before server starts |
| `TransformingClassLoader` | Custom class loader for transformed classes |

## Package: `com.hypixel.hytale.server.core.plugin`

Core plugin API for mod development.

### Main Classes

| Class | Description |
|-------|-------------|
| `JavaPlugin` | **Base class for Java plugins** - extend this |
| `JavaPluginInit` | Initialization data passed to plugin constructor |
| `PluginManager` | Manages plugin lifecycle and registration |
| `PluginBase` | Abstract base for all plugins |
| `PluginState` | Plugin state enum (loading, active, etc.) |
| `PluginType` | Type of plugin |
| `PluginLoader` | Loads plugins from disk |

### Plugin Events

| Class | Description |
|-------|-------------|
| `event.PluginEvent` | Base plugin event |
| `event.PluginSetupEvent` | Fired during plugin setup |

### Registry Classes

| Class | Description |
|-------|-------------|
| `registry.IRegistry` | Registry interface |
| `registry.AssetRegistry` | Asset registration |
| `registry.CodecMapRegistry` | Codec map registration |
| `registry.MapKeyMapRegistry` | Map key registration |

### Commands & Pages

| Class | Description |
|-------|-------------|
| `commands.PluginCommand` | Plugin management command |
| `pages.PluginListPage` | Debug page listing plugins |

## Usage Example

```java
public class MyPlugin extends JavaPlugin {
    public MyPlugin(JavaPluginInit init) {
        super(init);
    }
    
    @Override
    protected void setup() {
        // Register commands, events, etc.
    }
}
```
