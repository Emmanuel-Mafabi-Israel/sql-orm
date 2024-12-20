# Department Management System By      Israel Mafabi Emmanuel

This project is a Python-based Department Management System that interacts with an SQLite database to manage department records. The system supports creating, reading, updating, and deleting (CRUD) operations for department data.

## Project Structure

project-root/ ├── **init**.py ├── department.py ├── database/ │   └── company.db └── README.md

- `__init__.py`: Initializes the database connection and cursor.
- `department.py`: Contains the `Department` class with methods to interact with the database.
- `database/`: Directory to store the SQLite database file `company.db`.
- `README.md`: This README file.

## Prerequisites

- Python 3.x
- SQLite3
- MySQL Workbench (optional, for MySQL integration)

## Setup

1. Clone the repository:
   ```shell
   git clone https://github.com/Emmanuel-Mafabi-Israel/sql-mapping-an-sql-database.git
   cd project-root

2. Ensure you have `sqlite3` installed. You can verify it by running:

   ```shell
   sqlite3 --version
   ```

## Usage

### Creating the Database and Table

To create the `departments` table, run the following code:

```python
from department import Department

# Create the departments table
Department.create_table()
```

### Inserting a New Department

To insert a new department record:

```python
from department import Department

# Create a new department
new_department = Department.create('Human Resources', 'Building A')
```

### Updating a Department Record

To update an existing department record:

```python
from department import Department

# Assuming you have an existing department object
existing_department = Department('Human Resources', 'Building B', id=1)
existing_department.update_data()
```

### Deleting a Department Record

To delete an existing department record:

```python
from department import Department

# Assuming you have an existing department object
department_to_delete = Department('Human Resources', 'Building B', id=1)
department_to_delete.delete_data()
```

### Dropping the Table

To drop the `departments` table:

```python
from department import Department

# Drop the departments table
Department.drop_table()
```

### Testing...

To perform testing on the `project` run:

```shell
pytest # runs the tests available in the lib/testing folder...
```

## Features

- **Create Table**: Creates the `departments` table if it does not exist.

- **Drop Table**: Drops the `departments` table if it exists.

- **Insert Record**: Adds a new department record.

- **Update Record**: Updates an existing department record.

- **Delete Record**: Deletes an existing department record.

- **Unique Constraint**: Ensures department names are unique within the table.

  

### **Enjoy the Project!!!**

Feel free to reach out... 🤭😍😉

Made with Love... 😎

More so, Glory to God!!!