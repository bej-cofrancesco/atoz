# Bash Installation Guide

## Required Software

- **Bash**: Included by default on most Linux distributions and macOS
  - **Windows**: Available through WSL (Windows Subsystem for Linux) or Git Bash

## File Extensions

- `.sh` - Shell script files
- `.bash` - Bash-specific script files
- (no extension) - Executable scripts (common in Unix)
- `.bashrc`, `.bash_profile` - Bash configuration files
- `.env` - Environment variable files

## Package Management

```bash
# Bash doesn't have a dedicated package manager
# Packages are typically managed by the OS package manager

# Source external scripts
source script.sh
# or
. script.sh

# Include utility functions
# Often stored in /usr/lib or /usr/local/lib
```

## Running Bash Programs

```bash
# Make script executable
chmod +x script.sh

# Run script
./script.sh

# Run with bash interpreter explicitly
bash script.sh

# Pass arguments
./script.sh arg1 arg2

# Run with debugging
bash -x script.sh
```

## Common Libraries

- **Bash doesn't have libraries in the traditional sense**
- **GNU Coreutils**: Standard command-line utilities
- **awk/sed/grep**: Text processing tools
- **jq**: JSON processing
- **curl/wget**: Network utilities
- **Common utility scripts**: Often shared as snippets or functions
