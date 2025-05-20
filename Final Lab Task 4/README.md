## Finals Lab Task 4
### Task Description:
This task involved working with a single database containing two tables: EmployeeSalaries and EmployeeData. I performed a series of SELECT statements to extract and manipulate employee information.
### Step 1: Query Statements
Objective: Perform queries on the EmployeeSalaries table.

### - Problem 1: Consider a table named EmployeeSalaries that stores information about the salaries of employees.
### - The table has the following fields:
```CREATE DATABASE payroll;
USE payroll;

CREATE TABLE EmployeeSalaries (
    employee_id INT AUTO_INCREMENT PRIMARY KEY,
    employee_name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE
);
```
![image](https://github.com/user-attachments/assets/e6c078f5-1037-4ab5-8a49-4f8f7c2564b0)


### Retrieve the employee_name and salary and arrange from the highest salary to lowest.

```SELECT employee_name, salary FROM EmployeeSalaries ORDER BY salary DESC;```

![image](https://github.com/user-attachments/assets/36add1a1-9461-46ef-8856-c89d5418a9c5)


### Retrieve the department names along with the average salary for each department.

```SELECT department, AVG(salary) AS average_salary FROM EmployeeSalaries GROUP BY department;```

![image](https://github.com/user-attachments/assets/6ab48375-7ff0-4a0e-8293-9e04ff74c181)


### Step 2: Key Schema Statements
#### Objective: Perform queries on the EmployeeData table.

### - Problem 2: Create a database named employeeDB and copy and paste the initial query.
### - The EmployeeData table stores information about employees with the following schema:
CREATE DATABASE employeeDB;
USE employeeDB;

```CREATE TABLE EmployeeData (
    employee_id INT AUTO_INCREMENT PRIMARY KEY,
    full_name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE,
    manager_id INT
);
```
![image](https://github.com/user-attachments/assets/72378db4-fd78-4e17-8a53-3e525517292d)



### Retrieve the employees along with their full names and salaries with highest paying employee to the lowest.

```SELECT full_name, salary FROM EmployeeData ORDER BY salary DESC;```

![image](https://github.com/user-attachments/assets/c824a02e-59e7-4c43-a07f-73fb68408f45)


### Retrieve the average salary from EmployeeData table, where the average salary exceeds $70,000.

```SELECT AVG(salary) AS average_salary FROM EmployeeData HAVING average_salary > 70000;```
![image](https://github.com/user-attachments/assets/926e2cc7-9da8-4f12-83f5-521fbb06db0a)


### Retrieve the full names of employees who earn a salary greater than $100,000.

```SELECT full_name FROM EmployeeData WHERE salary > 100000;```

![image](https://github.com/user-attachments/assets/5e839a54-9008-4245-a88f-cbaa2ccace74)


### Retrieve the number of employees from the EmployeeData table.

```SELECT COUNT(employee_id) AS number_of_employees FROM EmployeeData;```

![image](https://github.com/user-attachments/assets/9f49d438-3604-4667-a5a0-f69fa98be6bd)

![image](https://github.com/user-attachments/assets/f7964ecf-5a42-4a54-89a8-549e69a03ec1)
