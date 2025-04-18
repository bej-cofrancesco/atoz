# Erlang Installation Guide

## Required Software

- **Erlang/OTP**: The Erlang Open Telecom Platform
- **Rebar3**: Build tool for Erlang projects
- **VS Code**: With Erlang extension (recommended)
- **IntelliJ IDEA**: With Erlang plugin (alternative)
- **Erlang LS**: Erlang Language Server

## File Extensions

- `.erl` - Erlang source files
- `.hrl` - Erlang header files
- `.beam` - Compiled Erlang bytecode
- `.app` - Application resource file
- `.app.src` - Application resource template
- `.config` - Erlang config files
- `.escript` - Erlang script files
- `.xrl` - Leex lexical analyzer files
- `.yrl` - Yecc parser generator files
- `rebar.config` - Rebar3 project configuration

## Package Management

```bash
# Using Rebar3
# Create a new project
rebar3 new app myapp

# Fetch dependencies
rebar3 get-deps

# Update dependencies
rebar3 upgrade

# Compile the project
rebar3 compile

# Using Hex (Erlang package manager)
# Add a dependency to rebar.config:
# {deps, [{some_dep, "0.1.0"}]}.

# Publish a package to Hex
rebar3 hex publish
```

## Running Erlang Programs

```bash
# Compile and run using Erlang
erlc module.erl
erl -noshell -s module start -s init stop

# Compile using rebar3
rebar3 compile

# Run in Erlang shell
erl
> application:start(myapp).

# Run with rebar3
rebar3 shell
> application:start(myapp).

# Run tests
rebar3 eunit
rebar3 ct

# Create a release
rebar3 release
```

## Common Libraries

- **Web Development**: Cowboy, Mochiweb, Webmachine
- **Testing**: Common Test, EUnit, PropEr
- **Database**: mnesia, epgsql (PostgreSQL client)
- **JSON**: jsx, jiffy, jason
- **HTTP Clients**: hackney, gun
- **ORM**: sumo_db
- **Message Queues**: RabbitMQ client
- **Parsing**: leex, yecc
- **Monitoring**: recon, folsom
- **Distributed Systems**: partisan, lasp
