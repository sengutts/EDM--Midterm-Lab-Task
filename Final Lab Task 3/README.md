## Finals-Lab-Task-3
This portfolio is about learning MySQL by creating and managing a product database. It includes simple tasks like making a table, adding rules, inserting correct data, and changing a field. The goal is to understand how to build and organize a database using basic SQL.
Step by Step Process:
### 1. Create the Table
Make a table named products.
Add three fields:
- id (auto-increment and primary key)
- product_name (text up to 100 characters, cannot be empty)
- price (decimal number)

### 2. Add a Rule
Add a CHECK constraint to make sure the price is more than 0.
### 3. Insert Valid Products
+ Only add products with a positive price:

+ Laptop – 999.99 

+ Smartphone – 599.99 

+ Tablet – 299.99 

+ Keyboard – 19.99 

+ Mouse – 14.99 

+ Desk Lamp – 24.99 

+ Speakers – 9.99 

+ Skip items with negative prices.

Update the Table

- Change the ***product_name*** field to allow up to 120 characters.
## Screenshots
Query Statements
### Task 1
     
<img src="Images/Task1_1.png" alt="Alt Text" width="500" height="300"> 

### Task 2
  
<img src="Images/Task2_2.png" alt="Alt Text" width="500" height="300"> 

### Task 3  
<img src="Images/Task3_3.png" alt="Alt Text" width="500" height="300"> 

### Task 4
<img src="Images/Task4_4.png" alt="Alt Text" width="500" height="300"> 

### Table Structure
<img src="Images/Task1-1_TS.png" alt="Alt Text" width="500" height="300">
<img src="Images/Task3-4_TS.png" alt="Alt Text" width="500" height="300">

### ER Diagram

<img src="Images/Task_ERD.png" alt="Alt Text" width="500" height="300">

## SQL Copy of Database and Table Structures
To export, in MySQL Workbench:

Go to Server > Data Export > Export to Self-Contained File (.sql) and select only the structure option.

📍: [SQL FINALS LAB TASK 3](http://github.com/sengutts/EDM--Midterm-Lab-Task/blob/main/Final%20Lab%20Task%203/mySQL)
