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


## ▶️ How to Run

1. Clone the repository or copy the script.
 ```bash
 git clone https://github.com/your-username/bash-dbms.git
 cd bash-dbms

2.Make the script executable:
---
chmod +x dbms.sh
3. execute script 
 ./project.sh
-------------------------------------------------------
🛠 Example Usage
=========================================
       Bash DBMS - Main Menu
=========================================
1. Create Database
2. List Databases
3. Connect To Database
4. Drop Database
5. Exit
=========================================
Enter your choice:


Create a database → Connect → Create a table → Insert data → Select data.


----------------------------------


 --------Future Improvements------------------

Support for more datatypes (float, date, etc.).

Add filtering in SELECT (WHERE clause).

Add exporting/importing tables (CSV).

Implement indexing for faster search.


---------------------------------
Author
-Ahmed Ezzat
- MagdyOwies 
