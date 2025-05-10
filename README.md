# Student Result Management System

This is a Spring Boot-based web application to manage student results, marks entry, result viewing, and admin login.

## Features
- Admin login & dashboard
- Admin can change password
- Add/view students
- Enter/view marks
- Manage notices
- Students can view marks and notices

## Technologies Used
- Java 21
- Spring Boot
- Thymeleaf
- MySQL
- HTML, CSS
How to Run the Application
Clone or download the project to your local machine.

Open the project in your favorite IDE (e.g., Spring Tool Suite, IntelliJ IDEA).

Ensure your MySQL database is set up with the correct username and password.

Modify the application.properties with your MySQL credentials and Gmail account info.

Run the project using Spring Boot by running the StudentResultManagementSystemApplication.java class.
## Spring Boot Application Properties

Make sure to configure the following properties in `src/main/resources/application.properties`:

```properties
# Server Port
server.port=8081

# Database Configuration
spring.datasource.url=jdbc:mysql://localhost:3306/srms
spring.datasource.username=root
spring.datasource.password=your-password

# JPA Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect

# Mail Service (For Email Notifications)
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=your-gmail
spring.mail.password=your-password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true

