# FinPay – Student Digital Wallet and Cashback Platform

**FinPay** is a student-focused digital wallet application designed to simplify digital payments within a campus environment. It allows students to manage their wallet balance, add money, make payments to campus merchants, earn cashback, and view transaction history.

The application is developed using **React, FastAPI, Python, and SQLite** as a team project.

---

## Table of Contents

1. [Problem Statement](#1-problem-statement)
2. [Objectives](#2-objectives)
3. [Project Overview](#3-project-overview)
   - [3.1 System Architecture](#31-system-architecture)
   - [3.2 Technologies Used](#32-technologies-used)
   - [3.3 Execution Steps](#33-execution-steps)
   - [3.4 Results](#34-results)
4. [Application Modules](#4-application-modules)
5. [Database Design](#5-database-design)
6. [Application Features](#6-application-features)
7. [Installation and Setup](#7-installation-and-setup)
8. [Future Enhancements](#8-future-enhancements)
9. [Conclusion](#9-conclusion)

---

## 1. Problem Statement

In college environments, students frequently make payments for food, stationery, books, and other campus-related services. Managing these transactions through cash or separate payment methods can be inconvenient.

There is a need for a centralized digital wallet system that allows students to manage their money, make payments to campus merchants, track transactions, and receive cashback benefits.

**FinPay** addresses this problem by providing a simple and user-friendly digital payment platform specifically designed for campus transactions.

## 2. Objectives

The main objectives of FinPay are:

- To develop a digital wallet application for students.
- To provide secure student authentication.
- To allow students to add money to their wallets.
- To enable digital payments to registered campus merchants.
- To implement merchant-based cashback calculations.
- To maintain transaction history.
- To display wallet balance and cashback information.
- To provide an easy-to-use dashboard for managing wallet activities.

## 3. Project Overview

FinPay follows a frontend-backend architecture. The React frontend provides the user interface, while the FastAPI backend handles authentication, business logic, payment processing, and database operations.

### 3.1 System Architecture

The application consists of three major layers:

1. **Frontend:** React provides the user interface and handles user interactions.
2. **Backend:** FastAPI processes requests, manages authentication, and implements wallet and payment operations.
3. **Database:** SQLite stores student details, wallet information, merchants, transactions, and related records.

**Application Flow:**

```text
        Student
           |
           v
    React Frontend
           |
           v
     FastAPI Backend
           |
     Business Logic
           |
           v
      SQLite Database
```

### 3.2 Technologies Used

| Component | Technology |
|---|---|
| Frontend | React.js |
| Frontend Build Tool | Vite |
| Backend | Python |
| Backend Framework | FastAPI |
| Database | SQLite |
| ORM | SQLAlchemy |
| Authentication | JWT |
| Password Security | bcrypt |
| API Testing | Swagger UI |
| Version Control | Git and GitHub |

### 3.3 Execution Steps

The following steps describe the execution of the FinPay application:

1. The student opens the FinPay application through the frontend.
2. The student logs in using their credentials.
3. The backend validates the authentication request.
4. After successful authentication, the dashboard displays wallet information.
5. The student can add money to the wallet.
6. The student can select a merchant and make a payment.
7. The backend processes the payment and calculates applicable cashback.
8. The wallet balance and transaction records are updated.
9. The student can view recent transactions and cashback details.

### 3.4 Results

The FinPay application was successfully developed and tested.

The following functionalities were implemented and verified:

- Student login and authentication.
- Wallet balance display.
- Add Money functionality.
- Payment processing for campus merchants.
- Merchant-specific cashback calculation.
- Transaction history.
- Cashback details.
- Dashboard navigation and logout.

The application successfully demonstrates a working campus-based digital wallet and payment system.

## 4. Application Modules

### 4.1 Student Module

Manages student information and authentication.

### 4.2 Wallet Module

Displays the student's wallet balance and supports adding money.

### 4.3 Payment Module

Processes payments made by students to registered merchants.

### 4.4 Merchant Module

Maintains merchant information and applicable cashback rates.

### 4.5 Cashback Module

Calculates cashback based on the merchant's configured cashback percentage.

### 4.6 Transaction Module

Maintains payment and wallet transaction records for tracking purposes.

## 5. Database Design

FinPay uses SQLite as its relational database and SQLAlchemy for database operations.

The backend manages records related to:

- Students
- Wallets
- Wallet tiers
- Wallet top-ups
- Merchants
- Merchant categories
- Cashback rules
- Payment transactions

These records support wallet management, payment processing, and transaction tracking.

## 6. Application Features

- **Student Dashboard:** Displays wallet balance and account information.
- **My Wallet:** Allows students to view and manage their wallet.
- **Add Money:** Supports wallet top-ups.
- **Make a Payment:** Enables payments to campus merchants.
- **Cashback:** Displays cashback earned through eligible transactions.
- **Transactions:** Provides access to transaction history.
- **Authentication:** Supports secure login and logout.

## 7. Installation and Setup

### Prerequisites

Install the following before running the application:

- Python 3
- Node.js and npm
- Git

### Step 1: Backend Setup

Navigate to the backend folder from the FinPay project directory:

```powershell
cd backend
```

Create a Python virtual environment:

```powershell
python -m venv venv
```

Activate the virtual environment in Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

Install the required dependencies:

```powershell
pip install -r requirements.txt
```

Start the backend server:

```powershell
python -m uvicorn main:app --reload
```

**Backend URL:** `http://127.0.0.1:8000`

**Swagger API Documentation:** `http://127.0.0.1:8000/docs`

### Step 2: Frontend Setup

Open another terminal in the FinPay project directory and navigate to the frontend folder:

```powershell
cd frontend
```

Install dependencies:

```powershell
npm install
```

Start the frontend development server:

```powershell
npm run dev
```

For Windows PowerShell, if npm scripts are blocked, use:

```powershell
npm.cmd install
npm.cmd run dev
```

**Frontend URL:** `http://localhost:5173`

### Step 3: Access the Application

Open the frontend URL in your browser:

`http://localhost:5173`

Ensure that both the backend and frontend servers are running.

## 8. Future Enhancements

The following features can be considered for future development:

- QR-code-based payments.
- Integration with real payment gateways.
- Admin dashboard for merchant and student management.
- Detailed monthly spending reports.
- Payment notifications.
- Improved security and fraud detection.
- Deployment to a cloud platform.

## 9. Conclusion

FinPay successfully demonstrates the development of a campus-based digital wallet and cashback platform. It provides students with a centralized system to manage wallet balances, add money, make merchant payments, earn cashback, and track transactions.

The project integrates frontend development, backend API development, database management, and authentication into a single application.

Overall, FinPay provides a practical implementation of a digital payment system that can be further extended with additional features and real-world payment integrations.

---

**Project Repository:** [FinPay – GitHub](https://github.com/Krupa1310/FinPay)