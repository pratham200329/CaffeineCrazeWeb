# ☕ Caffeine Craze – Online Coffee Shop Web Application

## 🚀 Project Overview

Caffeine Craze is a full-stack web application that simulates a modern online coffee ordering system. It enables users to browse coffee products, manage a shopping cart, and place orders seamlessly. Administrators can manage products, users, and orders through a dedicated dashboard.

The application is built using **Java JSP, MySQL, Bootstrap 5, and JavaScript**, following a **three-tier architecture** and **MVC design pattern** for scalability, maintainability, and performance.

---

## ✨ Features

### 👤 User Features

* User Registration & Login (Secure Authentication with BCrypt)
* Browse Coffee Menu (Hot, Cold, Pastries, etc.)
* Add to Cart / Remove / Update Quantity
* Real-time Cart using localStorage
* Place Orders with Delivery Details
* Order History & Tracking
* Responsive UI for all devices

### 🛠️ Admin Features

* Admin Dashboard (Overview & Analytics)
* Manage Products (Add, Update, Delete)
* Manage Orders (Update Status)
* Manage Users (View & Control Access)

---

## 🏗️ System Architecture

The project follows a **Three-Tier Architecture**:

1. **Presentation Layer** – JSP, HTML, CSS, Bootstrap
2. **Business Logic Layer** – Java (JSP Scriptlets, JDBC)
3. **Data Layer** – MySQL Database

Additionally, it implements the **MVC (Model-View-Controller)** pattern:

* **Model** → MySQL Database
* **View** → JSP + Bootstrap UI
* **Controller** → Java logic inside JSP

---

## 🧰 Tech Stack

| Technology    | Purpose                 |
| ------------- | ----------------------- |
| Java JSP      | Server-side development |
| MySQL         | Database management     |
| JDBC          | Database connectivity   |
| Bootstrap 5   | Responsive UI           |
| JavaScript    | Client-side logic       |
| BCrypt        | Password security       |
| Apache Tomcat | Server deployment       |

---

## 🔐 Security Features

* BCrypt Password Hashing
* SQL Injection Prevention using Prepared Statements
* Session Management (HttpSession)
* Role-Based Access Control (Admin/User)

---

## 🛒 Core Modules

### 1. Authentication Module

Handles login, registration, and session management securely.

### 2. Product Module

Displays coffee items dynamically with category-based filtering.

### 3. Cart Module

Client-side cart using localStorage for fast and real-time updates.

### 4. Order Processing Module

Uses JDBC transactions to ensure data consistency across multiple tables.

### 5. User Profile Module

Displays user details and complete order history.

### 6. Admin Dashboard Module

Provides analytics, order management, and system control.

---

## 🗄️ Database Design

Main Tables:

* users
* products
* orders
* order_items
* order_delivery

Relational integrity is maintained using foreign keys and transactions.

---

## ⚙️ Installation & Setup

### Prerequisites

* Java JDK 11+
* Apache Tomcat 10+
* MySQL 8+
* NetBeans / IntelliJ
* Git

### Steps

1. Clone the repository:

```bash
git clone https://github.com/your-username/caffeine-craze.git
```

2. Import project into IDE

3. Configure MySQL Database:

* Create database `caffeine_craze`
* Import SQL file

4. Update DB credentials in project

5. Deploy on Apache Tomcat

6. Run application:

```
http://localhost:8080/CaffeineCraze
```

---

## 📸 Screenshots

(Add your screenshots here: Home Page, Menu, Cart, Admin Dashboard)

---

## 🚀 Future Enhancements

* Payment Gateway Integration (Razorpay/Stripe)
* Real-time Order Tracking
* Email Notifications
* Mobile App (Android/iOS)
* AI-based Recommendation System
* Multi-branch Support

---

## 📚 Learning Outcomes

* MVC Architecture Implementation
* Database Design & Normalization
* Secure Web Development Practices
* Full-stack Application Development

---

## 👨‍💻 Author

**Pratham Mishra**
MCA (AI/ML) – Chandigarh University

---

## 📄 License

This project is for educational purposes.

---

⭐ If you like this project, don't forget to give it a star!
