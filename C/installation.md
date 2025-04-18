# C Installation Guide

## Required Software

- **C Compiler**:
  - **GCC**: GNU Compiler Collection (Linux, macOS via Homebrew)
  - **Clang**: Part of LLVM (Linux, macOS)
  - **MSVC**: Microsoft Visual C++ (Windows)
  - **MinGW**: Minimalist GNU for Windows
- **Build System**: Make, CMake, or Ninja
- **Debugger**: GDB, LLDB, or Visual Studio Debugger

## File Extensions

- `.c` - C source files
- `.h` - Header files
- `.o`, `.obj` - Object files
- `.a`, `.lib` - Static libraries
- `.so`, `.dll`, `.dylib` - Shared libraries
- `.out`, `.exe` - Executable files
- `.gch` - Precompiled header files

## Package Management

```bash
# C doesn't have a standard package manager
# Libraries are typically managed manually or with build systems

# Configure with CMake
mkdir build && cd build
cmake ..

# Install dependencies on Ubuntu/Debian
apt-get install libname-dev

# Install dependencies on macOS
brew install libname

# Build with Make
make
make install
```

## Running C Programs

```bash
# Compile a simple program
gcc -o program program.c

# Compile with warnings and optimizations
gcc -Wall -Wextra -O2 -o program program.c

# Compile with external libraries
gcc -o program program.c -lm -lpthread

# Run the program
./program

# Debug with GDB
gdb ./program
```

## Common Libraries

- **C Standard Library**: libc, glibc
- **Mathematics**: libm (math.h)
- **Networking**: Berkeley sockets (socket.h)
- **Text Processing**: PCRE (Perl Compatible Regular Expressions)
- **Graphics**: SDL, OpenGL
- **Databases**: SQLite, libpq (PostgreSQL)
- **Utility**: GLib, APR (Apache Portable Runtime)
