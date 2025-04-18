# OCaml Installation Guide

## Required Software

- **OCaml Compiler**: The OCaml programming language
- **OPAM**: OCaml Package Manager
- **Dune**: Build system for OCaml projects
- **OCaml LSP**: Language server for IDE integration
- **VS Code**: With OCaml Platform extension (recommended)
- **Emacs**: With Tuareg mode (alternative)
- **Merlin**: Context-sensitive completion for OCaml

## File Extensions

- `.ml` - OCaml implementation files
- `.mli` - OCaml interface files
- `.mll` - OCamllex lexer definitions
- `.mly` - OCamlyacc parser definitions
- `.cma` - OCaml bytecode library
- `.cmxa` - OCaml native library
- `.cmi` - Compiled interface files
- `.cmo` - Compiled bytecode object files
- `.cmx` - Compiled native object files
- `.cmxs` - Dynamically loadable native plugins
- `.o`, `.a`, `.so` - Generated C artifacts
- `dune` - Dune build configuration files
- `dune-project` - Dune project file
- `opam` - OPAM package definition files

## Package Management

```bash
# Install OPAM (OCaml Package Manager)
# Linux (Ubuntu/Debian)
sudo apt install opam

# macOS
brew install opam

# Initialize OPAM
opam init

# Set up environment
eval $(opam env)

# Install a specific OCaml version
opam switch create 4.14.0

# Install packages
opam install dune merlin ocaml-lsp-server odoc utop

# Create a new project with dune
dune init project myproject

# Install a specific package
opam install package_name

# Update packages
opam update
opam upgrade

# List installed packages
opam list
```

## Running OCaml Programs

```bash
# Compile and run a single file
ocamlc -o program program.ml
./program

# Compile to native code
ocamlopt -o program program.ml
./program

# Run in the OCaml interpreter
ocaml program.ml

# Use the interactive toplevel
ocaml

# Use UTop (enhanced toplevel)
utop

# Build a project with dune
dune build

# Run a program with dune
dune exec program_name

# Run tests with dune
dune runtest

# Generate documentation
dune build @doc
```

## Common Libraries

- **Core/Base**: Jane Street's alternative standard libraries
- **Lwt/Async**: Concurrent programming libraries
- **Cmdliner**: Command-line argument parsing
- **Yojson/Jsonm**: JSON processing
- **Cohttp/HTTP**: HTTP clients and servers
- **Ppx**: Syntax extensions and preprocessors
- **Graphics**: Simple graphics library
- **OUnit**: Unit testing framework
- **Ocamlgraph**: Graph library
- **OCaml-re**: Regular expressions
- **Menhir**: Parser generator
- **Cairo**: Bindings to the Cairo graphics library
- **Batteries Included**: Extended standard library
- **React**: Functional reactive programming
