# C++ Installation Guide

## Required Software

- **C++ Compiler**:
  - **Windows**: MinGW-w64 or MSVC (Visual Studio)
  - **macOS**: Clang (included with Xcode Command Line Tools)
  - **Linux**: GCC (install via package manager)
- **CMake**: Cross-platform build system generator

## File Extensions

- `.cpp`, `.cc`, `.cxx` - C++ source files
- `.h`, `.hpp`, `.hxx` - Header files
- `.o`, `.obj` - Object files
- `.a`, `.lib` - Static library
- `.so`, `.dll`, `.dylib` - Dynamic/shared library
- `.cmake`, `CMakeLists.txt` - CMake configuration files

## Package Management

```bash
# CMake
# Create a new project with CMakeLists.txt:
# cmake_minimum_required(VERSION 3.10)
# project(MyProject)
# add_executable(my_app main.cpp)

# Configure build
mkdir build && cd build
cmake ..

# Build project
cmake --build .

# Conan (C++ package manager)
# Install Conan
pip install conan

# Create conanfile.txt:
# [requires]
# fmt/8.1.1
# [generators]
# cmake

# Install dependencies
conan install . --build=missing
```

## Running C++ Programs

```bash
# Compile with g++
g++ -o program main.cpp

# Compile with flags
g++ -std=c++17 -Wall -O2 -o program main.cpp

# Run the program
./program

# Run with CMake
cd build
./my_app
```

## Common Libraries

- **Standard Library**: STL (containers, algorithms, iterators)
- **GUI**: Qt, wxWidgets, FLTK
- **Graphics**: OpenGL, Vulkan, SFML
- **Data Formats**: nlohmann/json, tinyxml, Protobuf
- **Testing**: Catch2, Google Test, Boost.Test
- **Networking**: Boost.Asio, libcurl, gRPC
