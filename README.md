 RevPasswordManager
RevPasswordManager is a secure, console-based password management system developed using Java, JDBC, and MySQL.
The application enables users to store, manage, and retrieve multiple account passwords securely using a single master account, following real-world security and architectural practices.
________________________________________
 Project Objective
The goal of this project is to build a secure password manager that:
•	Protects sensitive data using encryption and hashing
•	Supports password recovery using security questions
•	Demonstrates clean layered architecture
•	Applies proper validations, exceptions, and database design
________________________________________
 Features
 Authentication & User Management
•	User registration with:
o	Email format validation
o	Duplicate email check
o	Strong password validation
o	Security question & answer
•	Login using email and master password
•	Logout functionality
•	Forgot password recovery using:
o	Security question verification
o	One-time verification code (expires after use)
________________________________________
 Password Management
•	Add new password entries for various accounts
•	List all saved account names
•	View passwords (requires master password re-entry)
•	Update existing account passwords
•	Delete password entries
•	Search passwords by account name
________________________________________
 Security
•	Master passwords are hashed before storing in the database
•	Account passwords are encrypted
•	Sensitive operations require master password verification
•	Verification codes expire after use
•	Security questions are linked to user accounts
________________________________________
 Functional Scope
•	Registered users can:
o	Log in to the system
o	Add, update, delete, and view passwords
o	Change profile details (name, email, password)
o	Recover forgotten passwords using security questions
•	Only authenticated users can access password data
•	Duplicate emails are prevented during registration and update
________________________________________
 Application Architecture
The application follows a modular, layered architecture:
UI Layer
 └── MainMenu (console interaction)

Service Layer
 └── Business logic
 └── Validations & exception handling

DAO Layer
 └── JDBC-based database operations

Utility Layer
 └── Encryption, hashing, DB connection

Database Layer
 └── MySQL
________________________________________
🗄️ Database Design
Tables Used
•	users
•	password_entries
•	security_questions
•	verification_codes
Concepts Applied
•	Primary Keys
•	Foreign Keys
•	One-to-many relationships
•	Normalized schema design
________________________________________
 Technologies Used
•	Java (Core Java)
•	JDBC
•	MySQL
•	SHA-256 hashing
•	AES encryption
•	OOP principles
•	Exception handling & validations
________________________________________
 Definition of Done (DoD)
•	Fully working console application
•	All functional requirements implemented
•	Secure password handling (hashing + encryption)
•	Password recovery using security questions
•	Database integration using JDBC
•	Code pushed to GitHub for technical evaluation
•	ER Diagram created
•	Application architecture diagram prepared
________________________________________
ER Diagrams (Included in Project)
 ________________________________________  How to Run
1.	Clone the repository
2.	git clone https://github.com/your-username/RevPasswordManager.git
3.	Import into Eclipse / IntelliJ
4.	Configure MySQL database credentials
5.	Create database tables
6.	Run MainMenu.java
________________________________________
 Learning Outcomes
•	Real-world authentication flows
•	Difference between validations and exceptions
•	Secure password storage techniques
•	JDBC + SQL integration
•	Clean layered application design
________________________________________
 Author
Dijendra Pavan Kumar Gudivaka
Java Developer 
________________________________________
 Notes
This project was developed as part of a technical learning initiative and is suitable for college evaluation, interviews, and backend learning demonstrations.

