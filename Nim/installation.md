# Nim Installation Guide

## Required Software

- **Nim Compiler**: The Nim programming language
- **Nimble**: Nim package manager
- **C Compiler**: GCC, Clang, or Visual C++ (Nim compiles to C)
- **VS Code**: With Nim extension (recommended)
- **Aporia**: Nim-specific IDE (alternative)
- **Git**: For version control and package installation

## File Extensions

- `.nim` - Nim source files
- `.nims` - Nim script files
- `.nimble` - Nimble package specification files
- `.c`, `.cpp` - Generated C/C++ code
- `.h` - Generated header files
- `.o`, `.obj` - Compiled object files
- `.nim.cfg` - Nim configuration file
- `.nimcache/` - Directory for cache files
- `.nimsettings` - Nim settings file
- `.nimproject` - Nim project file

## Package Management

```bash
# Install a package
nimble install package_name

# Install a specific version
nimble install package_name@0.1.0

# Install a package from Git
nimble install "https://github.com/user/repo.git"

# Update packages
nimble update

# Search for packages
nimble search keyword

# List installed packages
nimble list

# Create a new Nimble package
nimble init

# Build a Nimble package
nimble build

# Publish a package
nimble publish
```

## Running Nim Programs

```bash
# Compile and run a Nim file
nim c -r filename.nim

# Compile with optimizations
nim c -d:release filename.nim

# Compile to C++
nim cpp -r filename.nim

# Compile to JavaScript
nim js -r filename.nim

# Compile to WebAssembly
nim c -d:emscripten filename.nim

# Run the Nim REPL
nim secret

# Generate documentation
nim doc filename.nim

# Compile with debugging information
nim c -g -r filename.nim
```

## Common Libraries

- **Web Frameworks**: Jester, Karax, Prologue
- **GUI**: nimx, nigui
- **Database**: norm, nimDB, nimongo
- **HTTP**: httpbeast, httpclient
- **JSON**: std/json, packedjson
- **Parsing**: npeg, parseopt
- **Testing**: unittest, testament
- **Async Programming**: asyncdispatch, chronos
- **Game Development**: nico, nimgame2
- **Graphics**: pixie, chroma
- **CLI**: cligen, docopt
- **Cryptography**: nimcrypto
