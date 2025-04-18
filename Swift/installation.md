# Swift Installation Guide

## Required Software

- **Swift Toolchain**: The Swift compiler and standard library
- **Xcode**: IDE for macOS/iOS development (macOS only)
- **Swift Package Manager**: Dependency manager included with Swift
- **VS Code**: With Swift extension (cross-platform alternative)
- **AppCode**: JetBrains' IDE for Swift (alternative)
- **LLDB**: Debugger (included with Swift)

## File Extensions

- `.swift` - Swift source files
- `.swiftmodule` - Compiled Swift module files
- `.swiftinterface` - Swift module interface files
- `.swiftdoc` - Swift documentation files
- `.swiftsourceinfo` - Swift source information
- `.xcodeproj` - Xcode project file
- `.xcworkspace` - Xcode workspace file
- `.playground` - Swift playground files
- `.framework` - Framework bundle
- `.xctest` - XCTest bundle
- `Package.swift` - Swift Package Manager manifest
- `.swiftpm` - Swift Package Manager files
- `.a`, `.dylib`, `.so` - Static and dynamic libraries

## Package Management

```bash
# Create a new Swift package
swift package init --type executable

# Initialize a library package
swift package init --type library

# Build a Swift package
swift build

# Add a dependency to Package.swift
# dependencies: [
#    .package(url: "https://github.com/Alamofire/Alamofire.git", from: "5.0.0"),
# ],

# Update dependencies
swift package update

# Resolve dependencies
swift package resolve

# Generate Xcode project from a package
swift package generate-xcodeproj

# Edit a package in Xcode
swift package xcode

# Show dependencies
swift package show-dependencies
```

## Running Swift Programs

```bash
# Compile a Swift file
swiftc main.swift -o program

# Run a compiled Swift program
./program

# Compile and run in one step
swift main.swift

# Run in Swift REPL
swift

# Run with Swift Package Manager
swift run

# Run with arguments
swift run MyProgram arg1 arg2

# Run tests
swift test

# Run with Xcode on macOS
# Open .xcodeproj or .xcworkspace and press Run

# Debug with LLDB
swift -g main.swift
lldb ./main
```

## Common Libraries

- **Foundation**: Basic data types and utilities
- **Swift Standard Library**: Built-in types and functions
- **UIKit**: iOS/tvOS user interface
- **AppKit**: macOS user interface
- **SwiftUI**: Declarative UI framework
- **Combine**: Reactive programming framework
- **Alamofire**: HTTP networking
- **SwiftyJSON**: JSON handling
- **SwiftNIO**: Asynchronous I/O framework
- **Vapor/Kitura/Perfect**: Web frameworks
- **CoreData**: Data persistence
- **RxSwift**: Reactive extensions
- **SnapKit**: Auto layout DSL
- **Realm**: Mobile database
- **Firebase**: Mobile backend services
- **Kingfisher**: Image loading and caching
