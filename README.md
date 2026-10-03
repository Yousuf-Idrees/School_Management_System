# School Management System

The **School Management System** is a web-based platform engineered to automate core educational operations and daily school administration. The system replaces paper-based tools (such as physical attendance registers, manual gradebooks, and notice boards) with a synchronized digital environment.

## Table of Contents
- [Key Features](#key-features)
- [User Roles & Permissions](#user-roles--permissions)
- [System Architecture & Design](#system-architecture--design)
- [Functional Requirements & Use Cases](#functional-requirements--use-cases)
- [Scope & Limitations](#scope--limitations)
- [Repository & Source Code](#repository--source-code)

---

## Key Features

* **User Authentication & Role Management:** Secure login and profile handling customized for different administrative level access.
* **Student & Teacher Information Management:** Maintain digital profiles, records, and assignments for students and faculty.
* **Attendance Tracking:** Real-time, batch attendance logging with instant reporting and cumulative status tracking.
* **Grade Entry & Calculation:** Dynamic input for grades, automatic GPA and weighted average calculations, and result publishing.
* **Study Materials Management:** Seamless upload and download of course resources, syllabus materials, and assignments.
* **Class & Room Scheduling:** Automated schedule publication with conflict detection and room assignment checking.
* **Announcements & Notifications:** School-wide and class-specific messaging system for events, reminders, and news.
* **Automated Reporting & Backups:** Multi-module data aggregation to export printable PDF reports and schedule system database backups.

---

## User Roles & Permissions

| Role | Access Level & Key Responsibilities |
| :--- | :--- |
| **Admin** | Full system control: manages user accounts, configures settings, manages schedules, generates system-wide reports, and triggers backups. |
| **Teacher** | Class management: records attendance, enters and updates grades, posts class announcements, and uploads study materials. |
| **Student** | Academic access: views personal grades, attendance logs, class schedules, announcements, and downloads course materials. |
| **Parent** | Monitoring access: views child performance, attendance history, grade reports, and school notifications. |

---

## System Architecture & Design

### Domain Entities
The core domain model is structured around the following primary entities:
* `UserAccount` (Base user entity)
* `Admin`, `Teacher`, `Student`, `Parent` (Role-specific entities)
* `Class`, `Subject`
* `AttendanceRecord`, `GradeRecord`
* `Report`, `Announcement`, `BackupData`

### Requirements Elicitation Strategy
The project requirements were established through multi-source research methods:
1. **Semi-Structured Interviews:** Feedback gathered directly from administrators, teachers, and students.
2. **Questionnaires:** Structured surveys to determine user interface preferences and prioritize functional features.
3. **Document Analysis:** Audit of existing paper attendance logs, manual schedules, and grade books.
4. **Observation:** Field observations of administrative daily workflows.
5. **Prototyping:** Wireframe iterations and interactive screen mockups for UI/UX validation.

---

## Functional Requirements & Use Cases

### Complexity Breakdown

* **Simple Use Cases:**
  * View Grades
  * View Attendance
  * View / Manage Announcements
  * Manage User Accounts
* **Moderate Use Cases:**
  * Add / Edit Student Information
  * Record Class Attendance (Batch processing)
  * Upload & Download Study Materials
* **Complex Use Cases:**
  * Assign Teachers to Classes (With conflict and room availability checks)
  * Publish System-Wide Schedules
  * Enter & Update Grades (With automated GPA and weighted calculations)
  * Generate Comprehensive Reports (Multi-module PDF export)

---

## Scope & Limitations

### In Scope
* Web-based access optimized for desktop, laptop, and tablet web browsers.
* Real-time access requiring an active internet connection.
* Comprehensive administration, academic tracking, and parent portal features.

### Out of Scope (Future Scope)
* Native mobile application (iOS / Android) development.
* Integrated fee collection and payment gateway processing.

---
