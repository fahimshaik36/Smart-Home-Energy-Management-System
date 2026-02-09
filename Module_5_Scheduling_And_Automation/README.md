# Module 5 - Scheduling, Automation, and Energy Policy Enforcement

## Overview
This module implements scheduling, automation, and energy policy enforcement
for the Smart Home Energy Management System (SHEMS).

It allows USERS to automate their own devices using time-based schedules,
while enabling ADMINS to define and enforce system-wide energy policies.
This module acts as the control and enforcement layer of the system.

---

## Responsibilities
- Enable users to create ON / OFF schedules for their devices
- Execute scheduled automation using background schedulers
- Allow admins to define energy usage policies
- Enforce admin-defined policies across users and devices
- Log automation actions and policy violations

---

## Role-Based Capabilities

### User Capabilities
- Create device ON / OFF schedules
- Enable or disable personal schedules
- Automate device operation without manual control

### Admin Capabilities
- Define system-wide energy usage policies
- Set usage thresholds and control rules
- Enforce policies automatically
- Monitor policy violations and automation outcomes

---

## Technology Stack
- Java 17
- Spring Boot
- Spring Scheduler
- Spring MVC
- Spring Data JPA
- Thymeleaf
- MySQL
- Maven

---

## Features

### Scheduling
- Time-based device ON / OFF scheduling
- Per-device schedule configuration
- Enable or disable schedules dynamically
- Automatic execution using Spring Scheduler

### Automation & Policy Enforcement
- Background execution of automation rules
- Admin-defined energy usage policies
- System-wide policy enforcement
- Logging of automated actions and violations

---

## Project Structure

```
Module_5_Scheduling_and_Automation/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/role/implementation/
│   │   │       └── automation/
│   │   │           ├── controller/
│   │   │           │   └── ScheduleController.java
│   │   │           ├── service/
│   │   │           │   ├── AutomationService.java
│   │   │           │   └── AutomationServiceImpl.java
│   │   │           ├── repository/
│   │   │           │   └── ScheduleRepository.java
│   │   │           └── model/
│   │   │               └── Schedule.java
│   │   │
│   │   └── resources/
│   │       ├── templates/
│   │       │   ├── schedules.html
│   │       │   ├── automation.html
│   │       │   └── policy-enforcement-logs.html
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
CREATE DATABASE shems_automation;
```

Run application:
```
mvn spring-boot:run
```

Open in browser:
```
http://localhost:8080/schedules
```

---

## Role in System
This module bridges device management and energy tracking by automating
device behavior and enforcing admin-defined energy policies across the
entire SHEMS platform.

---

## Summary
Module 5 enables intelligent automation by combining user-defined schedules
with admin-defined energy policies. It ensures optimized, rule-based, and
hands-free device operation, making it a core control module of the system.
