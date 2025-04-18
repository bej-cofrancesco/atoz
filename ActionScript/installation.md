# ActionScript Installation Guide

## Required Software

- **Adobe Flash Builder** or **Adobe Animate** (previously Flash Professional)
- **Apache Flex SDK**: [flex.apache.org](https://flex.apache.org/) for open-source development
- **Adobe AIR SDK**: For building desktop and mobile applications

## File Extensions

- `.as` - ActionScript source files
- `.mxml` - MXML component files (Flex)
- `.swf` - Compiled Flash movie
- `.swc` - Compiled component library
- `.fla` - Flash authoring file
- `.air` - Adobe AIR installation package

## Package Management

```bash
# Apache Flex
# Create a new Flex project
mxmlc -locale=en_US -source-path=./src -output=MyApp.swf ./src/MyApp.as

# Adobe AIR
# Package an AIR application
adt -package -storetype pkcs12 -keystore cert.p12 -storepass password MyApp.air application.xml MyApp.swf assets/
```

## Running ActionScript Programs

```bash
# Run a SWF file using standalone Flash Player
flashplayer MyApp.swf

# Debug with Flash Debug Player
flashplayerdebugger MyApp.swf

# Run AIR application for testing
adl application.xml
```

## Common Libraries

- **Flex Framework**: UI components and layout management
- **Starling**: 2D game framework
- **Away3D**: 3D engine
- **GreenSock**: Animation platform
- **PureMVC**: Application architecture framework
