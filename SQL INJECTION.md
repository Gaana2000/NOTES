# SQL INJECTION

**SQL injection** is a code injection technique attackers use to gain unauthorized access to a database by injecting malicious SQL commands into web page inputs.
Attackers can extract sensitive information, modify database data, execute administration operations on the database (such as shutdown DBMS), recover the content of a given file present on the DBMS file system, and in some cases, issue commands to the operating system.

● **SQLi** or **SQL Injection** is a web page vulnerability that lets an attacker make queries with the database. Attackers take advantage of web application vulnerability and inject an SQL command via the input from users to the application.
Attackers can SQL queries like **SELECT** to retrieve confidential information which otherwise wouldn’t be visible. SQL injection also lets the attacker to perform a denial-of-service (DoS) attacks by overloading the server requests.


**SQL in Web Pages**

● SQL injection typically occurs when you ask a user for input, such as their username/user ID, and instead of their name/ID, the user inputs an SQL statement that will be executed without the knowledge about your database.

● For example,

**txtUserId = getRequestString("UserId");
txtSQL = "SELECT * FROM Users
WHERE UserId = " + txtUserId;**

The above code is constructing an SQL query by directly concatenating a user input (txtUserId) into the query string. Attackers can easily exploit this by giving an input that is always true, like x=x,1=1, etc.

If the attacker gave input as ” 105 OR 1=1 ” in the UserId field, the resulting SQL will be:

**SELECT * FROM Users WHERE UserId = 105 OR 1=1;**
This resulting query will return data of all users, not just the user with UserId =”105″.


# SQL Injection Types

1. **In-band SQL Injection**

2. **Error-based SQL Injection**

3. **Blind SQL Injection**

4. **Out-of-band SQL Injection**

5. **Inference-based SQL Injection**


# Impact of SQL Injection

The hacker can retrieve all the user data present in the database such as user details, credit card information, and social security numbers, and can also gain access to protected areas like the administrator portal. It is also possible to delete user data from the tables. 
Nowadays, all online shopping applications and bank transactions use back-end database servers. So in case the hacker is able to exploit SQL injection, the entire server is compromised. 


# SQL Injection Prevention

1. **User Authentication**: Validating input from the user by pre-defining length, type of input, of the input field and authenticating the user.


2. Restricting access privileges of users and defining how much amount of data any outsider can access from the database. Basically, users should not be granted permission to access everything in the database.


3. Do not use system administrator accounts. 

..............................................................................................