# Command System

Hytale has a comprehensive command system with argument parsing, permissions, and suggestions.

## Package: `com.hypixel.hytale.server.core.command.system`

### Base Classes

| Class | Description |
|-------|-------------|
| `CommandBase` | **Base class for custom commands** - extend this |
| `AbstractCommand` | Abstract command implementation |
| `AbstractPlayerCommand` | Command requiring player sender |
| `AbstractWorldCommand` | Command requiring world context |
| `AbstractTargetEntityCommand` | Command targeting entities |
| `AbstractAsyncCommand` | Async command execution |
| `AbstractCommandCollection` | Group related commands |

### Command System

| Class | Description |
|-------|-------------|
| `CommandManager` | Manages command registration |
| `CommandRegistry` | Registry of commands |
| `CommandContext` | Execution context |
| `CommandSender` | Who sent the command |
| `CommandUtil` | Command utilities |
| `CommandOwner` | Command ownership |

### Argument System

| Class | Description |
|-------|-------------|
| `Argument` | Base argument class |
| `RequiredArg` | Required argument |
| `OptionalArg` | Optional argument |
| `FlagArg` | Flag argument |
| `DefaultArg` | Default value argument |

### Argument Types

| Class | Description |
|-------|-------------|
| `ArgumentType` | Argument type interface |
| `SingleArgumentType` | Single value |
| `ListArgumentType` | List of values |
| `EnumArgumentType` | Enum values |
| `AssetArgumentType` | Asset references |
| `GameModeArgumentType` | Game modes |
| `RelativeIntPosition` | Relative coordinates |

### Exceptions

| Class | Description |
|-------|-------------|
| `CommandException` | Base command exception |
| `NoPermissionException` | Permission denied |
| `SenderTypeException` | Wrong sender type |

## Built-in Commands

See [Built-in Commands](commands-builtin.md) for the full list.

## Usage Example

```java
public class MyCommand extends CommandBase {
    public MyCommand() {
        super("mycommand", "Description here");
        setPermissionGroup(GameMode.Adventure);
    }
    
    @Override
    protected void executeSync(CommandContext ctx) {
        ctx.sendMessage(Message.raw("Hello!"));
    }
}
```
