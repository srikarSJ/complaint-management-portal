# Complaint Management Portal

Java 17+ desktop complaint-management application built with Swing, JDBC, MySQL, Maven, FlatLaf and BCrypt.

## Repository status

This repository currently contains the Maven configuration, database scripts, example configuration, `.gitignore`, `.gitattributes` and this README. The Java source directory (`src/`), project report, diagrams, screenshots and packaged application are **not yet committed**.

To complete the repository, extract the prepared `project_payload.zip` package and upload its contents to the repository root using **Add file → Upload files**. The package contains the source code, SQL, Maven files, project report, diagrams, screenshots and a runnable JAR. The five duplicate bundled Windows Java runtime folders are intentionally excluded because they add hundreds of megabytes of repeated generated binaries.

## Requirements

- JDK 17 or later
- Maven 3.9+
- MySQL 8.0+

## Configure and run

1. Create a MySQL database named `complaint_portal` or allow the application to initialize it.
2. Copy `application.properties.example` to `application.properties` and set the database username and password.
3. Build with `mvn clean package`.
4. Run the generated JAR from `target/`.

`application.properties` is intentionally ignored by Git. Do not commit local credentials or production passwords.
