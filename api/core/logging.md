# Logging

Hytale provides a custom logging framework with file output and Sentry integration.

## Package: `com.hypixel.hytale.logger`

### Main Class

| Class | Description |
|-------|-------------|
| `HytaleLogger` | **Main logger class** - use this for logging |

### Backend

| Class | Description |
|-------|-------------|
| `backend.HytaleLoggerBackend` | Logger backend implementation |
| `backend.HytaleLogManager` | Log manager |
| `backend.HytaleConsole` | Console output |
| `backend.HytaleFileHandler` | File output |
| `backend.HytaleLogFormatter` | Log formatting |
| `backend.HytaleUncaughtExceptionHandler` | Exception handling |

### Sentry Integration

| Class | Description |
|-------|-------------|
| `sentry.HytaleSentryHandler` | Sentry error reporting |
| `sentry.SkipSentryException` | Skip Sentry for exception |

### Utilities

| Class | Description |
|-------|-------------|
| `util.LoggerPrintStream` | Print stream wrapper |
| `util.GithubMessageUtil` | GitHub integration |

## Usage

```java
private static final HytaleLogger LOGGER = HytaleLogger.forEnclosingClass();

public void myMethod() {
    LOGGER.atInfo().log("Info message");
    LOGGER.atWarning().log("Warning message");
    LOGGER.atSevere().log("Error message");
}
```
