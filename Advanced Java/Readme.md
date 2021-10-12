# 9/8
### JDBC 
Java Database Connectivity (JDBC) is an application programming interface (API) for the programming language Java, which defines how a client may access a database. It is a Java-based data access technology used for Java database connectivity. It is part of the Java Standard Edition platform, from Oracle Corporation. It provides methods to query and update data in a database, and is oriented toward relational databases. A JDBC-to-ODBC bridge enables connections to any ODBC-accessible data source in the Java virtual machine (JVM) host environment.
### Role of JDBC Driver 
JDBC tries to minimize the number of details that a developer needs to worry about. A common approach to this goal is to specify the layers at which various common activities occur and then to tightly define how those layers will interact with one another and with a program.
JDBC takes this approach. JDBC specifies that most of the details about communicating with a database system will be handled through a software layer called a driver. This driver will handle the details of the three basic tasks we need to do to work with a database:
1. Create and maintain a connection to a database
2. Send our commands to that database
3. Deliver the database response back to our program

### JDBC Driver-jar file
 in order for Java applications working with a database engine via Java Database Connectivity (JDBC), an appropriate JDBC driver library is required to be available in the application’s classpath. A JDBC driver library consists of Java classes which implement low-level communication with the database engine. It talks with Java applications via JDBC API and usually bundled as a JAR or ZIP file.
 
For your reference and convenience, i provides a summary of JDBC driver download for common databases including MySQL, SQL Server, Oracle, PostgreSQL, Apache Derby (Java DB), SQLite and Microsoft Access. If you use Maven, see the Maven dependencies for those JDBC drivers below.

|  Database | JDBC Driver Provider  |  JAR file name |
| ------------ | ------------ | ------------ |
|  MySQL |  Oracle Corporation |  mysql-connector-java-VERSION.jar |
|  SQL Server | Microsoft Corporation  | sqljdbc41.jar, sqljdbc42.jar  |
|  Oracle | Oracle Corporation  | ojdbc6.jar, ojdbc7.jar, ojdbc8.jar  |
| PostgreSQL  |  The PostgreSQL Global Development Group | postgresql-VERSION.jar  |
|  Apache Derby |Apache Software Foundation   | derby.jar, derbyclient.jar  |
| SQLite  |Xerial.org   |  sqlite-jdbc-VERSION.jar |


### Generation of JDBC Drivers
![JDBC](https://github.com/nayan1xyz/C-DAC-Notes/blob/main/Advanced%20Java/Media/Assignments/1_JDBC.jpg)

### Steps for connecting JDBC
- loading driver
- establishing connection
- creating statement or prepered statement
### Statement 
### Prepered Statement
### Stored Procedure 
### Callable Statement 

# 10/8
### Callable Statement
- Stored procedure is stored in db as db object
- It is used for frequently needed task
- Block of PL/SQL 
- Callable Statement used to call stored procedure 
- Supply required parameter and excute
- There are three parameter of strored procedure 
	- in
	- out 
	- inOut
- It seperate out java and sql
```sql
CREATE PROCEDURE `getSalary` (in empno int, out sal float)
BEGIN
	select salary into sal from emp where empid=empno;
END $$
delimiter;



```


```java




```

### Scrollable and updatable result set

## Servlet 
- It is a java class 
- Used for generating dynamic html 
- Host the servlet in the in the enviroment of web service 
- Web server is accept the request and send the request
- Servelet is present in web server
- Generating dynamic html cannont be done by web server					
