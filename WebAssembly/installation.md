# WebAssembly Installation Guide

## Required Software

- **Web Browser**: Modern browsers with WebAssembly support
  - Chrome, Firefox, Safari, Edge
- **Compilers/Toolchains**:
  - **Emscripten**: C/C++ to WebAssembly compiler (recommended)
  - **Rust**: With WebAssembly target
  - **AssemblyScript**: TypeScript-like language for WebAssembly
  - **Go**: With WebAssembly support
  - **Wat2Wasm**: WebAssembly text format converter
- **Node.js**: For server-side WebAssembly (with WASI)
- **VS Code**: With WebAssembly extensions
- **Wasmtime/Wasmer/WAVM**: WebAssembly runtimes

## File Extensions

- `.wasm` - WebAssembly binary format
- `.wat` - WebAssembly text format
- `.wast` - WebAssembly script format
- `.c`, `.cpp` - C/C++ source files for compilation to WebAssembly
- `.rs` - Rust source files
- `.ts` - AssemblyScript source files
- `.js` - JavaScript files for WebAssembly integration
- `.html` - HTML files loading WebAssembly modules
- `.wasm.map` - Source maps for WebAssembly
- `.d.ts` - TypeScript declaration files
- `.cargo/config` - Rust WebAssembly configuration
- `Cargo.toml` - Rust project manifest
- `package.json` - Node.js/AssemblyScript configuration
- `CMakeLists.txt` - CMake build configuration for C/C++

## Package Management

```bash
# Install Emscripten SDK
git clone https://github.com/emscripten-core/emsdk.git
cd emsdk
./emsdk install latest
./emsdk activate latest
source ./emsdk_env.sh  # On Windows: emsdk_env.bat

# Install AssemblyScript
npm install --global assemblyscript

# Install Rust with WebAssembly target
rustup target add wasm32-unknown-unknown
rustup target add wasm32-wasi  # For WASI target

# Install wasm-pack for Rust
cargo install wasm-pack

# Install wasm-bindgen-cli for Rust
cargo install wasm-bindgen-cli

# Install Binaryen (optimization tools)
npm install -g binaryen

# Install Wasmtime runtime
curl https://wasmtime.dev/install.sh -sSf | bash

# Install Wasmer runtime
curl https://get.wasmer.io -sSfL | sh
```

## Running WebAssembly Programs

```bash
# Compile C/C++ to WebAssembly with Emscripten
emcc hello.c -o hello.html

# Compile AssemblyScript to WebAssembly
asc hello.ts -o hello.wasm

# Compile Rust to WebAssembly
cargo build --target wasm32-unknown-unknown
wasm-bindgen --target web target/wasm32-unknown-unknown/debug/hello.wasm

# Convert WebAssembly text format to binary
wat2wasm hello.wat -o hello.wasm

# Run WebAssembly in browser
# Include in HTML:
# <script>
#   WebAssembly.instantiateStreaming(fetch('hello.wasm'))
#     .then(obj => obj.instance.exports.main());
# </script>

# Run WebAssembly with Node.js
node --experimental-wasm-modules program.js

# Run WebAssembly with Wasmtime
wasmtime hello.wasm

# Run WebAssembly with Wasmer
wasmer hello.wasm
```

## Common Libraries

- **wasm-bindgen**: Rust-WebAssembly interoperability
- **Emscripten Runtime**: C/C++ standard library support
- **Web APIs**: Browser APIs accessible from WebAssembly
- **wasm-pack**: Rust to WebAssembly packaging
- **WASI**: WebAssembly System Interface
- **AssemblyScript Runtime**: Standard library for AssemblyScript
- **Cranelift**: Code generator used in WebAssembly runtimes
- **Binaryen**: Compiler infrastructure and toolchain
- **wasm3**: Lightweight WebAssembly interpreter
- **Wabt**: WebAssembly Binary Toolkit
- **wasm-micro-runtime**: Small footprint interpreter
- **Wasmer/Wasmtime**: WebAssembly runtimes
- **Wasmer-js**: WebAssembly runtime for JavaScript
- **Lucet**: Native WebAssembly compiler and runtime
- **TensorFlow.js**: Machine learning with WebAssembly
