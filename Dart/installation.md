# Dart Installation Guide

## Required Software

- **Dart SDK**: Download from [dart.dev](https://dart.dev/get-dart)
- **Flutter SDK** (optional): For mobile, web, and desktop app development
- **VS Code** (recommended): With Dart and Flutter extensions
- **Android Studio** (optional): For Flutter mobile development

## File Extensions

- `.dart` - Dart source files
- `.dart.js` - Compiled JavaScript from Dart code
- `.g.dart` - Generated Dart code (typically by build_runner)
- `.freezed.dart` - Generated code from freezed package
- `.mocks.dart` - Generated mock classes for testing
- `pubspec.yaml` - Package configuration file
- `analysis_options.yaml` - Linter and analyzer configuration

## Package Management

```bash
# Initialize a new Dart project
dart create my_project

# Initialize a new Flutter project
flutter create my_flutter_app

# Add a package dependency
dart pub add package_name

# Add a dev dependency
dart pub add --dev test

# Install all dependencies
dart pub get

# Upgrade dependencies
dart pub upgrade

# Run code generators
dart run build_runner build
```

## Running Dart Programs

```bash
# Run a Dart script
dart run bin/main.dart

# Run a specific file
dart filename.dart

# Run with arguments
dart filename.dart arg1 arg2

# Compile to native executable
dart compile exe bin/main.dart -o my_app

# Compile to JavaScript
dart compile js -o main.js bin/main.dart

# Start a development server (for web apps)
webdev serve
```

## Common Libraries

- **Core**: dart:core, dart:async, dart:io, dart:convert
- **HTTP & Networking**: http, dio
- **State Management**: provider, riverpod, bloc
- **Data Serialization**: json_serializable, freezed
- **Database**: sqflite, Hive, Isar
- **Testing**: test, mockito, mocktail
