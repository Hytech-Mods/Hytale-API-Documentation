# Inventory System

Item containers and inventory management.

## Package: `com.hypixel.hytale.server.core.inventory`

### Core Classes

| Class | Description |
|-------|-------------|
| `Inventory` | **Player inventory** |
| `ItemStack` | **Item stack** - quantity + data |
| `ItemContext` | Item usage context |
| `MaterialQuantity` | Material + amount |
| `ResourceQuantity` | Resource + amount |

## ItemContainer API

### Package: `com.hypixel.hytale.server.core.inventory.container`

| Class | Description |
|-------|-------------|
| `ItemContainer` | **Base container interface** |
| `SimpleItemContainer` | Simple implementation |
| `ItemStackItemContainer` | ItemStack-based container |
| `CombinedItemContainer` | Multiple containers combined |
| `DelegateItemContainer` | Delegating container |
| `EmptyItemContainer` | Empty container |
| `ItemContainerUtil` | Container utilities |

### Container Methods

```java
// Get capacity
int getCapacity();

// Get item at slot
ItemStack getItemStack(int slot);

// Add items
boolean addItemStack(ItemStack stack);

// Remove from slot
ItemStack removeItemStackFromSlot(int slot, int count);

// Sort container
void sort(SortType type);
```

### Slot Filters

| Class | Description |
|-------|-------------|
| `filter.SlotFilter` | Base filter |
| `filter.ItemSlotFilter` | Item type filter |
| `filter.ArmorSlotAddFilter` | Armor slot filter |
| `filter.TagFilter` | Tag-based filter |
| `filter.ResourceFilter` | Resource filter |
| `filter.NoDuplicateFilter` | No duplicate items |
| `filter.FilterActionType` | Filter action type |

### Sorting

| Class | Description |
|-------|-------------|
| `SortType` | Sort type enum |
| `SlotReplacementFunction` | Slot replacement |

## Usage Example

```java
// Get player inventory
Inventory inventory = player.getInventory();
ItemContainer container = inventory.getBackpack();

// Check capacity
int capacity = container.getCapacity();

// Get item from slot
ItemStack stack = container.getItemStack(0);

// Remove items
ItemStack removed = container.removeItemStackFromSlot(0, 1);
```
