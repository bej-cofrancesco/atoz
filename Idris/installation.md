# Idris Installation Guide

## Required Software

- **Idris Compiler**: The Idris language compiler (Idris 1 or Idris 2)
- **Stack** or **Cabal**: For Haskell-based installation (Idris 1)
- **Scheme**: For Idris 2 (Chez Scheme recommended)
- **VS Code**: With Idris extension
- **Emacs**: With idris-mode (alternative)
- **Atom**: With language-idris package (alternative)

## File Extensions

- `.idr` - Idris source files
- `.lidr` - Literate Idris source files
- `.ipkg` - Idris package files
- `.ibc` - Idris bytecode files (compiled)
- `.iface` - Idris interface files
- `.ttc` - Idris type-checked term files
- `.o` - Object files
- `.a` - Archive files
- `.so`, `.dll`, `.dylib` - Shared libraries (platform dependent)

## Package Management

```bash
# Using Idris package manager
# Create a new package file (package.ipkg)

# Install a package
idris --install package.ipkg

# Install a package with dependencies
idris --installdeps package.ipkg

# Check a package
idris --checkpkg package.ipkg

# Clean compiled files
idris --clean package.ipkg

# For Idris 2:
idris2 --install package.ipkg
```

## Running Idris Programs

```bash
# Compile an Idris file
idris -o program file.idr

# Run the compiled program
./program

# Run in interpreter mode
idris file.idr -i

# Start the REPL
idris

# Load a file in REPL
idris file.idr

# For Idris 2:
# Compile
idris2 -o program file.idr

# Run REPL
idris2
```

## Common Libraries

- **Core**: prelude, base
- **Data Structures**: contrib, containers
- **Parsing**: lightyear, parser-combinators
- **Testing**: specdris, test
- **Web Development**: idris-http, scotty-ipsum
- **UI**: curses-idris
- **FFI**: idris-jvm (JVM backend), idris-gmp (bindings to GMP)
- **Effects**: effects, control.st (state)
- **Type-level Programming**: decidable, relations
- **Network**: network, socket
