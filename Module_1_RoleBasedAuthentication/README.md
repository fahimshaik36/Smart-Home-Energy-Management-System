# Module 1 – Role-Based Authentication & Authorization

## Overview
This module implements secure authentication and role-based authorization
for the Smart Home Energy Management System (SHEMS).

It manages user identity, access control, session handling, and password
recovery, and serves as the security foundation of the entire application.

---

## Responsibilities
- Authenticate users securely
- Authorize access based on roles (USER / ADMIN)
- Protect application endpoints
- Manage login sessions
- Handle password recovery workflows

---

## Technology Stack
- Java 17
- Spring Boot
- Spring Security
- Spring MVC
- Spring Data JPA
- Thymeleaf
- MySQL
- Maven

---

## Features

### Authentication
- User registration and login
- BCrypt password encryption
- Secure session management
- Logout handling

### Authorization
- Role-based access control (USER / ADMIN)
- Protected routes using Spring Security
- Custom authentication success handler

### Password Recovery
- Forgot-password workflow
- Token-based password reset
- Email service integration

---

## Project Structure

```
Module_1_RoleBasedAuthentication/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/role/implementation/
│   │   │       ├── config/
│   │   │       │   ├── SpringSecurityConfig.java
│   │   │       │   ├── CustomSuccessHandler.java
│   │   │       │   └── GlobalModelAttributes.java
│   │   │       ├── controller/
│   │   │       │   ├── LoginController.java
│   │   │       │   ├── RegistrationController.java
│   │   │       │   ├── ForgotPasswordController.java
│   │   │       │   └── HomeController.java
│   │   │       ├── model/
│   │   │       │   ├── User.java
│   │   │       │   ├── Role.java
│   │   │       │   └── PasswordResetToken.java
│   │   │       ├── repository/
│   │   │       │   ├── UserRepository.java
│   │   │       │   ├── RoleRepository.java
│   │   │       │   └── PasswordResetTokenRepository.java
│   │   │       ├── service/
│   │   │       │   ├── DefaultUserService.java
│   │   │       │   ├── DefaultUserServiceImpl.java
│   │   │       │   └── MailService.java
│   │   │       └── RoleBasedAuthenticationApplication.java
│   │   └── resources/
│   │       ├── templates/
│   │       │   ├── login.html
│   │       │   ├── register.html
│   │       │   ├── forgot-password.html
│   │       │   ├── reset-password.html
│   │       │   ├── access-denied.html
│   │       │   └── home.html
│   │       └── application.properties
├── pom.xml
└── README.md
```

---

## How to Run

Create database:
CREATE DATABASE shems_auth;

Run application:
mvn spring-boot:run

Open in browser:
http://localhost:8080/login

---

## Role in System
Provides secure authentication and role-based authorization
for all other SHEMS modules.

---

## Summary
This module establishes secure access control and identity management,
forming the backbone of application security.
