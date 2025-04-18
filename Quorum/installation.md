# Quorum Installation Guide

## Required Software

- **Quorum**: The Quorum programming language
- **Java Runtime Environment (JRE)**: Required to run Quorum programs
- **Java Development Kit (JDK)**: Required for building Quorum from source
- **Quorum Studio**: Integrated development environment for Quorum
- **VS Code**: With Java extension (alternative)
- **Android SDK**: For mobile app development (optional)

## File Extensions

- `.quorum` - Quorum source code files
- `.qp` - Quorum packages
- `.jar` - Java Archive (compiled Quorum or dependencies)
- `.sodbeans` - Quorum Studio project file
- `.properties` - Properties configuration files
- `.qrk` - Quorum project files
- `.class` - Java bytecode (compiled Quorum code)
- `.qproj` - Quorum project files
- `.h`, `.c`, `.cpp` - Native code files (for plugins)
- `.wav`, `.mp3`, `.ogg` - Audio files used in Quorum
- `.png`, `.jpg` - Image files used in Quorum

## Package Management

```bash
# Quorum uses a built-in package manager in its IDE
# Manual installation from the command line:

# Create a project directory
mkdir myproject
cd myproject

# Download a package (manual)
wget https://example.com/package.qp

# Add the package to your project
# (Usually done through Quorum Studio GUI)

# Update packages
# (Usually done through Quorum Studio GUI)
```

## Running Quorum Programs

```bash
# Run a Quorum program using the Quorum interpreter
quorum run Main.quorum

# Compile a Quorum program
quorum compile Main.quorum

# Run a compiled Quorum program
java -jar MyCompiledProgram.jar

# Run with Quorum Studio
# 1. Open Quorum Studio
# 2. Open your project
# 3. Click the Run button

# Run with specific console parameters
quorum run Main.quorum parameter1 parameter2

# Build a distributable application
quorum build distribute Main.quorum

# Run in debug mode
quorum debug Main.quorum
```

## Common Libraries

- **Standard Library**: Core utilities included with Quorum
- **Game Engine**: Built-in 2D/3D game development library
- **Database**: Database connectivity and management
- **Sound**: Audio playback and manipulation
- **Speech**: Text-to-speech capabilities
- **Web**: Web services and HTTP requests
- **UI**: User interface components
- **Disability Components**: Accessibility features
- **Input/Output**: File I/O operations
- **Math**: Mathematical operations and algorithms
- **Physics**: Physics simulation for games
- **Accessibility Plugins**: Screen reader support, etc.
- **Charts**: Data visualization tools
