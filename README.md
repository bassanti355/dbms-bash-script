DBMS Bash Script
Overview
This is a simple Database Management System (DBMS) implemented using Bash scripting. It allows users to manage databases and tables with operations such as creating, listing, connecting to, and deleting databases. It also provides basic functionality for managing tables (e.g., create, drop, insert data, and more).

The system is designed for local use and operates via a terminal interface.

Features
Create Database: Allows the user to create a new database (as a directory).
List Databases: Lists all the available databases created in the system.
Connect to Database: Allows the user to connect to an existing database.
Drop Database: Deletes an existing database after confirming the action.
Table Operations (once connected to a database):
Create Table: Create a new table inside the selected database.
Drop Table: Remove an existing table.
Insert Into Table: Add data to a table.
Select From Table: View the contents of a table.
Delete From Table: Remove rows from a table.
Update Table: Modify existing table data.
List Tables: List all available tables in the connected database.
Requirements
A Linux or macOS environment with Bash.
Basic familiarity with terminal commands.
Bash scripting knowledge (optional, for customization).
Setup
Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/DBMS-Bash.git
cd DBMS-Bash
Run the Script:

Execute the script from the terminal:

bash
Copy code
./your_script_name.sh
Directory Setup:

The script will create a DBMS directory in your home directory (~/DBMS) where all databases will be stored.
Each database is represented by a directory, and inside each database, tables are stored as files.
Script Functions
The script contains various functions to handle common database operations:

1. Create Database:
Prompts for a valid database name (only letters, numbers, or underscores).
Checks if the database already exists and creates it if not.
2. List Databases:
Lists all the databases (directories) in the ~/DBMS folder.
3. Connect to Database:
Prompts the user to select a database to connect to (if it exists).
Once connected, the user can perform various table operations (create, drop, insert, select, delete, update, etc.).
4. Drop Database:
Allows the user to delete a database after confirming the action.
5. Table Operations:
Once connected to a database, users can choose from several options to manage tables:

Create Table: Adds a table to the connected database.
Drop Table: Deletes a table from the database.
Insert Into Table: Adds data to a table.
Select From Table: Displays the contents of a table.
Delete From Table: Deletes rows from a table.
Update Table: Modifies data in a table.
List Tables: Lists all tables in the connected database.
6. Exit:
Exits the script with a goodbye message.
Example Workflow
Start the program by running the script.
Choose an option from the main menu (e.g., Create Database).
Enter a valid database name.
Once the database is created, you can connect to it and perform operations on tables.
You can drop databases or tables as needed.
Example Session:
bash
Copy code
Welcome user

This is the main menu, Choose [1-5]: 
1) Create Database
2) List Database
3) Connect Database
4) Drop Database
5) Exit

Choose option: 1
Please Enter Database Name: testDB
Database 'testdb' is created successfully :)

This is the main menu, Choose [1-5]: 
1) Create Database
2) List Database
3) Connect Database
4) Drop Database
5) Exit

Choose option: 3
Enter the name of the database to connect: testdb
Connected To testdb Database

You are inside DB testdb, Choose [1-8]: 
1) Create Table
2) Drop Table
3) Insert Into Table
4) Select From Table
5) Delete From Table
6) Update Table
7) List Tables
8) Disconnect
Error Handling
The script performs basic input validation to ensure the following:

Database and table names contain only valid characters (letters, numbers, and underscores).
Operations like creating or dropping databases and tables are confirmed by the user before proceeding.
If the database or table doesn't exist, appropriate error messages are displayed.
Contributing
Contributions are welcome! If you have suggestions for new features or improvements, feel free to fork the project and create a pull request.

License
