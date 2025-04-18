# C# Installation Guide

## Required Software

- **.NET SDK**: Download from [dotnet.microsoft.com](https://dotnet.microsoft.com/download)
  - Includes the C# compiler, runtime, and basic libraries
- **Visual Studio** (optional): Comprehensive IDE from Microsoft
- **Visual Studio Code** (optional): Lightweight editor with C# extensions

## File Extensions

- `.cs` - C# source files
- `.csproj` - C# project files
- `.sln` - Solution files (container for projects)
- `.dll` - .NET library files
- `.exe` - Windows executable files
- `.config`, `.json` - Configuration files
- `.resx` - Resource files

## Package Management

```bash
# Create a new project
dotnet new console -n MyProject

# Add a NuGet package
dotnet add package PackageName

# Add a specific version
dotnet add package PackageName --version 1.2.3

# Restore packages
dotnet restore

# Create a NuGet package
dotnet pack
```

## Running C# Programs

```bash
# Build the project
dotnet build

# Run the application
dotnet run

# Run with arguments
dotnet run -- arg1 arg2

# Publish a self-contained application
dotnet publish -c Release -r win-x64 --self-contained

# Run tests
dotnet test
```

## Common Libraries

- **Web Development**: ASP.NET Core, Blazor
- **Desktop**: WPF, Windows Forms, Avalonia UI
- **Data Access**: Entity Framework Core, Dapper
- **Testing**: xUnit, NUnit, MSTest
- **Utility**: Newtonsoft.Json, AutoMapper
- **Reactive**: Reactive Extensions (Rx.NET)
