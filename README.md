# Week-2-Assignment
# week-2-answers-for-sql
Introduction to SQL and Basic Queries — Assignment
/*  
📊 Introduction to SQL and Basic Queries — Assignment

📌 Overview
This assignment focuses on learning and practicing SQL basics such as retrieving data, filtering, sorting, and limiting results.

🎯 Learning Objectives
- Understand SQL query structure
- Retrieve specific columns from tables
- Apply WHERE for filtering
- Use ORDER BY for sorting
- Use LIMIT for restricting results

🛠 Requirements
- MySQL, PostgreSQL, or MariaDB installed
- SQL editor (MySQL Workbench, DBeaver, pgAdmin, CLI)
- Basic SQL syntax knowledge
*/

/*  
1️⃣ Retrieve the checkNumber, paymentDate, and amount from the payments table  
*/
SELECT checkNumber, paymentDate, amount
FROM payments;

/*  
2️⃣ Retrieve the orderDate, requiredDate, and status from orders where status is 'In Process',
   sorted by orderDate in descending order  
*/
SELECT orderDate, requiredDate, status
FROM orders
WHERE status = 'In Process'
ORDER BY orderDate DESC;

/*  
3️⃣ Display the firstName, lastName, and email of employees with job title 'Sales Rep',
   ordered by employeeNumber descending  
*/
SELECT firstName, lastName, email
FROM employees
WHERE jobTitle = 'Sales Rep'
ORDER BY employeeNumber DESC;

/*  
4️⃣ Retrieve all columns and records from the offices table  
*/
SELECT *
FROM offices;

/*  
5️⃣ Fetch productName and quantityInStock from products,
   sorted by buyPrice in ascending order, limited to 5 records  
*/
SELECT productName, quantityInStock
FROM products
ORDER BY buyPrice ASC
LIMIT 5;

/*  
📜 License
For educational purposes only — feel free to modify for learning.
*/
