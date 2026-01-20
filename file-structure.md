# Hytale Installation Structure

This document describes the file structure of a Hytale installation.

## Installation Path

```
%APPDATA%/Hytale/
```

## Directory Structure

```
Hytale/
├── install/
│   └── release/
│       ├── env.dat
│       └── package/
│           ├── game/
│           │   ├── latest/
│           │   │   ├── Assets.zip      (~3.1 GB - game assets)
│           │   │   ├── Client/
│           │   │   │   ├── HytaleClient.exe    (native C++ client)
│           │   │   │   ├── Data/
│           │   │   │   ├── NodeEditor/
│           │   │   │   └── [DLLs: Noesis, SDL3, OpenAL, etc.]
│           │   │   └── Server/
│           │   │       ├── HytaleServer.jar    (Java server - 80MB)
│           │   │       ├── HytaleServer.aot    (AOT compiled)
│           │   │       └── Licenses/
│           │   └── build-*/                    (previous builds)
│           ├── jre/                            (bundled Java runtime)
│           └── sig/                            (signatures)
└── UserData/
    ├── Mods/                                   (user mods folder)
    ├── Saves/
    ├── Settings.json
    └── Logs/
```

## Key Files for Modding

| File | Description |
|------|-------------|
| `HytaleServer.jar` | Java server - decompile this for API investigation |
| `Assets.zip` | Game assets (models, textures, prefabs) |
| `UserData/Mods/` | Where mods are installed |

## Notes

- **Client**: Native C++ executable (not directly moddable via Java)
- **Server**: Java-based, supports plugin/mod development
- **Modding**: Plugins interact with the server JAR API
