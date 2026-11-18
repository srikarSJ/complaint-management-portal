# Complaint Management Portal

Java-based desktop application for managing complaints, users, and administrative workflows.

## Project contents
- Java source code (`src/`)
- Database schema and sample data (`database/`)
- Project report (PDF and DOCX) and diagrams (`Project_Report/`)
- Maven build configuration (`pom.xml`)
- Example configuration (`application.properties.example`)

## Build
Install JDK 17+ and Maven, then run:

```bash
mvn clean package
```

## Configuration
Copy `application.properties.example` to `application.properties` and fill in your local database settings. Do not commit local credentials.

## Windows packaging
The `package-windows.ps1` script can be used to generate a Windows package. Generated runtime bundles and build outputs are excluded from version control to avoid committing large duplicate binaries.
