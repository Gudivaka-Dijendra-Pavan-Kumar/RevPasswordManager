**🔐 RevPasswordManager**

RevPasswordManager is a **secure, console-based password management application** developed using **Java, JDBC, and MySQL**.  
The application allows users to safely store, manage, and retrieve multiple account passwords using a single master account, following standard security and architectural practices.

---

**📌 Project Overview**

The project focuses on building a **secure password manager** that supports real-world features such as encrypted password storage, master password verification, security question–based recovery, and modular layered design.

It demonstrates strong backend fundamentals including **authentication, validation, encryption, exception handling, and database integration**.

---
**🚀 Features**

**🔑 User Authentication & Security**
- User registration with:
  - Email validation
  - Duplicate email prevention
  - Strong password enforcement
  - Security question and answer setup
- Login using email and master password
- Logout functionality
- Forgot password recovery using:
  - Security question verification
  - One-time verification code (expires after use)

---

**🔐 Password Management**
- Add new password entries for various accounts
- List all saved password entries
- View account passwords (requires master password re-entry)
- Update existing passwords
- Delete password entries
- Search passwords by account name

---

**🛡️ Security Implementation**
- Master passwords are **hashed** before storing in the database
- Account passwords are **encrypted**
- Sensitive operations require **master password re-entry**
- Verification codes are time-bound and expire after use
- Security questions are linked to user accounts for recovery

---

**📂 Functional Scope**

- Registered users can:
  - Log in to the system
  - Add, update, delete, and search passwords
  - Change master password
  - Recover forgotten passwords using security questions
- Only authenticated users can access password-related operations
- Email uniqueness is enforced during registration and updates

---

**🏗️ Application Architecture**

The project follows a **modular, layered architecture**:

- **UI Layer**  
  Console-based user interaction (MainMenu)

- **Service Layer**  
  Business logic, validations, and exception handling

- **DAO Layer**  
  Database operations using JDBC

- **Utility Layer**  
  Encryption, hashing, and database connectivity

- **Database Layer**  
  MySQL relational database

---

**🗄️ Database Design**

- Relational database using MySQL
- Tables include:
  - Users
  - Passwords
  - Security Questions
  - Verification Codes
- Supports:
  - Primary keys
  - Foreign key relationships
  - Normalized schema design

---

**🛠️ Technologies Used**

- Java (Core Java)
- JDBC
- MySQL
- Encryption & Hashing (for passwords)
- Object-Oriented Programming (OOP)
- Exception Handling & Validations

---

**✅ Definition of Done (DoD)**

- Fully working console-based application
- Secure authentication and password management
- Password recovery via security questions
- Verification code mechanism implemented
- Clean layered architecture
- Database integration using JDBC
- ER Diagram created
- Application Architecture Diagram created
- Code shared via GitHub for technical evaluation

---

**📊 ER Diagram**

This diagram represents the database design of the RevPasswordManager application, 
showing users, password entries, security questions, and verification codes along 
with their relationships.

![ER Diagram](ER%20diagram.jpeg)

---

**▶️ How to Run the Application**

1. Clone the repository:
```bash
git clone https://github.com/your-username/RevPasswordManager.git
Open the project in an IDE

Use Eclipse, IntelliJ IDEA, or any Java-supported IDE

Import the project as a Java Project

Set up the database

Create a MySQL database (for example: rev_password_manager)

Run the provided SQL table creation scripts to create:

users

password_entries

security_questions

verification_codes

Configure database connection

Open DBConnection.java

Update the following values with your local MySQL details:

Database URL

Username

Password

Add MySQL JDBC Driver

Ensure MySQL Connector/J is added to your project classpath

If using Maven/Gradle, add the dependency

Otherwise, add the JAR manually to the build path

Build the project

Resolve any dependency issues

Ensure there are no compilation errors

Run the application

Locate the MainMenu class

Right-click → Run as Java Application
