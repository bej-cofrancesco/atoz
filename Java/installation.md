# Java Installation Guide

## Required Software

- **JDK**: Install Java Development Kit from [Oracle](https://www.oracle.com/java/technologies/downloads/) or [OpenJDK](https://adoptium.net/) (version 11+ recommended)
- **Maven/Gradle**: Build automation tools (download separately)

## File Extensions

- `.java` - Java source files
- `.class` - Compiled Java bytecode files
- `.jar` - Java Archive (executable or library)
- `.war` - Web Application Archive
- `.pom` - Maven Project Object Model file
- `.gradle` - Gradle build script files
- `.properties` - Configuration files

## Package Management

```bash
# Maven
# Create a project from archetype
mvn archetype:generate -DgroupId=com.example -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

# Add dependencies in pom.xml:
# <dependency>
#   <groupId>group-id</groupId>
#   <artifactId>artifact-id</artifactId>
#   <version>version</version>
# </dependency>

# Install dependencies
mvn install

# Gradle
# Initialize a new project
gradle init

# Add dependencies in build.gradle:
# dependencies {
#   implementation 'group:name:version'
# }
```

## Running Java Programs

```bash
# Compile a Java file
javac Main.java

# Run a Java class
java Main

# Run a JAR file
java -jar app.jar

# With Maven
mvn exec:java -Dexec.mainClass="com.example.Main"

# With Gradle
gradle run
```

## Common Libraries

- **Web Frameworks**: Spring Boot, Jakarta EE, Micronaut, Quarkus
- **ORM**: Hibernate, JPA
- **Testing**: JUnit, Mockito, TestNG
- **Utilities**: Apache Commons, Guava, Lombok
- **Concurrency**: Akka, Java Concurrency Utilities
