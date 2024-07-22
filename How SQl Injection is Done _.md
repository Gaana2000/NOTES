# How Sql Injection Works?

**For Working of SQL injection we need a Web Application that uses a Database.**

**SQL in Web Pages**

SQL injection typically occurs when you ask a user for input, such as their username/user ID, and instead of their name/ID, the user inputs an SQL statement that will be executed without the knowledge about your database.

**For example**,

**txtUserId = getRequestString("UserId");
txtSQL = "SELECT * FROM Users
WHERE UserId = " + txtUserId;**

The above code is constructing an SQL query by directly concatenating a user input (txtUserId) into the query string. Attackers can easily exploit this by giving an input that is always true, like **x=x,1=1**, etc.

If the attacker gave input as **” 105 OR 1=1 ”** in the UserId field, the resulting SQL will be:

**SELECT * FROM Users WHERE UserId = 105 OR 1=1;**

This resulting query will return data of all users, not just the user with UserId =”105″.


**SQL Injection Example**

For a better understanding of how attackers do a SQL injection attack, let’s learn how to do an SQL injection attack ourselves. In this example, we will perform a basic SQL injection attack and learn the process behind it.

Suppose we have an application based on student records. Any student can view only his or her records by entering a unique and private student ID. 

Suppose we have a field like the one below: 

**Student id: The student enters the following in the input field: 12222345 or 1=1.** 

**Query**

**SELECT * FROM STUDENT WHERE
STUDENT-ID == 12222345 or 1 = 1**

SQL Injection based on 1=1 is always true. As you can see in the above example, 1=1 will return all records for which this holds true. So basically, all the student data is compromised. Now the malicious user can also similarly use other SQL queries. 

Consider the following SQL query.

**Query 1**

** SELECT * FROM USER WHERE
USERNAME = “” AND PASSWORD=”” ** 

Now the malicious attacker can use the **‘=’** operator cleverly to retrieve private and secure user information. So following query when executed retrieves protected data, not intended to be shown to users.

**Query 2**

** SELECT* FROM User WHERE
(Username = “” OR 1=1) AND 
(Password=”” OR 1=1) **

Since 1=1 always holds true, user data is compromised.