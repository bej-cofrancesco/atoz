# Clojure Installation Guide

## Required Software

- **Java Development Kit (JDK)**: Version 8 or newer
- **Clojure CLI Tools**: [clojure.org/guides/getting_started](https://clojure.org/guides/getting_started)
- **Leiningen**: Alternative build tool [leiningen.org](https://leiningen.org/)

## File Extensions

- `.clj` - Clojure source files
- `.cljc` - Cross-platform Clojure (JVM, ClojureScript)
- `.cljs` - ClojureScript source files
- `.edn` - Extensible Data Notation files
- `.jar` - Java Archive (compiled Clojure)
- `deps.edn` - Dependencies file for Clojure CLI
- `project.clj` - Leiningen project file

## Package Management

```bash
# With Clojure CLI tools
# Create deps.edn:
# {:deps {org.clojure/clojure {:mvn/version "1.11.1"}
#         other/dependency {:mvn/version "1.0.0"}}}

# Get dependencies
clj -P

# With Leiningen
# Create a new project
lein new app my-project

# Install dependencies (defined in project.clj)
lein deps
```

## Running Clojure Programs

```bash
# Run with Clojure CLI
clj -M -m namespace.core

# Start a REPL with Clojure CLI
clj

# Run with Leiningen
lein run

# Start a REPL with Leiningen
lein repl

# Create an uberjar (standalone JAR)
lein uberjar
java -jar target/uberjar/my-app-0.1.0-standalone.jar
```

## Common Libraries

- **Web Development**: Ring, Compojure, Pedestal, Reitit
- **Database**: next.jdbc, HoneySQL, Datomic
- **HTTP Clients**: clj-http, httpkit
- **Data Processing**: core.async, Specter
- **Testing**: clojure.test, test.check
