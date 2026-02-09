# Module 2 – Smart Device Management

## Overview
This module implements smart device management for the Smart Home Energy
Management System (SHEMS).

It is responsible for registering, controlling, and managing smart devices
owned by users, while providing administrators with centralized control.
This module represents the device control layer of the system.

---

## Responsibilities
- Register smart devices with metadata
- Maintain device ownership per user
- Control device ON / OFF states
- Provide admin-level system-wide device control
- Supply device data for energy tracking and analytics

---

## Technology Stack
- Java 17
- Spring Boot
- Spring MVC
- Spring Data JPA
- Thymeleaf
- MySQL
- Maven

---

## Features

### User Features
- Add smart devices (name, type, location, power rating)
- View assigned devices
- Toggle device ON / OFF
- Delete devices

### Admin Features
- View all devices across users
- Control any device system-wide
- Delete devices globally

---

## Project Structure

```
Module_2_Device_Management/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/role/implementation/
│   │   │       └── devicemanagement/
│   │   │           ├── controller/
│   │   │           │   └── DeviceController.java
│   │   │           ├── service/
│   │   │           │   ├── DeviceService.java
│   │   │           │   └── DeviceServiceImpl.java
│   │   │           ├── repository/
│   │   │           │   └── DeviceRepository.java
│   │   │           └── model/
│   │   │               └── Device.java
│   │   │
│   │   └── resources/
│   │       ├── templates/
│   │       │   ├── devices.html
│   │       │   ├── adminDevices.html
│   │       │   └── admin-home.html
│   │       │
│   │       └── application.properties
│   │
├── pom.xml
└── README.md
```

---

## How to Run

Create database:
```
CREATE DATABASE shems_devices;
```

Run application:
```
mvn spring-boot:run
```

Open in browser:
```
http://localhost:8080/devices
```

---

## Role in System
This module manages all smart device operations and acts as the foundation
for energy tracking, analytics, scheduling, and automation modules in SHEMS.

---

## Summary
Module 2 provides secure, centralized, and real-time smart device management,
enabling effective appliance control and supporting intelligent energy
optimization across the system.
