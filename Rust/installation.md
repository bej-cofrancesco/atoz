# Rust Installation Guide

## Required Software

- **Rust**: Install using [rustup](https://rustup.rs/) (recommended)
- **Cargo**: Package manager (included with Rust installation)

## File Extensions

- `.rs` - Rust source files
- `.toml` - Configuration files (Cargo.toml)
- `.rlib` - Rust library files

## Package Management

```bash
# Create a new project
cargo new project_name

# Add dependencies in Cargo.toml:
# [dependencies]
# serde = "1.0"

# Update dependencies
cargo update

# Install a binary crate
cargo install crate_name
```

## Running Rust Programs

```bash
# Build project
cargo build

# Run project
cargo run

# Release build
cargo build --release

# Run tests
cargo test
```

## Common Libraries

- **Web**: Rocket, Actix, warp, tide
- **CLI**: clap, structopt
- **Serialization**: serde
- **Async**: tokio, async-std
- **Database**: sqlx, diesel, rusqlite
