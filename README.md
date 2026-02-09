🔐 RevPasswordManager

RevPasswordManager is a **secure, console-based password management application** developed using **Java, JDBC, and MySQL**.  
The application allows users to safely store, manage, and retrieve multiple account passwords using a single master account, following standard security and architectural practices.

---

📌 Project Overview

The project focuses on building a **secure password manager** that supports real-world features such as encrypted password storage, master password verification, security question–based recovery, and modular layered design.

It demonstrates strong backend fundamentals including **authentication, validation, encryption, exception handling, and database integration**.

---
🚀 Features

🔑 User Authentication & Security
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

🔐 Password Management
- Add new password entries for various accounts
- List all saved password entries
- View account passwords (requires master password re-entry)
- Update existing passwords
- Delete password entries
- Search passwords by account name

---

🛡️ Security Implementation
- Master passwords are **hashed** before storing in the database
- Account passwords are **encrypted**
- Sensitive operations require **master password re-entry**
- Verification codes are time-bound and expire after use
- Security questions are linked to user accounts for recovery

---

📂 Functional Scope

- Registered users can:
  - Log in to the system
  - Add, update, delete, and search passwords
  - Change master password
  - Recover forgotten passwords using security questions
- Only authenticated users can access password-related operations
- Email uniqueness is enforced during registration and updates

---

🏗️ Application Architecture

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

🗄️ Database Design

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

🛠️ Technologies Used

- Java (Core Java)
- JDBC
- MySQL
- Encryption & Hashing (for passwords)
- Object-Oriented Programming (OOP)
- Exception Handling & Validations

---

✅ Definition of Done (DoD)

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

📊 ER Diagram

The **Entity Relationship (ER) Diagram** represents the logical structure of the RevPasswordManager database and defines how entities are related to each other.

🔗 Key Entities
- **Users**
  - Stores user account information such as name, email, and master password hash.
- **Passwords**
  - Stores encrypted passwords for different accounts linked to a user.
- **Security_Questions**
  - Stores security questions and hashed answers for account recovery.
- **Verification_Codes**
  - Stores one-time verification codes used for sensitive operations like password reset.

🔐 Relationships
- One **User** can have **multiple Password entries**.
- Each **Password** belongs to exactly **one User**.
- Each **User** has **one Security Question** for recovery.
- Each **User** can generate **multiple Verification Codes**, each expiring after use.

🧩 Design Highlights
- Primary and Foreign Keys are used to maintain referential integrity.
- The schema follows normalization principles to avoid redundancy.
- The design supports secure authentication and recovery workflows.

---

▶️ How to Run the Application

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/RevPasswordManager.git
