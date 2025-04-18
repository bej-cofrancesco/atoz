# Zig Installation Guide

## Required Software

- **Zig Compiler**: The Zig programming language
- **Git**: For version control and package management
- **VS Code**: With Zig extension (recommended)
- **Emacs**: With zig-mode (alternative)
- **Vim/Neovim**: With zig.vim (alternative)
- **LLVM**: Used by Zig for compilation and optimization (included in Zig)

## File Extensions

- `.zig` - Zig source files
- `.o` - Object files
- `.a` - Static libraries
- `.so`, `.dll`, `.dylib` - Shared libraries (platform dependent)
- `.h` - C header files (for interfacing with C)
- `.exe` - Executable files (on Windows)
- `build.zig` - Zig build script
- `.wasm` - WebAssembly output
- `.ui` - Zir (Zig IR) files
- `.d` - Dependency files
- `.S` - Assembly files
- `.zigmod` - Zigmod package manager files
- `.gyro.zzz` - Gyro package manager files

## Package Management

```bash
# Zig doesn't have an official package manager yet, but there are community options

# Using zigmod
# Install zigmod
wget -qO- https://github.com/nektro/zigmod/releases/download/r68/zigmod-x86_64-linux > zigmod
chmod +x zigmod
sudo mv zigmod /usr/local/bin/

# Initialize a project
zigmod init

# Add a dependency
zigmod add --git https://github.com/username/repo

# Update dependencies
zigmod fetch

# Using gyro
# Install gyro
curl -fsSL https://github.com/mattnite/gyro/releases/download/0.5.0/gyro-0.5.0-linux-x86_64.tar.gz | tar -xz
sudo mv gyro /usr/local/bin/

# Initialize a project
gyro init

# Add a dependency
gyro add --github username/repo

# Update dependencies
gyro fetch
```

## Running Zig Programs

```bash
# Compile a Zig file
zig build-exe main.zig

# Run a compiled program
./main

# Compile and run in one step
zig run main.zig

# Compile with optimizations
zig build-exe main.zig -O ReleaseFast

# Build a library
zig build-lib lib.zig

# Run tests
zig test main.zig

# Build for a specific target
zig build-exe main.zig -target x86_64-windows-gnu

# Use the build system
zig build

# Initialize a build.zig file
zig init-exe
# or
zig init-lib

# Compile to WebAssembly
zig build-exe main.zig -target wasm32-freestanding

# Cross-compile
zig build-exe main.zig -target aarch64-linux-gnu
```

## Common Libraries

- **Standard Library**: Built-in standard library
- **C Standard Library**: Accessible via @cImport
- **Zig Algorithm and Data Structure Library (ZASDL)**: Community library
- **Mach**: Game engine and graphics library
- **ZigJSON**: JSON parsing and generation
- **ZigHttpLib**: HTTP library
- **ZiglySQL**: SQL interface
- **ZLS**: Zig Language Server
- **ZBUS**: Message bus implementation
- **ZBOR**: CBOR implementation
- **Tigerbeetle**: Distributed financial accounting database
- **Zig-gamedev**: Game development toolkit
- **ZGUI**: Dear ImGui bindings
- **Network**: Networking library
- **Event**: Event handling
- **Args**: Command-line argument parsing
