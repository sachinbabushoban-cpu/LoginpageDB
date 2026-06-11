# Login Page - Java Servlet + JSP + JDBC

A simple login application built using Java Servlets, JSP, and MySQL database connectivity.

## Technologies Used
- Java (Servlets, JSP)
- Apache Tomcat 10.1
- MySQL (JDBC)
- Eclipse IDE

## Project Structure
- `login.jsp` - Login form (UI)
- `LoginServlet.java` - Handles login logic, validates credentials against MySQL database
- `web.xml` - Configuration file (welcome page setup)

## Database Setup
Run this SQL script in MySQL Workbench before running the project:

```sql
CREATE DATABASE logindb;

USE logindb;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(50) NOT NULL
);

INSERT INTO users (username, password) VALUES ('Sachin', '1234');
```

## How to Run
1. Import project into Eclipse (Dynamic Web Project)
2. Add MySQL Connector JAR to `WEB-INF/lib`
3. Update `LoginServlet.java` with your MySQL username & password
4. Run on Apache Tomcat server
5. Open browser: `http://localhost:8080/LoginAppDB/`

## Features
- User login validation against MySQL database
- Session-based error handling for invalid credentials
- Simple, clean UI

## Author
Sachin Babu S
