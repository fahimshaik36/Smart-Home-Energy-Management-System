# Module 4 – Energy Analytics Dashboard

## Overview
This module implements the analytics and visualization layer for the Smart
Home Energy Management System (SHEMS).

It analyzes energy consumption data collected from the Energy Tracking
module and presents meaningful insights through dashboards for users and
administrators. This module enables data-driven decisions and energy
optimization.

---

## Responsibilities
- Analyze device-level and user-level energy consumption
- Generate daily, weekly, and monthly usage summaries
- Identify peak and high energy usage patterns
- Provide system-wide analytics for administrators
- Transform raw energy data into actionable insights

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

### User Analytics
- Personal energy usage dashboard
- Device-wise energy consumption breakdown
- Daily, weekly, and monthly usage trends
- Peak usage identification

### Admin Analytics
- System-wide energy consumption overview
- High energy usage user detection
- Top energy-consuming device analysis
- Overall usage pattern monitoring

---

## Project Structure

```
Module_4_Analytics_Dashboard/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/role/implementation/
│   │   │       └── analytics/
│   │   │           ├── controller/
│   │   │           │   └── AnalyticsController.java
│   │   │           ├── service/
│   │   │           │   ├── AnalyticsService.java
│   │   │           │   └── AnalyticsServiceImpl.java
│   │   │           ├── repository/
│   │   │           │   └── AnalyticsRepository.java
│   │   │           └── model/
│   │   │               └── AnalyticsReport.java
│   │   │
│   │   └── resources/
│   │       ├── templates/
│   │       │   ├── analytics.html
│   │       │   ├── admin-analytics.html
│   │       │   ├── dashboard.html
│   │       │   └── dashboard-home.html
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
CREATE DATABASE shems_analytics;
```

Run application:
```
mvn spring-boot:run
```

Open in browser:
```
http://localhost:8080/analytics
```

---

## Role in System
This module converts raw energy consumption data into structured analytics
and insights. It supports user awareness, administrative monitoring, and
energy optimization decisions within the SHEMS platform.

---

## Summary
Module 4 transforms energy usage data into clear, actionable analytics,
enabling users and administrators to understand consumption patterns and
optimize energy usage effectively.
