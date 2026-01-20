# Inventory Transactions

Safe inventory modifications with transaction system.

## Package: `com.hypixel.hytale.server.core.inventory.transaction`

### Core Classes

| Class | Description |
|-------|-------------|
| `Transaction` | **Base transaction class** |
| `SlotTransaction` | Slot-based transaction |
| `ListTransaction` | List of transactions |
| `ClearTransaction` | Clear container |

### ItemStack Transactions

| Class | Description |
|-------|-------------|
| `ItemStackTransaction` | ItemStack transaction |
| `ItemStackSlotTransaction` | Slot-specific ItemStack transaction |

### Material Transactions

| Class | Description |
|-------|-------------|
| `MaterialTransaction` | Material transaction |
| `MaterialSlotTransaction` | Slot-specific material transaction |

### Resource Transactions

| Class | Description |
|-------|-------------|
| `ResourceTransaction` | Resource transaction |
| `ResourceSlotTransaction` | Slot-specific resource transaction |

### Tag Transactions

| Class | Description |
|-------|-------------|
| `TagTransaction` | Tag-based transaction |
| `TagSlotTransaction` | Slot-specific tag transaction |

### Move Transactions

| Class | Description |
|-------|-------------|
| `MoveTransaction` | Move items between containers |
| `MoveType` | Type of move operation |
| `ActionType` | Transaction action type |

## Usage

Transactions ensure atomic inventory operations:

```java
// Create a transaction
ItemStackSlotTransaction transaction = new ItemStackSlotTransaction(
    container, slot, itemStack, ActionType.ADD
);

// Execute transaction
transaction.execute();
```
