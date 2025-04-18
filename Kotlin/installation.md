# Kotlin Installation Guide

## Required Software

- **JDK**: Java Development Kit 8 or newer (https://www.oracle.com/java/technologies/downloads/)
- **Kotlin Compiler**: The Kotlin command-line compiler (https://github.com/JetBrains/kotlin/releases)
- **IntelliJ IDEA**: IDE with built-in Kotlin support (recommended) (https://www.jetbrains.com/idea/)
- **Android Studio**: For Android development with Kotlin (https://developer.android.com/studio)
- **Gradle**: Build automation tool for Kotlin projects (https://gradle.org/install/)
- **Maven**: Alternative build tool (https://maven.apache.org/download.cgi)

## File Extensions

- `.kt` - Kotlin source code files
- `.kts` - Kotlin script files
- `.ktm` - Kotlin module files
- `.klib` - Kotlin library files
- `.jar` - Java Archive files (used for compiled Kotlin code)
- `.class` - Java class files (compiled Kotlin code)
- `.gradle.kts` - Gradle build scripts written in Kotlin
- `.main.kts` - Main Kotlin script files

## Package Management

```bash
# Using Gradle (recommended)
# Initialize a new Gradle project with Kotlin
gradle init --type kotlin-application

# Using Maven
# Create from archetype
mvn archetype:generate -DarchetypeGroupId=org.jetbrains.kotlin -DarchetypeArtifactId=kotlin-archetype-jvm

# Using SDKMAN (to install Kotlin)
sdk install kotlin

# Using Homebrew (on macOS)
brew install kotlin

# Using Kotlinc directly
kotlinc HelloWorld.kt -include-runtime -d HelloWorld.jar
```

## Running Kotlin Programs

```bash
# Compile and run using kotlinc
kotlinc HelloWorld.kt -include-runtime -d HelloWorld.jar
java -jar HelloWorld.jar

# Run Kotlin script directly
kotlin script.kts

# Run using Gradle
./gradlew run

# Run using Maven
mvn exec:java

# Compile without creating a JAR
kotlinc HelloWorld.kt -d classes
kotlin -classpath classes HelloWorldKt

# REPL (interactive console)
kotlinc

# REPL with dependencies
kotlinc-jvm -cp dependency.jar
```

## Common Libraries

- **Web Development**: Ktor, Spring Boot, Javalin, Micronaut
- **Android**: Android Jetpack, KTX, Compose
- **Testing**: JUnit, Kotest, Mockk, Spek
- **Coroutines**: kotlinx.coroutines
- **Serialization**: kotlinx.serialization, Jackson, Gson, Moshi
- **Dependency Injection**: Koin, Kodein, Dagger
- **Database**: Exposed, JDBC, Room (Android), ktorm
- **HTTP Clients**: Ktor Client, Retrofit, OkHttp
- **Functional Programming**: Arrow
- **Multiplatform**: Kotlin Multiplatform Mobile (KMM)
- **Image Processing**: Skija, KorGE
- **Data Science**: Kotlin for Apache Spark, KotlinDL
- **Utilities**: kotlinx.datetime, kotlinx.collections.immutable
- **Reactive Programming**: RxKotlin, Reaktive, Flow
