# Go Installation Guide

## Required Software

- **Go SDK**: The Go programming language toolchain
- **Git**: For version control and package management
- **VS Code**: With Go extension (recommended)
- **GoLand**: JetBrains IDE for Go (alternative)
- **delve**: Go debugger

## File Extensions

- `.go` - Go source code files
- `.mod` - Go module definition file (go.mod)
- `.sum` - Go module checksum file (go.sum)
- `.s` - Assembly files
- `.a` - Compiled package archives
- `.h` - C header files used with cgo
- `.c` - C source files used with cgo
- `.pb.go` - Generated Protocol Buffer files
- `.test` - Test binary
- `.out` - Default binary output filename (a.out)
- `.exe` - Windows executable

## Package Management

```bash
# Initialize a new module
go mod init module_name

# Add/update dependencies
go get package_name
go get package_name@v1.0.0

# Update all dependencies
go get -u ./...

# Tidy up unused dependencies
go mod tidy

# Vendor dependencies
go mod vendor

# List dependencies
go list -m all

# Clean module cache
go clean -modcache
```

## Running Go Programs

```bash
# Compile and run a Go program
go run main.go

# Build a Go program
go build

# Build for a specific platform
GOOS=linux GOARCH=amd64 go build

# Install a Go program
go install

# Run tests
go test ./...

# Run tests with coverage
go test -cover ./...

# Format code
go fmt ./...

# Vet code for potential issues
go vet ./...

# Generate code (e.g., for interfaces)
go generate ./...
```

## Common Libraries

- **Web Frameworks**: gin-gonic/gin, gorilla/mux, echo, fiber
- **Database**: gorm, sqlx, pgx
- **JSON/XML/Config**: encoding/json, encoding/xml, viper
- **CLI**: cobra, urfave/cli
- **Testing**: testify, gomock, go-sqlmock
- **HTTP Clients**: net/http, resty
- **Logging**: zap, logrus
- **Authentication**: golang-jwt/jwt, oauth2
- **GraphQL**: gqlgen, graphql-go
- **Validation**: validator
- **Concurrency**: sync, errgroup
