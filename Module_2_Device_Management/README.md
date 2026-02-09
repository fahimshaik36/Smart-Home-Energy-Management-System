# Module 2 – Smart Device Management

## Overview
This module implements smart device management for the Smart Home Energy
Management System (SHEMS).

It handles device registration, ownership, and real-time control, and
provides administrators with centralized monitoring. This module acts as
the device control layer of the application.

---

## Responsibilities
- Register and manage smart devices
- Control device ON / OFF states
- Maintain device ownership and metadata
- Provide system-wide device visibility for administrators
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
- Add smart devices with metadata
- View assigned devices
- Toggle device status (ON / OFF)
- Remove devices when required

### Admin Features
- View all devices across users
- Control any device system-wide
- Delete devices globally

---

## Project Structure

Module_2_Device_Management/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/role/implementation/
│   │   │       ├── devicemanagement/
│   │   │       │   ├── controller/
│   │   │       │   │   └── DeviceController.java
│   │   │       │   ├── service/
│   │   │       │   │   ├── DeviceService.java
│   │   │       │   │   └── DeviceServiceImpl.java
│   │   │       │   └── repository/
│   │   │       │       └── DeviceRepository.java
│   │   │       │
│   │   │       └── model/
│   │   │           └── Device.java
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

---

## How to Run

Create database:
CREATE DATABASE shems_devices;

Run application:
mvn spring-boot:run

Open in browser:
http://localhost:8080/devices

---

## Role in System
This module provides centralized smart device control and serves as the
foundation for energy tracking, analytics, scheduling, and automation
within SHEMS.

---

## Summary
Module 2 enables secure and real-time smart device management, allowing
efficient control of appliances and supporting intelligent energy
optimization.
