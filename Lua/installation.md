# Lua Installation Guide

## Required Software

- **Lua Interpreter**: The Lua programming language (5.1, 5.2, 5.3, 5.4)
- **LuaRocks**: Package manager for Lua modules
- **VS Code**: With Lua extension (recommended)
- **ZeroBrane Studio**: Lightweight Lua IDE (alternative)
- **LuaJIT**: Just-In-Time compiler for Lua (for performance)

## File Extensions

- `.lua` - Lua source files
- `.luac` - Compiled Lua bytecode
- `.rockspec` - LuaRocks package specification
- `.so`, `.dll`, `.dylib` - Compiled C modules (platform dependent)
- `.wlua` - Lua scripts for GUI applications
- `.tlua` - Typed Lua files
- `.moon` - Moonscript files (Lua preprocessor)
- `.lua.tmp` - Temporary Lua files
- `.luacheckrc` - Luacheck configuration file
- `.luarocks` - LuaRocks configuration directory

## Package Management

```bash
# Install LuaRocks package manager
# (varies by OS, example for Ubuntu)
sudo apt-get install luarocks

# Install a package globally
luarocks install package_name

# Install a specific version
luarocks install package_name 2.0.1

# Install locally
luarocks install package_name --local

# Remove a package
luarocks remove package_name

# List installed packages
luarocks list

# Create a new rock specification
luarocks write_rockspec

# Build and install from a rockspec
luarocks build package.rockspec
```

## Running Lua Programs

```bash
# Run a Lua script
lua script.lua

# Run with arguments
lua script.lua arg1 arg2

# Run with LuaJIT (for better performance)
luajit script.lua

# Run Lua interactively (REPL)
lua

# Compile to bytecode
luac -o output.luac script.lua

# Run bytecode
lua output.luac

# Run with debugging
lua -e "debug.debug()" script.lua
```

## Common Libraries

- **Web Frameworks**: Lapis, OpenResty, Sailor
- **Testing**: Busted, Luaunit
- **ORM**: Lapis DB, LuaSQL
- **HTTP**: LuaSocket, lua-requests, http
- **JSON**: dkjson, lunajson, cjson
- **GUI**: IUP, wxLua, LuaQt
- **Game Development**: LÖVE, Corona SDK
- **Networking**: LuaSocket, Copas
- **Concurrency**: Lanes, Lumen
- **Templating**: etlua, lustache
- **Utility**: penlight, middleclass (OOP), inspect (debugging)
