# Smart School Management System

A desktop application to automate and modernize everyday school administration, developed with C# (WinForms, OOP) and SQL Server. The system provides modules for managing students, attendance, fees, academic results, and integrates role-based authentication for Admins, Teachers, and Accountants.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [System Architecture](#system-architecture)
- [Database Design](#database-design)
- [How to Run](#how-to-run)
- [Project Organization](#project-organization)
- [Contributing](#contributing)
- [Planned Enhancements](#planned-enhancements)
- [Contact](#contact)

---

## Project Overview

Smart School Management System (SSMS) is a Windows Forms application designed for schools to digitize their academic and administrative work. Built using C#'s OOP features and a normalized SQL Server database, it automates:

- Student management and admissions
- Attendance tracking
- Fee collection and reporting
- Academic records and mark sheets
- Secure, role-based user access

The system demonstrates use of core OOP principles (encapsulation, inheritance, abstraction, polymorphism) in a real project.

---

## Features

### Admin
- Manage students, classes, users
- Dashboard & analytics
- Database backup/restore
- Generate system-wide and financial reports

### Teacher
- View and manage assigned classes/students
- Mark daily attendance
- Enter grades, generate report cards

### Accountant
- Manage student fees/payments
- Track unpaid fees
- Generate and print fee receipts/reports

### All Roles
- Secure login
- Notification system

---

## Technology Stack

| Component     | Technology                      |
| ------------- | ------------------------------- |
| Frontend      | Windows Forms (C#)              |
| Logic Layer   | C# (OOP, .NET Framework)        |
| Database      | SQL Server / SQL Express        |
| Reporting     | Crystal Reports / iTextSharp    |
| IDE           | Visual Studio                   |

---

## System Architecture

The solution uses a layered architecture:

- **Presentation Layer:** WinForms UI/forms and user interaction
- **Business Logic Layer (BLL):** Centralizes validation, calculations, and core logic
- **Data Access Layer (DAL):** Handles CRUD operations with SQL Server, using parameterized queries for security

This structure promotes modular code, easy debugging, scalability for new features, and maintainability.

---

## Database Design

- Fully normalized (3NF) relational design
- Primary and foreign keys enforce data integrity
- Core tables: Users, Students, Classes, Subjects, Attendance, Fees, Marks, Notifications

A sample database script is included:  
`/Database/SmartSchoolDB.sql`

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/SmartSchoolManagementSystem.git
   ```

2. **Open in Visual Studio**  
   Open the `.sln` solution file.

3. **Restore NuGet packages**  
   Required for reporting libraries (Crystal Reports/iTextSharp).

4. **Configure Database Connection**
   - Create a SQL Server database using the provided script.
   - Update the connection string in the application config:  
     `App.config` or `Settings.cs`

5. **Build & Run**
   - Debug or run the project directly from Visual Studio.

---

## Project Organization

| Folder/File              | Description                         |
|--------------------------|-------------------------------------|
| `/Presentation`          | WinForms UI forms                   |
| `/BLL`                   | Business logic classes              |
| `/DAL`                   | Data Access Layer classes           |
| `/Models`                | All core entity (POCO) classes      |
| `/Reports`               | Crystal Reports / PDF templates     |
| `/Database/SmartSchoolDB.sql` | Database schema and sample data |
| `README.md`              | Project information                 |
| `docs/`                  | Diagrams, documentation, walkthroughs|

---

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes
4. Push and open a PR with description

---

## Planned Enhancements

- SMS and email alerts
- Parent/guardian portal
- Teacher payroll management
- Timetable scheduling
- Web/mobile client
- Cloud backup/sync

---

## Contact

**Author:** Hussain Hakimi  


---
