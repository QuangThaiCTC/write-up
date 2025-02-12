# Challenge name: Try it! Writing safe code

### Challenge Description:
You can see some code down below, but the code is incomplete. Complete the code, so that it’s no longer vulnerable to a SQL injection! Use the classes and methods you have learned before.

The code has to retrieve the status of the user based on the name and the mail address of the user. Both the name and the mail are in the string format.

### My Solution
Connection conn = DriverManager.`getConnection`(DBURL, DBUSER, DBPW);
`PreparedStatement pstmt` = conn.`prepareStatement`("SELECT status FROM users WHERE name=`?` AND mail=`?`");
`pstmt.setString(1,"wonnocri")`;
`pstmt.setString(2,"attacker@here.com")`;
