🛒 E-Commerce Web Application using Spring Boot

A full-stack e-commerce web application built using Spring Boot, Hibernate, JSP, and MySQL, featuring user authentication, product management, cart functionality, and admin controls.

📌 Project Overview

This project was developed as part of the Semester 4 academic curriculum (Jan–May 2024).
It simulates a real-world e-commerce platform with clearly separated user and admin workflows, following a layered backend architecture based on MVC and DAO–Service patterns.

🆕 What’s New (Current Version)

Hibernate configuration added (database & tables auto-created on startup)
Service layer introduced for reusable business logic
DAO layer for clean database interaction
Bug fixes (product images, security, minor issues)
Codebase redesigned for better modularity and reusability
Compatible with both IntelliJ IDEA and Eclipse

⚠️ Disclaimer: This branch is under active development; some endpoints and cart logic may still be unstable

✨ Key Features
👤 User Module

User registration and secure login
Browse products by category
Add and remove products from cart
View cart summary

🛠 Admin Module

Admin authentication
Add, update, and delete products
Manage product categories
View customers and dashboard data

🧱 System Architecture

MVC pattern using Spring MVC
Controller → Service → DAO → Database flow
Hibernate ORM for persistence
JSP for server-side UI rendering

🧑‍💻 My Role & Contributions

Designed and implemented backend modules using Spring Boot
Developed Controllers, Services, and DAO layers
Integrated Hibernate-based database persistence
Contributed to JSP-based UI and product–cart workflows
Collaborated in a two-member team using modular development

🛠 Tools & Technologies

Language: Java
Frameworks: Spring Boot, Spring MVC
ORM: Hibernate
Database: MySQL / MariaDB
Frontend: JSP, HTML, CSS
Build Tool: Maven

📂 Project Structure
JtProject/
├── src/main/java/
│   └── com.jtspringproject.JtSpringProject
│       ├── controller
│       ├── service
│       ├── dao
│       ├── configuration
│       └── model
├── src/main/webapp/
│   └── WEB-INF/jsp
├── pom.xml
└── basedata.sql

⚙️ Quick Start
1️⃣ Clone the Repository
git clone https://github.com/priyansh-2105/springboot-ecommerce-webapp.git

2️⃣ Open in IDE

IntelliJ IDEA (recommended) or Eclipse
Ensure the project is opened as a Maven project

3️⃣ Configure Database

Edit src/main/resources/application.properties:

db.url=jdbc:mysql://[db_host]:[db_port]/ecommjava?createDatabaseIfNotExist=true
db.username=your_username
db.password=your_password

⚠️ Avoid using the root user. Ensure the database user has appropriate permissions.

4️⃣ Run the Project

Run the main method in JtSpringProjectApplication.java
OR
mvn spring-boot:run

5️⃣ Access the Application
http://localhost:8080/

🔐 Sample Credentials (Optional)

If you execute basedata.sql, you may use the following demo credentials:

Admin
Username: admin
Password: 123

User
Username: lisa
Password: 765

⚠️ These are sample credentials for academic demonstration only.

🗄 Database Notes
MySQL or MariaDB supported
If you face the error:
java.lang.IllegalArgumentException: Could not resolve placeholder 'db.driver'
Update the mysql-connector-java version in pom.xml according to your MySQL version and reload Maven.

🖥 Web Directory Configuration (Important for JSP)

Views are located in:
src/main/webapp/views

Spring Boot may not detect this by default.

IntelliJ IDEA Fix:

Open Edit Configurations
Select JtSpringProjectApplication
Set Working directory to:
$MODULE_WORKING_DIR$

Apply and rerun

🌐 Available Endpoints

/
/register
/admin/products
/admin/customers
/admin/categories
/admin/dashboard

🚀 Future Enhancements

REST-based backend with React or Angular frontend
Role-based authorization
Payment gateway integration
Improved UI and UX
Optimized cart logic

📄 Academic Details

Course: Semester 4 Mini Project
Duration: Feb 2024 – May 2024
Team Size: 2