# Tcl Installation Guide

## Required Software

- **Tcl/Tk**: The Tcl (Tool Command Language) interpreter and Tk toolkit
- **Expect**: Extension for automating interactive applications (optional)
- **Tclkit**: Standalone runtime for Tcl/Tk applications
- **VS Code**: With Tcl extension (recommended)
- **KomodoEdit**: Alternative IDE with Tcl support
- **ActiveTcl**: Commercial distribution of Tcl/Tk

## File Extensions

- `.tcl` - Tcl source files
- `.tk` - Tk-specific Tcl files
- `.exp` - Expect script files
- `.tm` - Tcl modules
- `.tbc` - Tcl bytecode files
- `.kit` - Tclkit starkit files
- `.exe` - Standalone Tcl executables (with Tclkit)
- `.so`, `.dll`, `.dylib` - Compiled Tcl extensions
- `.tclIndex` - Tcl package index files
- `.tclet` - Tcl applet files
- `.tsh` - Tclsh script files
- `.vfs` - Virtual filesystem used in starkits

## Package Management

```bash
# Install Tcl packages with teacup (part of ActiveTcl)
teacup install package_name

# Install Tcl packages manually
mkdir -p ~/lib/tcl
cd ~/lib/tcl
wget http://example.com/package.zip
unzip package.zip

# Add a package to your Tcl script
# package require PackageName

# List available packages
teacup list

# Search for packages
teacup search package_name

# Update packages
teacup update

# Using Tcllib (standard library)
# package require struct::list
```

## Running Tcl Programs

```bash
# Run a Tcl script with tclsh
tclsh script.tcl

# Run a Tcl script with wish (for Tk GUI)
wish script.tcl

# Run Tcl interactively
tclsh

# Run Tcl with arguments
tclsh script.tcl arg1 arg2

# Run Expect scripts
expect script.exp

# Create a standalone executable with Tclkit
tclkit sdx qwrap script.tcl
tclkit sdx unwrap script.kit

# Run a starkit
tclkit script.kit

# Debug a Tcl script
tclsh -d script.tcl
```

## Common Libraries

- **Tcllib**: Standard library collection
- **Tklib**: Tk widget collection
- **BLT**: Additional widgets and graph plotting
- **Img**: Extended image handling
- **Tdom**: XML/DOM processing
- **Tls**: SSL/TLS support
- **Itcl**: Object-oriented extensions
- **Thread**: Multi-threading support
- **Sqlite**: SQLite database interface
- **Snack**: Sound processing toolkit
- **Expect**: Program automation
- **Ffidl**: Foreign function interface
- **Critcl**: C embedding in Tcl
- **Http**: HTTP protocol support
- **Tclws**: Web services
- **Tk**: Standard GUI toolkit
