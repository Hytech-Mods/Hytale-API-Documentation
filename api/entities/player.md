# Player

Player entity and management systems.

## Package: `com.hypixel.hytale.server.core.entity.entities`

### Main Class

| Class | Description |
|-------|-------------|
| `Player` | **Player entity class** |

## Package: `com.hypixel.hytale.server.core.entity.entities.player`

### Managers

| Class | Description |
|-------|-------------|
| `CameraManager` | Player camera control |
| `HiddenPlayersManager` | Player visibility |
| `HotbarManager` | Hotbar management |
| `MovementManager` | Movement handling |
| `PageManager` | UI page management |
| `WindowManager` | Window/UI management |

### HUD System

| Class | Description |
|-------|-------------|
| `hud.HudManager` | **HUD management** |
| `hud.CustomUIHud` | Custom HUD elements |

### Movement

| Class | Description |
|-------|-------------|
| `movement.MovementConfig` | Movement configuration |
| `movement.MovementManager` | Movement system |

### Data Components

| Class | Description |
|-------|-------------|
| `data.PlayerConfigData` | Player config |
| `data.PlayerWorldData` | World-specific data |
| `data.PlayerDeathPositionData` | Death position |
| `data.PlayerRespawnPointData` | Respawn location |
| `data.UniqueItemUsagesComponent` | Item usage tracking |

### Windows

| Class | Description |
|-------|-------------|
| `windows.Window` | Base window class |
| `windows.WindowManager` | Window management |
| `windows.ContainerWindow` | Container window |
| `windows.ItemContainerWindow` | Item container |
| `windows.BlockWindow` | Block interaction window |
| `windows.ValidatedWindow` | Validated window |

### UI Pages

| Class | Description |
|-------|-------------|
| `pages.CustomUIPage` | Custom UI page |
| `pages.InteractiveCustomUIPage` | Interactive page |
| `pages.RespawnPage` | Respawn screen |
| `pages.choices.ChoiceBasePage` | Choice dialog |
| `pages.itemrepair.ItemRepairPage` | Item repair UI |
