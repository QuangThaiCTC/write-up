# Challenge name: Quiz

**1. What is the difference between a prepared statement and a statement?**
Solution 1: Prepared statements are statements with hard-coded parameters.
Solution 2: Prepared statements are not stored in the database.
Solution 3: A statement is faster.
*Solution 4: A statement has got values instead of a prepared statement*

**2. Which one of the following characters is a placeholder for variables?**
Solution 1: *
Solution 2: =
*Solution 3: ?*
Solution 4: !

**3. How can prepared statements be faster than statements?**
Solution 1: They are not static so they can compile better written code than statements.
*Solution 2: Prepared statements are compiled once by the database management system waiting for input and are pre-compiled this way.*
Solution 3: Prepared statements are stored and wait for input it raises performance considerably.
Solution 4: Oracle optimized prepared statements. Because of the minimal use of the databases resources it is faster.

**4. How can a prepared statement prevent SQL-Injection?**
Solution 1: Prepared statements have got an inner check to distinguish between input and logical errors.
Solution 2: Prepared statements use the placeholders to make rules what input is allowed to use.
*Solution 3: Placeholders can prevent that the users input gets attached to the SQL query resulting in a seperation of code and data.*
Solution 4: Prepared statements always read inputs literally and never mixes it with its SQL commands.

**5. What happens if a person with malicious intent writes into a register form :Robert); DROP TABLE Students;-- that has a prepared statement?**
Solution 1: The table Students and all of its content will be deleted.
Solution 2: The input deletes all students with the name Robert.
Solution 3: The database registers 'Robert' and deletes the table afterwards.
*Solution 4: The database registers 'Robert' ); DROP TABLE Students;--'.*