# Unison Installation Guide

## Required Software

- **Unison Codebase Manager (UCM)**: The Unison language environment
- **Git**: For version control and sharing code
- **VS Code**: With Unison extension (recommended)
- **Atom**: With Unison extension (alternative)
- **Emacs**: With Unison mode (alternative)
- **Homebrew**: For macOS installation (optional)

## File Extensions

- `.u` - Unison source files
- `.md` - Markdown documentation files
- `.uu` - Unison universal files
- `LICENSE` - License files for Unison libraries
- `.unisonhistory` - Unison command history
- `.unison/` - Unison workspace directory
- `.session` - Unison session files
- `.branches/` - Unison branch information
- `.transcript` - Unison transcript files
- `.output` - Unison output files
- `.json` - JSON files for configuration
- `.svg`, `.png` - Documentation graphics

## Package Management

```bash
# Unison has a content-addressed code model rather than traditional packages
# Libraries are shared via "pulls" from remote code repositories

# Start the UCM (Unison Codebase Manager)
ucm

# Inside the UCM, pull from a published library
.pull https://github.com/username/repo:.releases._latest .mylib

# List available libraries in your codebase
.ls

# Update dependencies (pull latest)
.pull https://github.com/username/repo:.releases._latest .mylib

# Share your own code
# First push to GitHub or similar
.push git@github.com:username/repo:.trunk

# Create a release
.create_release.minor trunk
```

## Running Unison Programs

```bash
# Start the Unison Codebase Manager
ucm

# Create a new scratch file
# (This would be done in your editor)
# Save as scratch.u

# Load a scratch file
.load scratch.u

# Run a function in UCM
> myFunction 42

# Watch a file for changes
.watch scratch.u

# Run a program with arguments
.run myProgram "argument1" "argument2"

# Add a test
.add_test

# Run tests
.test

# Debug a function
.debug myFunction

# Display documentation
.display doc myFunction
```

## Common Libraries

- **Base**: Standard library (built-in)
- **Distributed**: Distributed computing primitives
- **HTTP**: HTTP client and server
- **Doc**: Documentation utilities
- **Text**: Text processing utilities
- **IO**: Input/output operations
- **Parser**: Parsing combinators
- **JSON**: JSON encoding/decoding
- **Stream**: Stream processing
- **Test**: Testing utilities
- **Code**: Code manipulation utilities
- **Terminal**: Terminal interaction
- **Concurrency**: Concurrency utilities
- **Crypto**: Cryptographic functions
- **Math**: Mathematical utilities
- **Collections**: Additional data structures
