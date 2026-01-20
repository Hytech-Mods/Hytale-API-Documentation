# Player Events

Handling player connection and interaction events.

## Package: `com.hypixel.hytale.server.core.event.events.player`

### Available Events

| Event | Status | Description |
|-------|--------|-------------|
| `PlayerConnectEvent` | 🟢 Verified | Player connects to server |
| `PlayerDisconnectEvent` | 🔴 Requires Validation | Player disconnects |
| `PlayerReadyEvent` | 🔴 Requires Validation | Player is ready |
| `PlayerChatEvent` | 🔴 Requires Validation | Player sends chat message |
| `PlayerInteractEvent` | 🔴 Requires Validation | Player interacts |
| `PlayerCraftEvent` | 🔴 Requires Validation | Player crafts item |

## Registering Event Handlers

```java
import com.hypixel.hytale.event.IEventRegistry;
import com.hypixel.hytale.server.core.event.events.player.PlayerConnectEvent;

@Override
protected void setup() {
    IEventRegistry eventRegistry = this.getEventRegistry();
    eventRegistry.register(PlayerConnectEvent.class, this::onPlayerConnect);
}

private void onPlayerConnect(PlayerConnectEvent event) {
    Player player = event.getPlayer();
    // Handle player connection
}
```

## Getting Player from Event

```java
// Note: getPlayer() is deprecated but still works
Player player = event.getPlayer();

// Send message to player
player.sendMessage(Message.raw("Welcome!"));
```

## Important Notes

> **⚠️ Deprecated API**: `event.getPlayer()` is marked as deprecated. It still works but may change in future versions.

## Validation Status Legend

| Status | Meaning |
|--------|---------|
| 🟢 Verified | Tested in-game, confirmed working |
| 🔴 Requires Validation | Discovered from decompilation, not yet tested |

## Related

- [Messaging](messaging.md) - Sending messages to players
- [Event System](event-system.md) - General event handling
