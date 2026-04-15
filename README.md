# 🔐 Flask Authentication System

## 📌 Overview

This project is a **secure user authentication system** built using **Flask (Python)**, **SQLite**, and **HTML/CSS**. It demonstrates how a backend application handles user registration, login, session management, and protected routes.

The application follows a real-world authentication flow where user credentials are securely processed and validated.

---

## ⚙️ Features

* User Registration with validation
* Secure password storage using hashing
* User Login with credential verification
* Session-based authentication
* Protected dashboard access
* Logout functionality
* Flash messages for user feedback

---

## 🧠 Project Description

This project implements a complete authentication workflow:

### 🔹 User Registration

When a user registers, the system:

* Checks if the username already exists in the database
* Hashes the password using a secure hashing function
* Stores the username and hashed password in SQLite

This ensures that **plain text passwords are never stored**, improving security.

---

### 🔹 User Login

During login:

* The entered username is searched in the database
* The stored hashed password is retrieved
* The entered password is compared using hash verification

If valid, the user is successfully authenticated.

---

### 🔹 Session Management

After successful login:

* The username is stored in a session
* This session is used to maintain the user's login state

Only authenticated users can access the dashboard.

---

### 🔹 Protected Dashboard

The dashboard route is protected by:

* Checking whether a user session exists

If no session is found, the user is redirected to the login page.
This prevents unauthorized access.

---

### 🔹 Logout

When the user logs out:

* The session is cleared
* The user is redirected to the home page

---

### 🔹 Flash Messages

The system uses flash messages to:

* Show success messages (e.g., login success)
* Show error messages (e.g., invalid credentials)

This improves user experience by providing immediate feedback.

---

## 🔐 Security Highlights

* Password hashing using secure methods
* No storage of plain text passwords
* Session-based authentication
* Protected routes to prevent unauthorized access

---

## 🧠 Learning Outcomes

* Building authentication systems using Flask
* Handling user sessions securely
* Implementing password hashing
* Connecting backend with frontend forms
* Managing database operations using SQLite

---

## 👩‍💻 Author

**Amrutha D N**
