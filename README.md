# Smart Home Energy Management System (SHEMS)

## Overview
Smart Home Energy Management System (SHEMS) is a role-based web application
built using Spring Boot to monitor, control, and optimize energy usage in
smart homes.

The system allows USERS to manage smart devices, track personal energy
consumption, and automate device schedules, while ADMINS monitor system-wide
usage, analyze energy patterns, and define energy usage policies that are
automatically enforced across the platform.

---

## Project Demo
Voice Explanation Demo (PPT + Live Demo):
https://drive.google.com/file/d/1NcrOQ2NJSLJAei7Wio2MC46r-o_BtUFb/view

Video Breakdown:
- 00:00 – 06:47  → PPT Explanation
- 06:48 – End    → Live Project Demo

---

## Key Objectives
- Enable users to control and automate smart devices
- Track and analyze real-time energy consumption
- Provide data-driven insights through analytics dashboards
- Allow admins to define and enforce energy usage policies
- Optimize overall energy consumption through automation

---

## Role-Based Features

### User Capabilities
- Secure registration and login
- Add and manage personal smart devices
- Turn devices ON / OFF
- Track daily energy consumption
- View weekly and monthly analytics
- Create device automation schedules

### Admin Capabilities
- View and manage all users and devices
- Monitor system-wide energy consumption
- Analyze high energy usage patterns
- Define energy usage policies
- Enforce policies automatically using schedulers
- Generate system-level energy reports

---

## System Modules

| Module | Responsibility |
|------|----------------|
| Module 1 – Authentication & Security | Secure login, registration, role-based access |
| Module 2 – Device Management | Smart device registration and control |
| Module 3 – Energy Tracking | Real-time energy consumption tracking |
| Module 4 – Analytics Dashboard | Energy usage analysis and insights |
| Module 5 – Scheduling & Automation | User scheduling and admin policy enforcement |

---

## Architecture Overview
The system follows a modular, layered architecture:

- Presentation Layer (Thymeleaf, HTML, CSS)
- Controller Layer (Spring MVC)
- Service Layer (Business Logic)
- Repository Layer (Spring Data JPA)
- Database Layer (MySQL)
- Scheduler Layer (Automation & Policy Enforcement)

This design ensures scalability, maintainability, and clear separation of
concerns.

---

## Technology Stack

### Backend
- Java 17
- Spring Boot
- Spring MVC
- Spring Security
- Spring Data JPA

### Frontend
- Thymeleaf
- HTML
- CSS

### Database
- MySQL

### Automation & Build
- Spring Scheduler
- Maven

---

## How to Run

Create database:
```
CREATE DATABASE shems;
```

Clone repository:
```
git clone https://github.com/your-username/Smart-Home-Energy-Management-System.git
```

Configure database credentials in:
```
src/main/resources/application.properties
```

Run application:
```
mvn spring-boot:run
```

Open in browser:
```
http://localhost:8080
```

---

## What This Project Demonstrates
- Real-world Spring Boot application design
- Secure authentication and role-based authorization
- Modular system architecture
- Real-time data tracking and analytics
- Policy-based automation using schedulers
- Clear separation between user and admin responsibilities

---

## Developd by
Fahim Shaik  
Software Engineer | Java | Spring Boot

---

## License
This project is licensed under the MIT License.
