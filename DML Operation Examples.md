# Examples of DML Operations

# 1. INSERT 

Q: Display the query to insert a new employee record into the employees table with first_name, last_name, and hire_date.

INSERT INTO employees (first_name, last_name, hire_date)
VALUES ('John', 'Doe', '2024-01-15');

# 2. SELECT

Q: Display the query to select all records from the employees table.

SELECT * FROM employees;

# 3. SELECT with WHERE Clause

Q: Display the query to select all employees whose department is ‘HR’ from the employees table.

SELECT * FROM employees
WHERE department = 'HR';

# 4. UPDATE

Q: Display the query to update the hire_date of an employee with employee_id 5 to ‘2024-03-01’ in the employees table.

UPDATE employees
SET hire_date = '2024-03-01'
WHERE employee_id = 5;

# 5. DELETE

Q: Display the query to delete an employee with employee_id 10 from the employees table.

DELETE FROM employees
WHERE employee_id = 10;

# 6. SELECT with ORDER BY

Q: Display the query to select all employees from the employees table and order them by hire_date in descending order.

SELECT * FROM employees
ORDER BY hire_date DESC;

# 7. SELECT with LIMIT

Q: Display the query to select the first 5 records from the employees table.

SELECT * FROM employees
LIMIT 5;

# 8. SELECT with DISTINCT

Q: Display the query to select unique values from the department column in the employees table.

SELECT DISTINCT department FROM employees;

# 9. UPDATE with CASE

Q: Display the query to update the department column to ‘Sales’ for employees with employee_id greater than 50, and ‘Marketing’ for employees with employee_id less than or equal to 50.

UPDATE employees
SET department = CASE 
                    WHEN employee_id > 50 THEN 'Sales'
                    ELSE 'Marketing'
                  END;

# 10. DELETE with LIMIT

Q: Display the query to delete the first 3 employees from the employees table based on their employee_id.

DELETE FROM employees
WHERE employee_id IN (SELECT employee_id FROM employees LIMIT 3);
