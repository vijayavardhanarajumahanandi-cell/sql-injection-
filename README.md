What is it: A SQL Injection attack happens when an attacker is able to insert or inject malicious SQL statements into a query made by an application. The application treats this malicious input as part of the SQL command, rather than as harmless data. How it works The application takes user input (for example: a user ID, search term, login form etc.). Instead of a regular value, the attacker enters something like: 105 OR 1=1

which always evaluates to true. Because the user input is directly concatenated into the SQL statement (rather than using safe parameters), the attacker’s input changes the meaning of the query. As a result the attacker can:

Retrieve data they’re not supposed to see.

Modify or delete data.

In some cases even execute operations on the database server or underlying OS
