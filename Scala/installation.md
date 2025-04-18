# Scala Installation Guide

## Required Software

- **Java Development Kit (JDK)**: Version 8 or higher required for Scala
- **Scala**: The Scala compiler and runtime
- **sbt**: Scala Build Tool for dependency management
- **IntelliJ IDEA**: With Scala plugin (recommended IDE)
- **VS Code**: With Metals extension (alternative)
- **Coursier**: Command-line installer for Scala

## File Extensions

- `.scala` - Scala source files
- `.sc` - Scala script files
- `.sbt` - SBT build definition files
- `.class` - Compiled JVM bytecode
- `.jar` - Java/Scala Archive (compiled code)
- `.scala-build` - Scala CLI build directory
- `build.sbt` - SBT project configuration
- `project/` - SBT project directory
- `.scalafmt.conf` - Scala formatter configuration
- `.metals/` - Metals language server cache
- `.bloop/` - Bloop compilation server files
- `.worksheet.sc` - Scala worksheet files

## Package Management

```bash
# Install Scala using Coursier (recommended)
curl -fL https://github.com/coursier/launchers/raw/master/cs-x86_64-apple-darwin.gz | gzip -d > cs
chmod +x cs
./cs setup

# Create a new SBT project
sbt new scala/scala-seed.g8

# Create a new Scala 3 project
sbt new scala/scala3.g8

# Add a library dependency in build.sbt
# libraryDependencies += "org.typelevel" %% "cats-core" % "2.7.0"

# Update dependencies
sbt update

# Install a plugin in project/plugins.sbt
# addSbtPlugin("org.scalameta" % "sbt-scalafmt" % "2.4.6")

# Using Mill (alternative build tool)
mill init
```

## Running Scala Programs

```bash
# Compile a Scala file
scalac HelloWorld.scala

# Run a compiled Scala program
scala HelloWorld

# Run the Scala REPL
scala

# Run a Scala script
scala script.sc

# Using SBT
# Compile
sbt compile

# Run
sbt run

# Run with arguments
sbt "run arg1 arg2"

# Run tests
sbt test

# Package a JAR file
sbt package

# Create an executable JAR
sbt assembly

# Using Scala CLI (modern tool)
scala-cli run HelloWorld.scala

# Continuous compilation
sbt ~compile
```

## Common Libraries

- **Cats**: Functional programming abstractions
- **ZIO**: Effect system for functional programming
- **Akka**: Actor-based concurrency and streaming
- **Play Framework**: Web application framework
- **Spark**: Big data processing
- **http4s**: HTTP server and client
- **Circe**: JSON processing
- **ScalaTest/Specs2**: Testing frameworks
- **FS2**: Functional streaming
- **Slick**: Database access
- **ScalaCheck**: Property-based testing
- **Shapeless**: Generic programming
- **Monix**: Asynchronous programming
- **Doobie**: Functional JDBC layer
- **Chimney**: Data transformation
