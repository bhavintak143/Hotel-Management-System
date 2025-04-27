# Hotel Management System

A comprehensive hotel management system built with Java, JSP, Servlets, and MySQL.

## Prerequisites

1. Java JDK 1.8 or higher
2. Eclipse IDE for Enterprise Java Developers
3. Apache Tomcat 9.0
4. MySQL Server 8.0
5. Maven 3.6 or higher

## Setup Instructions

### 1. Database Setup

1. Open MySQL Command Line or MySQL Workbench
2. Run the SQL script located at `src/main/resources/database.sql`
3. This will create the database and all necessary tables

### 2. Eclipse Project Setup

1. Open Eclipse
2. Import the project:
   - File -> Import -> Maven -> Existing Maven Projects
   - Select the project root directory
   - Click Finish

3. Configure Tomcat Server:
   - Right-click on the project
   - Properties -> Targeted Runtimes
   - Select Apache Tomcat v9.0
   - Click Apply and Close

4. Configure Build Path:
   - Right-click on the project
   - Properties -> Java Build Path
   - Ensure all Maven dependencies are properly resolved
   - Click Apply and Close

### 3. Configure Database Connection

1. Open `src/main/java/com/hotel/util/DatabaseUtil.java`
2. Verify the database connection parameters:
   ```java
   private static final String URL = "jdbc:mysql://localhost:3306/hotel_management";
   private static final String USERNAME = "root";
   private static final String PASSWORD = "bhavin";
   ```
3. Update the values if your MySQL configuration is different

### 4. Run the Application

1. Right-click on the project
2. Run As -> Run on Server
3. Select Tomcat v9.0 Server
4. Click Finish

### 5. Access the Application

1. Open your web browser
2. Navigate to: `http://localhost:8080/HotelManagementSystem/`
3. Default login credentials:
   - Username: admin
   - Password: admin123

## Project Structure

- `src/main/java/com/hotel/servlet/` - Contains all servlets
- `src/main/java/com/hotel/util/` - Contains utility classes
- `src/main/webapp/` - Contains JSP files and static resources
- `src/main/resources/` - Contains configuration files and SQL scripts

## Features

- User Authentication
- Employee Management
- Room Management
- Customer Management
- Booking System
- Department Management
- Menu Management
- Reception Management

## Troubleshooting

1. If you get "ClassNotFoundException" for MySQL driver:
   - Right-click on the project
   - Properties -> Java Build Path
   - Check if mysql-connector-java is in the classpath

2. If you get "HTTP 404" error:
   - Verify Tomcat server is running
   - Check if the application is deployed correctly
   - Verify the context path in server configuration

3. If you get database connection errors:
   - Verify MySQL server is running
   - Check database credentials in DatabaseUtil.java
   - Ensure the database and tables are created

## Support

For any issues or questions, please contact the development team. 