# Event System

Hytale uses an event bus system for communication between game systems and plugins.

## Package: `com.hypixel.hytale.event`

### Core Interfaces

| Interface | Description |
|-----------|-------------|
| `IEvent` | Base event interface |
| `IBaseEvent` | Extended base event |
| `IAsyncEvent` | Async event marker |
| `ICancellable` | Cancellable events |
| `IProcessedEvent` | Post-processing events |

### Event Bus

| Class | Description |
|-------|-------------|
| `EventBus` | Main event bus implementation |
| `IEventBus` | Event bus interface |
| `EventBusRegistry` | Registry of event buses |
| `AsyncEventBusRegistry` | Async event bus registry |
| `SyncEventBusRegistry` | Sync event bus registry |

### Registration

| Class | Description |
|-------|-------------|
| `EventRegistry` | Registers event handlers |
| `IEventRegistry` | Event registry interface |
| `EventRegistration` | Registration metadata |
| `IEventDispatcher` | Dispatches events |
| `EventPriority` | Handler priority ordering |

## Usage

```java
// In your plugin setup
eventRegistry.register(MyEvent.class, this::onMyEvent);

// Event handler
private void onMyEvent(MyEvent event) {
    // Handle event
}
```
