# Examples of DDL Operations

# 1. CREATE TABLE

Q: Display the query to create an employees table with the following fields: employee_id (primary key), first_name, last_name, hire_date.

CREATE TABLE employees (

  employee_id SERIAL PRIMARY KEY,

  first_name VARCHAR(50) NOT NULL,

  last_name VARCHAR(50) NOT NULL,

  hire_date DATE

);

# 2. ALTER TABLE (Add Column)

Q: Display the query to add a column department (type VARCHAR(50)) to the employees table.

ALTER TABLE employees ADD COLUMN department VARCHAR(50);

# 3. ALTER TABLE (Rename Column)

Q: Display the query to rename the department column to department_name in the employees table.

ALTER TABLE employees RENAME COLUMN department TO department_name;

# 4. DROP TABLE

Q: Display the query to delete the employees table and all its data.

DROP TABLE employees;

# 5. CREATE INDEX

Q: Display the query to create an index idx_last_name on the last_name column of the employees table.

CREATE INDEX idx_last_name ON employees (last_name);

# 6. TRUNCATE TABLE

Q: Display the query to remove all rows from the employees table, keeping its structure intact.

TRUNCATE TABLE employees;

# 7. RENAME TABLE

Q: Display the query to rename the employees table to staff.

ALTER TABLE employees RENAME TO staff;

# 8. ALTER TABLE (Modify Column Data Type)

Q: Display the query to change the data type of the hire_date column in the employees table to TIMESTAMP.

ALTER TABLE employees ALTER COLUMN hire_date TYPE TIMESTAMP;
