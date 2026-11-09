# Bank of Lebanon JavaFX App

## Overview

This desktop banking simulation puts the user in the role of an employee working with client and account records. The JavaFX interface brings searches, tables, and forms into one window, while SQLite gives the records a local home. The code also models employees, loans, and interest, showing how a desktop UI can sit on top of a domain model and a database.

## How it’s built

- **Desktop interaction.** The [JavaFX application](src/main/java/com/bank/bank_of_lebanon/BankOfLebanonEmployeeApplication.java) uses observable lists, filtered and sorted tables, and dialogs to work with records.
- **Java and SQL.** Client, account, and employee models sit alongside JDBC classes that read and update the local SQLite database.
- **Build.** Maven manages JavaFX and the SQLite JDBC dependency.

## Run or explore locally

From the repository root, use JDK 19 and Maven, then run `mvn clean javafx:run`. The repository includes `database.db`. The source and [Maven configuration](pom.xml) are the starting points for inspecting the database and UI setup.
