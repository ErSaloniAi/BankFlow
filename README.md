# 🏦 BankFlow — Online Banking System

**BankFlow** is a console-based **Online Banking System built with Core Java** that simulates essential banking operations such as account registration, secure login, deposits, withdrawals, transaction tracking, loan management, EMI payments, and fixed deposits.

The project was designed to demonstrate practical **Java programming, Object-Oriented Programming, validation, arrays, and application-level banking logic** through an interactive command-line application.

---

## ✨ Features

### 👤 Account Management

* New customer registration
* Automatic Customer ID generation
* Automatic Account Number generation
* IFSC code generation
* Profile management
* Initial account balance setup

### 🔐 Authentication & Security

* Customer ID and password-based login
* 4-digit mPIN authentication for sensitive transactions
* Password validation with:

  * Minimum and maximum length
  * Uppercase character
  * Lowercase character
  * Number
  * Special character
  * No spaces
* Limited mPIN attempts for transactions

### 💰 Banking Operations

* Deposit money
* Withdraw money
* Check account balance
* Maintain transaction history
* View complete transaction records

### 🏠 Loan Management

BankFlow supports two types of loans:

**Personal Loan**

* Apply for a personal loan
* Specify loan purpose
* Calculate monthly EMI
* Pay EMI
* Repay outstanding loan amount
* View loan details

**Home Loan**

* Apply for a home loan
* Store property information
* Calculate monthly EMI
* Pay EMI
* Repay outstanding loan amount
* View loan details

### 🏦 Fixed Deposit

* Create fixed deposits
* Maintain multiple FD records
* View FD details
* Track FD status
* Close an active FD
* Calculate the amount received on FD closure

### ✅ Input Validation

BankFlow validates important user inputs such as:

* Name
* Mobile number
* Aadhaar number
* PAN number
* Date of birth
* Gmail address
* Password
* mPIN
* Initial account balance

---

## 🧠 Java Concepts Demonstrated

This project focuses on **Core Java** and demonstrates:

* Object-Oriented Programming
* Classes and Objects
* Encapsulation
* Inheritance
* Constructors
* Method Overloading
* Method Overriding
* Inner Classes
* Arrays
* Loops
* Conditional Statements
* Exception Handling
* String Manipulation
* Regular Expressions
* Java Time API
* Scanner-based input handling
* Modular application design

---

## 🏗️ Project Structure

```text
BankFlow/
│
├── OnlineBanking.java
│
└── README.md
```

The main Java file contains the application's core components, including:

```text
User
├── Profile Management
├── Account Balance
├── Transactions
├── Personal Loan
├── Home Loan
└── Fixed Deposits

Validations
├── Name Validation
├── Mobile Validation
├── Aadhaar Validation
├── PAN Validation
├── Email Validation
├── Date Validation
├── Password Validation
├── mPIN Validation
└── Balance Validation

BankingOperations
├── Registration
├── Login
├── Deposit
├── Withdrawal
├── Balance Checking
├── Transactions
├── Loan Operations
└── Fixed Deposit Operations

LoanManagement
├── Personal Loan
└── Home Loan

FixedDeposit
└── FD Management
```

---

## 🔄 Application Flow

```text
              ┌─────────────────┐
              │     BankFlow    │
              └────────┬────────┘
                       │
              ┌────────▼────────┐
              │   Registration  │
              └────────┬────────┘
                       │
             Generate Account
             Customer ID & IFSC
                       │
              ┌────────▼────────┐
              │      Login      │
              └────────┬────────┘
                       │
              ┌────────▼────────┐
              │  Account Menu   │
              └────────┬────────┘
                       │
       ┌───────────────┼────────────────┐
       │               │                │
       ▼               ▼                ▼
   Banking          Loans              FD
 Operations       Management       Management
       │               │                │
       ├─ Deposit      ├─ Personal      ├─ Create FD
       ├─ Withdraw     ├─ Home          ├─ View FD
       ├─ Balance      ├─ EMI           └─ Close FD
       └─ History      └─ Repayment
```

---

## 🛠️ Technologies Used

| Technology              | Purpose                            |
| ----------------------- | ---------------------------------- |
| **Java**                | Core application development       |
| **Java SE**             | Standard Java functionality        |
| **OOP**                 | Application structure and modeling |
| **Arrays**              | User, transaction and FD storage   |
| **Scanner**             | Console input                      |
| **Java Time API**       | Date/time-related functionality    |
| **Regular Expressions** | Input validation                   |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have:

* **Java JDK 8 or later**
* Any Java IDE such as IntelliJ IDEA, Eclipse, VS Code, or NetBeans

Check your Java installation:

```bash
java -version
```

---

### Clone the Repository

```bash
git clone https://github.com/your-username/BankFlow.git
```

Move into the project directory:

```bash
cd BankFlow
```

---

### Run the Application

Compile the Java file:

```bash
javac OnlineBanking.java
```

Run the application:

```bash
java OnlineBanking
```

Follow the instructions displayed in the terminal.

---

## 💻 Example Operations

After registering and logging in, users can perform operations such as:

```text
1. View Profile
2. Deposit Money
3. Withdraw Money
4. Check Balance
5. View Transactions
6. Apply for Loan
7. Pay EMI
8. Create Fixed Deposit
9. View Fixed Deposits
10. Close Fixed Deposit
11. Logout
```

*The exact menu options depend on the current implementation.*

---

## 📊 Data Management

BankFlow currently uses **in-memory storage** using Java arrays.

For example:

```java
User[] users;
```

Transaction records are maintained using:

```java
String[] transaction;
```

Fixed deposits are maintained using:

```java
FixedDeposit[] fixedDeposits;
```

This makes the project suitable for demonstrating Java data structures and application logic without requiring an external database.

---

## 🔒 Security Note

BankFlow is an **educational banking simulation** and is not intended for real financial transactions.

It does not currently use:

* Database encryption
* Production authentication
* Password hashing
* Banking APIs
* Real payment gateways
* Persistent cloud storage

Never use real banking credentials, Aadhaar numbers, PAN numbers, or financial information while testing the application.

---

## 🚧 Future Enhancements

The project can be extended into a full-scale banking application by adding:

* 🗄️ MySQL/PostgreSQL database
* 🔐 Password hashing and stronger authentication
* 👨‍💼 Admin and customer roles
* 🖥️ JavaFX graphical interface
* 🌐 Web-based banking interface
* 📧 Email transaction notifications
* 📱 SMS notifications
* 📈 Banking analytics and reports
* 🔎 Searchable transaction history
* 💳 Fund transfer between accounts
* 🧾 Downloadable account statements
* ☁️ Cloud deployment
* 🔑 OTP / multi-factor authentication
* 🏦 More loan and investment products

---

## 🎯 Learning Objectives

BankFlow was developed to gain practical experience with:

1. Designing a multi-feature Java application
2. Applying Object-Oriented Programming principles
3. Managing multiple objects using arrays
4. Implementing user authentication
5. Validating real-world user input
6. Building transaction-based application logic
7. Implementing financial calculations such as EMI
8. Structuring related functionality into classes
9. Handling user interaction through the command line

## 📄 License

This project is available under the **MIT License**.

---

⭐ If you found this project useful, consider giving the repository a star!
