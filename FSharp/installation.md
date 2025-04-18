# F# Installation Guide

## Required Software

- **.NET SDK**: Includes F# compiler and runtime
- **Visual Studio** (Windows): With F# development workload
- **Visual Studio Code**: With Ionide-fsharp extension
- **JetBrains Rider**: Supports F# development
- **Mono** (for non-Windows platforms, if needed)

## File Extensions

- `.fs` - F# source code files
- `.fsi` - F# signature files (interfaces)
- `.fsx` - F# script files
- `.fsscript` - Alternative extension for F# scripts
- `.fsproj` - F# project files
- `.dll` - Compiled F# assemblies
- `.exe` - Executable files (on Windows)
- `paket.dependencies` - Paket dependency manager file
- `paket.lock` - Paket lock file

## Package Management

```bash
# Create a new F# console application
dotnet new console -lang F# -o MyProject

# Create a new F# library
dotnet new classlib -lang F# -o MyLibrary

# Add a package reference
dotnet add package PackageName

# Restore packages
dotnet restore

# Using Paket (alternative package manager)
dotnet tool install --global Paket
paket init
paket add PackageName
paket install
```

## Running F# Programs

```bash
# Compile F# project
dotnet build

# Run F# application
dotnet run

# Run F# script
dotnet fsi script.fsx

# Create a release build
dotnet publish -c Release

# Run tests
dotnet test
```

## Common Libraries

- **Core**: FSharp.Core
- **Data Access**: SqlProvider, FSharp.Data
- **Web Development**: Giraffe, Suave, Saturn, Fable
- **Parsing**: FParsec
- **Testing**: Expecto, FsUnit, Unquote
- **Functional Utilities**: FSharpPlus, FSharpx
- **JSON**: Thoth.Json, Newtonsoft.Json
- **UI**: Avalonia, Elmish
