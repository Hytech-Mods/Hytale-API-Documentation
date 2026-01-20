# Player Messaging

How to send messages to players in Hytale.

## Package: `com.hypixel.hytale.server.core`

### Message Class

| Class | Status | Description |
|-------|--------|-------------|
| `Message` | 🟢 Verified | Message to send to players |
| `Message.raw()` | 🟢 Verified | Create raw text message |

## Sending Messages

```java
import com.hypixel.hytale.server.core.Message;
import com.hypixel.hytale.server.core.entity.entities.Player;

// Send a simple message
player.sendMessage(Message.raw("Hello, player!"));
```

## Important Notes

> **⚠️ Color Codes**: Hytale does NOT use Minecraft-style color codes (`§6`, `§a`, etc.). These will display as literal characters in chat. Use plain text for now.

> **⚠️ Unicode Characters**: Some Unicode characters (like `━` box drawing or `✦` symbols) may not render correctly. Stick to basic ASCII characters.

## Working Example

```java
// This works (Verified):
player.sendMessage(Message.raw("========================================"));
player.sendMessage(Message.raw("* Welcome to Hytech! *"));
player.sendMessage(Message.raw("  - Mod Name v1.0.0"));
player.sendMessage(Message.raw("========================================"));
```

## Validation Status Legend

| Status | Meaning |
|--------|---------|
| 🟢 Verified | Tested in-game, confirmed working |
| 🔴 Requires Validation | Discovered from decompilation, not yet tested |

## Related

- [Player Events](player-events.md) - Handling player join/disconnect
