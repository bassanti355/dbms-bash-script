# DBMS Script Project

## Overview

This project is a Bash script-based **Database Management System (DBMS)**. It allows users to create, list, connect to, and drop databases via a menu-driven interface. Within each database, users can perform operations such as creating tables, inserting, selecting, updating, and deleting records using external scripts.

---

## Features

1. **Database Management:**
   - Create a new database with a validated name.
   - List all existing databases.
   - Connect to a specific database.
   - Drop an existing database with a confirmation prompt.

2. **Table Management:**
   - Create tables (external script: `create_table`).
   - Drop tables (external script: `drop_table`).
   - Insert data into tables (external script: `insert_into_table`).
   - Select data from tables (external script: `select_table`).
   - Delete records from tables (external script: `delete_table`).
   - Update records in tables (external script: `update_table`).
   - List all tables in the database (external script: `list_table`).

3. **Validation:**
   - Database and table names must only contain letters, numbers, or underscores.
   - Ensures unique database names.

---

## Prerequisites

- **Operating System:** Linux or any system with Bash shell.
- **Environment Setup:**
  - Ensure you have a `~DBMS` directory or let the script create it automatically.
  - Create external scripts (`create_table`, `drop_table`, etc.) for table-level operations and place them in the working directory.

---

## Usage Instructions

1. Clone or copy the script to your system.
2. Make the script executable:
   ```bash
   chmod +x first_menu.sh

---

### Error Handling
- **Invalid Names:** Prompts the user to enter valid database/table names.
- **Non-Existent Resources:** Provides feedback if a requested database/table is not found.
- **Invalid Inputs:** Ensures user selections are within the expected range and format.

---
### Future Work
- Adding GUI to make it more user friendly
- Adding SQL query logic to the select, update, delete



