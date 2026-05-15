# NTCentinel: Automated Student Violation Management System

[![SDG Goal 4: Quality Education](https://img.shields.io/badge/SDG-Goal%204-gold)](https://sdgs.un.org/goals/goal4)
[![SDG Goal 11: Sustainable Cities and Communities](https://img.shields.io/badge/SDG-Goal%2011-orange)](https://sdgs.un.org/goals/goal11)

## Project Title & SDG Goal
**Project Title:** NTCentinel  
**Primary SDG Goal:** **Goal 4: Quality Education** & **Goal 11: Sustainable Cities and Communities**

NTCentinel is a kiosk-based automated violation tracking system designed for the **National Teachers College (NTC)**. It addresses the critical issue of inefficient campus entry and manual record-keeping. By digitizing the violation logging process, the project ensures a safer learning environment (SDG 4) and reduces hazardous student congestion at school gates, contributing to safer institutional infrastructure (SDG 11).

---

## Project Description

### The Problem
The traditional manual logging system at NTC relies on physical logbooks. This leads to:
* **Manual Bottlenecks:** Processing each student takes significant time, causing long lines that spill onto public streets, posing safety risks.
* **Data Integrity Issues:** "Messy handwriting" makes it difficult for the Office of Student Affairs (OSA) to decode and encode data accurately.
* **Security Risks:** Physical logbooks containing sensitive student data are accessible to unauthorized individuals.

### The Solution: NTCentinel
NTCentinel is a digital kiosk solution that integrates hardware and software to streamline the violation process. It utilizes QR code scanning for near-instant identity verification and a touchscreen interface for security guards to log preset violations.

### Architecture Justification
The system follows a **Client-Server Architecture** optimized for Local Area Network (LAN) deployment:
* **QR Integration:** Chosen for high-speed data retrieval (decoding under 1 second), crucial for maintaining traffic flow at the gate.
* **Centralized Database (SQL):** Ensures real-time synchronization between the entry kiosk and the OSA backend, enabling the "3-Strike Rule" automated flagging system.
* **Thermal Printing Module:** Provides immediate physical evidence of the violation for the student, ensuring transparency and adherence to school policy.
* **Role-Based Access Control (RBAC):** Justified by the Data Privacy Act of 2012, ensuring only authorized OSA staff can modify student records.

---

## Key Features
* **Rapid Verification:** QR scanning reduces processing time to under 3 seconds.
* **Automated Sanctions:** System automatically calculates the number of offenses and flags repeat offenders.
* **Digital Audit Trail:** Eliminates manual encoding errors and provides OSA with real-time analytics.
* **Offline Resilience:** Capable of temporary local storage during network interruptions.

---

## Contributor
| Team Member | Primary Contribution / Assigned Module |
| :--- | :--- |
| **Gracias, Kevin Jay C.** | Project Lead, System Analysis, SRS Documentation, Database Schema Design, UI/UX Design for Kiosk, and Frontend Dashboard Development. |

---

## Technical Stack
* **Language:** (VB.NET Forms)
* **Database:** SQL-based relational database
* **Hardware:** QR Scanner, Thermal Printer, Touchscreen Kiosk
* **Network:** Local Area Network (LAN)

---
*Developed as a Semestral Project for System Analysis and Design - National Teachers College.*
