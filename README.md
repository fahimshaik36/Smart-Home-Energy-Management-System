# Smart Home Energy Management System (SHEMS)

A Spring Boot web application to manage smart home devices, track energy usage, and automate device scheduling.

---

## About the Project

Smart Home Energy Management System (SHEMS) is a backend-focused web application built to practice real-world Java and Spring Boot development concepts.

The system allows users to manage smart devices, monitor energy consumption, automate device schedules, and view analytics dashboards.  
An admin role is included to monitor system-wide activity and generate reports.

---

## Features

### User
- Secure registration and login
- Add and manage smart devices
- Turn devices ON/OFF
- View daily energy usage
- View weekly and monthly analytics
- Create device automation schedules

### Admin
- View all users and devices
- Monitor system-wide energy analytics
- Detect high energy usage
- Generate energy reports

---

## Modules Implemented

| Module | Description |
|------|-------------|
| Authentication & Security | Login, registration, role-based access |
| Device Management | Add, update, delete, and control devices |
| Energy Tracking | Track device-level and user-level energy usage |
| Analytics Dashboard | Energy charts and usage insights |
| Scheduling & Automation | Automatic device ON/OFF scheduling |
| Reporting | PDF report generation |

---

## Tech Stack

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

### Other
- Spring Scheduler
- Maven

---

## How to Run

1. Create the database  
   CREATE DATABASE shems;

2. Clone the repository  
   git clone https://github.com/your-username/Smart-Home-Energy-Management-System.git

3. Update MySQL credentials in `application.properties`

4. Run the application  
   mvn spring-boot:run

5. Open in browser  
   http://localhost:8080

---

## What I Learned

- Building a complete Spring Boot backend application
- Implementing authentication and authorization
- Working with relational databases using JPA
- Scheduling background tasks
- Designing a modular and maintainable architecture

---

## Developed By

Fahim Shaik  
Software Engineer | Java | Spring Boot

---

## License

MIT License
