# 💰 Wallet Management & Transactions API

A **Spring Boot RESTful API** for wallet management, supporting **user registration, authentication, wallet funding, withdrawals, transfers, merchant payments**, and **transaction PIN/OTP verification**.

---

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Authentication & Security](#authentication--security)
- [Database Schema](#database-schema)
- [Postman Collection](#postman-collection)
- [Future Enhancements](#future-enhancements)

---

## 📝 Project Overview
This project allows users to:
- Register and login with email/password
- Create and manage wallets
- Fund wallets and withdraw money
- Transfer funds between wallets
- Pay merchants
- View transaction history
- Set and use transaction PINs for secure operations  

The system uses **JWT authentication**, **Spring Security**, and **Spring Data JPA** for data management.

---

## ✨ Features
- **User Management:** Register, login, and profile management.
- **Wallet Management:** Each user has a wallet with an account number.
- **Transaction Management:** All transfers, withdrawals, and deposits are recorded.
- **Merchant Payments:** Pay merchants and record transactions.
- **Transaction PIN:** Optional security layer for sensitive operations.
- **JWT Security:** Secure, stateless authentication for API calls.
- **Global Exception Handling:** Centralized error management for API responses.

---

## 🛠 Technologies Used
- Java 17
- Spring Boot 3.x
- Spring Data JPA / Hibernate
- Spring Security + JWT
- PostgreSQL / MySQL (configurable)
- Maven
- Lombok (optional)
- Postman (for testing)

---

## 🚀 Getting Started

### Prerequisites
- Java 17+
- Maven 3+
- PostgreSQL/MySQL
- Postman (for testing)

### Clone the Repo
```bash
git clone https://github.com/<your-username>/wallet-management-api.git
cd wallet-management-api

### Configure application.propertie
```bash
spring.datasource.url=jdbc:postgresql://localhost:5432/wallet_db
spring.datasource.username=your_db_username
spring.datasource.password=your_db_password
spring.jpa.hibernate.ddl-auto=update

jwt.secret=YourBase64EncodedSecretKey
jwt.expiration=1800000

### Run the Application
```bash
mvn spring-boot:run


