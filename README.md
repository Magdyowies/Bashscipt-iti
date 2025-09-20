# Bash DBMS

A simple **Database Management System (DBMS)** implemented in **Bash Script**.  
This project simulates the basic functionality of a DBMS using **directories** for databases and **files** for tables.

---

## 📌 Features

### Database Level
- **Create Database** → Create a new database (directory).
- **List Databases** → Show all existing databases.
- **Connect To Database** → Connect to a specific database to manage its tables.
- **Drop Database** → Delete a database permanently.

### Table Level
- **Create Table**  
  - Define columns, data types, and a primary key.  
  - Metadata is stored in the first three lines of the table file:
    1. Columns (comma separated)  
    2. Datatypes (comma separated)  
    3. Primary key  

- **List Tables** → Show all tables in the connected database.  
- **Drop Table** → Delete a specific table (file).  

### Record Level
- **Insert Into Table**  
  - Add new records while checking:
    - Data type validity (`int` or `str`).
    - Primary key uniqueness.  

- **Select From Table** → Display table records in a readable format.  
- **Delete From Table** → Remove a record using its primary key.  
- **Update Table** → Update an existing record by primary key (with validation).  

### Utility
- **Disconnect** → Exit the current database and return to the main menu.  
- **Exit** → Quit the program.  

---

## 📂 Project Structure

- Each **database** is represented by a directory.  
- Each **table** is a text file inside its database directory.  
- File content format:
