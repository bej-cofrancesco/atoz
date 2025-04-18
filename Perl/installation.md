# Perl Installation Guide

## Required Software

- **Perl Interpreter**: The Perl programming language
- **CPAN**: Comprehensive Perl Archive Network
- **cpanm**: CPAN Minus, a script to get, unpack, build and install modules from CPAN
- **VS Code**: With Perl extension (recommended)
- **Padre**: Perl Application Development and Refactoring Environment (IDE)
- **Perlbrew**: Tool to manage multiple Perl installations

## File Extensions

- `.pl` - Perl scripts
- `.pm` - Perl modules
- `.t` - Perl test files
- `.pod` - Plain Old Documentation
- `.cgi` - CGI scripts
- `.psgi` - PSGI web application files
- `.xs` - Perl XS (interface to C/C++ libraries)
- `.PL` - Perl scripts that generate other files
- `.al` - Perl autoload functions
- `Makefile.PL` - Perl Makefile generator
- `cpanfile` - CPAN dependencies file

## Package Management

```bash
# Install modules with CPAN
cpan Module::Name

# Install modules with cpanm (recommended)
cpanm Module::Name

# Install specific version
cpanm Module::Name@1.2

# Install from local directory
cpanm .

# Install with dependencies
cpanm --installdeps .

# Install in a local directory (no root required)
cpanm -l ~/perl5 Module::Name

# Using Carton (for application dependencies)
cpanm Carton
carton install
```

## Running Perl Programs

```bash
# Run a Perl script
perl script.pl

# Run with warnings and strict mode
perl -w -strict script.pl

# Check syntax without running
perl -c script.pl

# Run with debugging
perl -d script.pl

# Run as a one-liner
perl -e 'print "Hello, World!\n"'

# Run with modules from specific directories
perl -I /path/to/lib script.pl

# Run PSGI application with Plack
plackup app.psgi
```

## Common Libraries

- **Web Frameworks**: Mojolicious, Catalyst, Dancer
- **ORM**: DBIx::Class, Rose::DB
- **Template Systems**: Template Toolkit, Mason, HTML::Template
- **Testing**: Test::More, Test::Simple, Test2
- **XML/HTML Processing**: XML::LibXML, HTML::Parser
- **JSON**: JSON, JSON::XS, Cpanel::JSON::XS
- **Database**: DBI, DBD::\* drivers
- **CLI**: Getopt::Long, Pod::Usage
- **HTTP Clients**: LWP, HTTP::Tiny, Mojo::UserAgent
- **Async**: AnyEvent, IO::Async, Mojo::IOLoop
- **DateTime Handling**: DateTime, Time::Piece
- **Text Processing**: Text::CSV, Text::Diff
- **Email**: Email::Sender, Email::MIME
