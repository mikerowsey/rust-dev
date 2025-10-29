# Rust Dev Container Template

A ready-to-use Rust development environment using VS Code Dev Containers.

## What's Included

- **Rust** - Latest stable toolchain
- **Cargo** - Rust package manager
- **VS Code Extensions**:
  - rust-analyzer (language server)
  - CodeLLDB (debugger)
  - Even Better TOML
  - crates (dependency management helper)
- **Shell**: zsh with oh-my-zsh
- **Git & GitHub CLI**: Pre-installed

## How to Use

1. **Clone this template**
2. **Open in VS Code**
3. **Click "Reopen in Container"** when prompted
4. **Create new project**: `cargo new my-project`
5. **Start coding!**

## Quick Start

```bash
# The container includes a sample "hello" binary
cargo run

# Create a new project
cargo new --bin my-app
cd my-app
cargo run
```

## Clippy Integration

The container is configured to use `clippy` for linting. Run:

```bash
cargo clippy
```
