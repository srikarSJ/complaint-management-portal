# Complaint Management Portal

Java 17+ desktop complaint-management application built with Swing, JDBC, MySQL, Maven, FlatLaf and BCrypt.

## Project files

- `pom.xml` — Maven build configuration
- `src/main/java/` — application source code (33 Java files)
- `database/` — database schema and optional sample data
- `application.properties.example` — example local database configuration
- `package-windows.ps1` — script to build a Windows app-image
- `dist/README.txt` and `dist/Run Complaint Portal.bat` — Windows launch guidance
- `source-code/complaint-portal-source.tar.xz` — compressed bundle of the Java source tree and Windows packaging helpers

To extract the source bundle at the repository root, run:

```sh
tar -xJf source-code/complaint-portal-source.tar.xz
```

The source bundle includes `src/`, `package-windows.ps1`, and the two lightweight `dist/` helper files. It does not include the bundled runtime folders, project report, report images, or compiled JAR. Those binaries and report documents from the original upload have not been added to this repository yet.

## Requirements

- JDK 17 or later
- Maven 3.9+
- MySQL 8.0+

## Configure and run

1. Create a MySQL database named `complaint_portal` or allow the application to initialize it.
2. Copy `application.properties.example` to `application.properties` and set your database username and password. This local file is ignored by Git.
3. Build with:
   ```sh
   mvn clean package
   ```
4. Run the generated JAR from `target/`.

Do not commit local credentials or production passwords. Change the demonstration administrator password before using the application in a real environment.
