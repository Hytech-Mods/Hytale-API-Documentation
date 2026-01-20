# Player Events

Handling player connection and interaction events.

## Package: `com.hypixel.hytale.server.core.event.events.player`

### Available Events

| Event | Description |
|-------|-------------|
| `PlayerConnectEvent` | Player connects to server |
| `PlayerDisconnectEvent` | Player disconnects |
| `PlayerReadyEvent` | Player is ready |
| `PlayerChatEvent` | Player sends chat message |
| `PlayerInteractEvent` | Player interacts |
| `PlayerCraftEvent` | Player crafts item |

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

> **Deprecated API**: `event.getPlayer()` is marked as deprecated. It still works but may change in future versions.

## Related

- [Messaging](messaging.md) - Sending messages to players
- [Event System](event-system.md) - General event handling
