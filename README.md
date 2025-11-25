# ATM Simulator System

**One-line summary:**  
A console-based Java program simulating an ATM system with basic user authentication, account operations (withdraw, deposit, balance check), and data persistence.

---

## Table of Contents
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Architecture](#architecture)  
- [Setup & Run](#setup--run)  
- [Usage](#usage)  
- [Tests](#tests)  
- [Future Improvements](#future-improvements)  
- [What I Learned](#what-i-learned)  
- [License](#license)

---

## Features
- User login/authentication (via account number & PIN)  
- View current balance  
- Withdraw cash, Deposit cash  
- Transaction history (if implemented)  
- Secure handling of incorrect credentials  
- Clean console menu-driven UI

---

## Tech Stack
- Language: Java  
- Data Storage: (mention what you are using — e.g., file system, in-memory, JDBC+database)  
- Build System: (Maven / Gradle / plain Java)  
- Version Control: Git + GitHub  
- (Optional) Testing: JUnit  
- (Optional) CI/CD: GitHub Actions

---

## Architecture
Briefly describe how the system is structured. Example:
- `ATMSystem` (main class) → handles user menu and input  
- `AccountService` → business logic for account operations  
- `AccountRepository` → data access for accounts  
- `models/Account.java` → account entity with fields: accountNumber, pin, balance, transactionList  
- Data persisted in a file/DB so that state remains between runs  
- Example flow: Login → Menu → Choose option → Service layer → Update repository → Save → Show result

Include a simple ASCII diagram or link to `docs/architecture.png`.

---

## Setup & Run

1. **Clone the repo**  
   ```bash
   git clone https://github.com/YOUR-USERNAME/ATM-Simulator-System.git
   cd ATM-Simulator-System
