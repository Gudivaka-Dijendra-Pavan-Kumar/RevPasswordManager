🔐 RevPasswordManager

RevPasswordManager is a console-based Password Manager application developed using Java, JDBC, and MySQL.
It allows users to securely store and manage multiple account passwords using a single master account, with proper authentication, validation, and recovery mechanisms.
This project follows real-world application design principles such as layered architecture, encryption, validations, and exception handling.
________________________________________
📌 Key Features

👤 User Management
•	User Registration with:
o	Email validation
o	Strong password validation
o	Security question & answer
•	Login using email and master password
•	Logout functionality
•	Profile Update:
o	Change name
o	Change email (with duplicate email check)
o	Change master password (with verification)
________________________________________
🔐 Security & Authentication

•	Master passwords are hashed (SHA-256) before storing in database
•	Account passwords are encrypted using AES
•	Forgot Password feature (available only when logged out):
o	Security question verification
o	Time-based verification code
•	Sensitive operations require master password re-verification
________________________________________
🔑 Password Management

•	Add passwords for multiple accounts (Gmail, Facebook, etc.)
•	List all saved account names
•	View a specific account password
•	Update an existing account password
•	Delete an account password
________________________________________
🏗️ Project Architecture

The application follows a Layered Architecture:
UI Layer
 └── MainMenu (Console interaction)

Service Layer
 └── Business logic & validations

DAO Layer
 └── Database access using JDBC

Utility Layer
 └── Encryption, DB connection, validators

Database Layer
 └── MySQL
________________________________________
🛠️ Technologies Used

•	Java (Core Java)
•	JDBC
•	MySQL
•	SHA-256 hashing
•	AES encryption
•	OOP concepts
•	Exception handling & validations
________________________________________
📂 Database Tables

•	users – stores user details and master password hash
•	security_questions – stores security questions and hashed answers
•	password_entries – stores encrypted account passwords
•	verification_codes – stores forgot-password verification codes
________________________________________
🚀 How to Run the Project

1.	Clone the repository:
2.	git clone https://github.com/your-username/RevPasswordManager.git
3.	Import the project into your Java IDE (Eclipse / IntelliJ)
4.	Configure MySQL database and update DB credentials in DBConnection
5.	Create required tables
6.	Run MainMenu.java

