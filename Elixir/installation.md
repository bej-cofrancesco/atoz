# Elixir Installation Guide

## Required Software

- **Erlang/OTP**: Required runtime for Elixir
- **Elixir**: The language itself
- **Mix**: Build tool (included with Elixir)
- **VS Code** (recommended): With ElixirLS extension
- **asdf** (optional): Version manager for Erlang and Elixir

## File Extensions

- `.ex` - Elixir source code files (compiled)
- `.exs` - Elixir script files (interpreted)
- `.eex` - Embedded Elixir templates
- `.leex` - Live Embedded Elixir templates
- `.heex` - HTML Embedded Elixir templates
- `.beam` - Compiled Elixir/Erlang bytecode
- `mix.exs` - Mix project configuration
- `mix.lock` - Dependency lock file

## Package Management

```bash
# Create a new Elixir project
mix new project_name

# Create a new Phoenix (web) project
mix phx.new web_app_name

# Add a dependency (edit mix.exs, then run:)
mix deps.get

# Update dependencies
mix deps.update

# Compile the project
mix compile

# Clean compiled artifacts
mix clean
```

## Running Elixir Programs

```bash
# Run an Elixir script
elixir script.exs

# Run a mix application
mix run

# Start an interactive Elixir shell
iex

# Start an interactive Elixir shell with your application loaded
iex -S mix

# Start a Phoenix server
mix phx.server

# Run tests
mix test

# Generate a release
mix release
```

## Common Libraries

- **Web Development**: Phoenix, Plug, Absinthe (GraphQL)
- **Data Processing**: Ecto, Flow, Broadway
- **Testing**: ExUnit, Mox
- **HTTP Clients**: HTTPoison, Tesla, Finch
- **JSON**: Jason, Poison
- **Utilities**: Timex (dates/times), ex_doc (documentation)
