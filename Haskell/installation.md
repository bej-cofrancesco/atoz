# Haskell Installation Guide

## Required Software

- **GHC**: The Glasgow Haskell Compiler
- **Stack**: The Haskell Tool Stack for project management
- **Cabal**: Common Architecture for Building Applications and Libraries
- **VS Code**: With Haskell extension (recommended)
- **IntelliJ IDEA**: With Haskell plugin (alternative)
- **HLS**: Haskell Language Server

## File Extensions

- `.hs` - Haskell source code files
- `.lhs` - Literate Haskell source files
- `.hsc` - Haskell with C bindings
- `.chs` - C2HS binding files
- `.cabal` - Cabal package description
- `.yaml`, `.yml` - Stack/project configuration files
- `.hi` - Haskell interface files (compiled)
- `.o` - Object files
- `.hsig` - Haskell signature files
- `.hie` - Haskell Interface Extended files
- `.gadt` - GADT syntax files

## Package Management

```bash
# Using Stack:
# Create a new project
stack new project-name

# Build project
stack build

# Install dependencies
stack install package-name

# Update package index
stack update

# Using Cabal:
# Initialize a new project
cabal init

# Configure and build
cabal build

# Install a package
cabal install package-name

# Update package index
cabal update

# Add a dependency to .cabal file
cabal install --lib package-name
```

## Running Haskell Programs

```bash
# Using Stack:
# Run project
stack run

# Run GHCi (REPL) with project modules
stack ghci

# Run tests
stack test

# Using Cabal:
# Run project
cabal run

# Start GHCi with project modules
cabal repl

# Run tests
cabal test

# Standalone GHC:
# Compile a Haskell file
ghc MyFile.hs

# Run the compiled executable
./MyFile

# Run with GHCi (REPL)
ghci MyFile.hs
```

## Common Libraries

- **Web Frameworks**: Yesod, Servant, Scotty, Spock
- **Parsers**: Parsec, Megaparsec, Attoparsec
- **Testing**: HUnit, QuickCheck, Tasty, Hspec
- **Data Structures**: containers, unordered-containers, vector
- **Text Processing**: text, bytestring, aeson (JSON)
- **Database**: persistent, esqueleto, postgresql-simple, HDBC
- **Concurrency**: async, stm (Software Transactional Memory)
- **Type-level**: type-level, servant-type-level
- **Functional Programming**: lens, mtl, transformers
- **Graphics/UI**: gloss, brick (terminal UI), threepenny-gui
