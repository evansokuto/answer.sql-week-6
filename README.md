# answer.sql-week-6

-- Question 1
SELECT e.firstName, e.lastName, e.email, oc.officeCode
FROM employees AS e
INNER JOIN offices AS oc ON e.officeCode = oc.officeCode;
-- Question 2
SELECT p.productName, p.productVendor, p.productLine
FROM products p
LEFT JOIN productlines AS pl ON p.productLine = pl.productLine;
-- Question 3
SELECT o.orderDate, o.shippedDate, o.status, o.customerNumber
FROM orders AS o
RIGHT JOIN customers AS c ON o.customerNumber = o.customerNumber
LIMIT 10;
