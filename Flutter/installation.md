# Flutter Installation Guide

## Required Software

- **Flutter SDK**: The Flutter framework and tools
- **Dart SDK**: Included with Flutter installation
- **Android Studio**: For Android development
- **Xcode**: For iOS development (macOS only)
- **VS Code**: With Flutter extension (recommended)
- **IntelliJ IDEA/Android Studio**: With Flutter plugin (alternative)
- **Git**: Required for Flutter installation
- **Android/iOS Emulators**: For testing without physical devices

## File Extensions

- `.dart` - Dart source code files
- `.yaml`, `.yml` - Configuration files (pubspec.yaml, etc.)
- `.json` - JSON configuration files
- `.g.dart` - Generated Dart files (code generation)
- `.freezed.dart` - Freezed generated files
- `.arb` - Application Resource Bundle (localization)
- `.iml` - IntelliJ module files
- `.gradle` - Gradle build files (Android)
- `.pbxproj` - Xcode project files (iOS)
- `.swift` - Swift source code (iOS platform code)
- `.kt`, `.java` - Kotlin/Java source code (Android platform code)
- `.png`, `.jpg`, `.svg` - Image assets
- `.ttf`, `.otf` - Font files
- `.lock` - Lock files for dependencies
- `.metadata` - Flutter metadata files

## Package Management

```bash
# Install Flutter SDK (macOS/Linux)
git clone https://github.com/flutter/flutter.git
export PATH="$PATH:`pwd`/flutter/bin"

# Install Flutter SDK (Windows)
git clone https://github.com/flutter/flutter.git
# Add flutter\bin to your PATH

# Check installation and dependencies
flutter doctor

# Fix any issues reported by flutter doctor

# Create a new Flutter project
flutter create my_app

# Add a package dependency to pubspec.yaml
# dependencies:
#   provider: ^6.0.0

# Install dependencies
flutter pub get

# Upgrade dependencies
flutter pub upgrade

# Add dev dependencies
# dev_dependencies:
#   flutter_test:
#     sdk: flutter
#   build_runner: ^2.0.0

# Install a specific version
# dependencies:
#   http: ^0.13.4
```

## Running Flutter Programs

```bash
# Run Flutter app in debug mode
flutter run

# Run on a specific device when multiple are connected
flutter devices
flutter run -d device_id

# Run with release configuration
flutter run --release

# Run with profile mode (performance testing)
flutter run --profile

# Build an Android APK
flutter build apk

# Build an Android App Bundle
flutter build appbundle

# Build an iOS app (macOS only)
flutter build ios

# Build a web app
flutter build web

# Run tests
flutter test

# Run a specific test file
flutter test test/widget_test.dart

# Clean build files
flutter clean

# Analyze code for issues
flutter analyze
```

## Common Libraries

- **Flutter SDK**: Core Flutter framework
- **Material/Cupertino**: UI component libraries
- **Provider/Riverpod**: State management
- **Bloc**: State management pattern
- **GetX**: State management, routing, and dependencies
- **Dio/Http**: HTTP clients
- **Firebase**: Google's app development platform
- **Hive/SQLite**: Local storage solutions
- **Flutter_hooks**: React-like hooks
- **GoRouter/AutoRoute**: Navigation and routing
- **Flutter_form_builder**: Form management
- **Intl**: Internationalization and localization
- **Image_picker**: Access device gallery and camera
- **Shared_preferences**: Persistent key-value storage
- **Flutter_svg**: SVG rendering
- **Google_maps_flutter**: Maps integration
- **Permission_handler**: Request and check permissions
