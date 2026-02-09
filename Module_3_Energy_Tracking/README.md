# Module 3 – Real-Time Energy Tracking

## Overview
This module implements real-time energy tracking for the Smart Home Energy
Management System (SHEMS).

It is responsible for monitoring device usage duration, calculating energy
consumption, and storing historical energy data. This module acts as the
energy data foundation for analytics, reporting, and automation.

---

## Responsibilities
- Track smart device ON / OFF duration
- Calculate energy consumption using power ratings
- Store historical energy usage records
- Associate energy data with users and devices
- Supply energy data to analytics and scheduling modules

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
- Device-level energy consumption tracking
- User-level energy usage aggregation
- Time-based energy calculation
- Historical energy usage storage
- Support for peak usage detection

---

## Project Structure

```
Module_3_Energy_Tracking/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/role/implementation/
│   │   │       └── energytracking/
│   │   │           ├── controller/
│   │   │           │   └── EnergyTrackingController.java
│   │   │           ├── service/
│   │   │           │   ├── EnergyTrackingService.java
│   │   │           │   └── EnergyTrackingServiceImpl.java
│   │   │           ├── repository/
│   │   │           │   └── EnergyTrackingRepository.java
│   │   │           └── model/
│   │   │               └── EnergyUsage.java
│   │   │
│   │   └── resources/
│   │       ├── templates/
│   │       │   ├── analytics.html
│   │       │   ├── dashboard.html
│   │       │   └── energy-reports.html
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
CREATE DATABASE shems_energy;
```

Run application:
```
mvn spring-boot:run
```

Open in browser:
```
http://localhost:8080/energy
```

---

## Role in System
This module records and manages all energy consumption data and serves as
the primary data source for analytics dashboards, reporting, and automated
energy optimization within SHEMS.

---

## Summary
Module 3 enables accurate and continuous energy consumption tracking,
providing reliable data that powers analytics, reporting, and intelligent
automation across the Smart Home Energy Management System.
