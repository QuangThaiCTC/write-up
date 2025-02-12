# Challenge name: Try it! Writing safe code

### Challenge Description:
Now it is time to write your own code! Your task is to use JDBC to connect to a database and request data from it.

Requirements:

- connect to a database

- perform a query on the database which is immune to SQL injection attacks

- your query needs to contain at least one string parameter

Some tips before you start:
For connecting to the database, you can simply assume the constants DBURL, DBUSER and DBPW as given.
The content of your query does not matter, as long as the SQL is valid and meets the requirements.
All the code you write gets inserted into the main method of a Java class with the name "TestClass" that already imports java.sql.* for you.

Not creative enough to think of your own query? How about you try to retrieve the data of a user with a specific name from a fictional database table called users.

For example; the following code would compile without any error (but of course does not meet the requirements to complete this lesson).

```Java
try {
    Connection conn = null;
    System.out.println(conn);   //should output 'null'
} catch (Exception e) {
    System.out.println("Oops. Something went wrong!");
}
```


### My Solution
```Java
try {
    String query = "SELECT name FROM users where name = ?";
    Connection conn = DriverManager.getConnection(DBURL,DBUSER,DBPW);
    PreparedStatement pstmt = conn.prepareStatement(query);
    pstmt.setString(1,"wonnocri");
    pstmt.executeQuery();
} catch (Exception e) {
    System.out.println("Oops. Something went wrong!");
}
```