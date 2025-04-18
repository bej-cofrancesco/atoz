# Visual Basic Installation Guide

## Required Software

- **Visual Studio**: Microsoft's IDE with Visual Basic support
  - Community Edition (free)
  - Professional or Enterprise Edition (paid)
- **.NET Framework**: Windows-only .NET Framework
- **.NET Core/.NET 5+**: Cross-platform .NET implementation
- **Visual Studio Code**: Lightweight alternative with extensions
- **Rider**: JetBrains' cross-platform .NET IDE (alternative)
- **MonoDevelop**: Cross-platform IDE for Mono

## File Extensions

- `.vb` - Visual Basic source files
- `.vbproj` - Visual Basic project files
- `.sln` - Visual Studio solution files
- `.dll` - Compiled assembly files
- `.exe` - Executable files
- `.config` - Configuration files
- `.designer.vb` - Designer-generated code files
- `.resx` - Resource files
- `.vbx` - Visual Basic extension files (legacy)
- `.frm` - Form definition files (legacy VB6)
- `.vbhtml` - Razor view files for ASP.NET MVC
- `.aspx.vb` - ASP.NET code-behind files
- `.xaml.vb` - XAML code-behind files

## Package Management

```bash
# Using NuGet Package Manager in Visual Studio
# Right-click on project > Manage NuGet Packages

# Using .NET CLI
# Install a package
dotnet add package PackageName

# Install specific version
dotnet add package PackageName --version 1.2.3

# Remove a package
dotnet remove package PackageName

# List installed packages
dotnet list package

# Restore packages
dotnet restore

# Update packages
dotnet add package PackageName --version Latest
```

## Running Visual Basic Programs

```bash
# Compile a VB.NET file with the .NET CLI
dotnet build

# Run a VB.NET application
dotnet run

# Run with arguments
dotnet run -- arg1 arg2

# Create a release build
dotnet build -c Release

# Publish a standalone application
dotnet publish -c Release -r win-x64 --self-contained

# Run unit tests
dotnet test

# Run with Visual Studio
# Press F5 or click on the Start button

# Create a new VB.NET Console Application
dotnet new console -lang VB -o MyProject

# Create a new VB.NET Web Application
dotnet new webapp -lang VB -o MyWebApp
```

## Common Libraries

- **Core**: .NET Base Class Library
- **Windows Forms**: Desktop UI framework (Windows)
- **WPF**: Windows Presentation Foundation (Windows)
- **ASP.NET**: Web development framework
- **Entity Framework**: ORM for database access
- **LINQ**: Language-Integrated Query
- **ADO.NET**: Data access technology
- **System.IO**: File and stream operations
- **System.Net**: Network communications
- **System.XML**: XML processing
- **System.JSON**: JSON processing
- **NUnit/xUnit/MSTest**: Testing frameworks
- **NLog/log4net**: Logging frameworks
- **Newtonsoft.Json**: Popular JSON library
- **ML.NET**: Machine learning library
- **Blazor**: Web UI framework
