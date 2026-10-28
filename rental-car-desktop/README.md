# BELHAJ Luxury Rent Car — Java Desktop Rental Management Application

A desktop application to manage a car rental agency: **clients, vehicles, contracts and invoicing**, with role-based access and **PDF invoice export**.

> Academic project — Java API module, ENSA Fez, April–May 2025.

![Java](https://img.shields.io/badge/Java-SE%2022-orange) ![Swing](https://img.shields.io/badge/UI-Swing-blue) ![Maven](https://img.shields.io/badge/Build-Maven-C71A36) ![JDBC](https://img.shields.io/badge/JDBC-UCanAccess-grey) ![iText](https://img.shields.io/badge/PDF-iText-green)

---

## Features

| Module | What it does |
|---|---|
| **Login** | Authentication against the database, Admin / non-Admin roles |
| **Dashboard** | Statistics (clients, vehicles, contracts) and side navigation |
| **Clients** | Add, edit, search and view clients |
| **Vehicles** | Manage the fleet, search vehicles, filter available ones |
| **Contracts** | Create and list rental contracts |
| **Invoicing** | Automatic amount calculation and **PDF invoice export** (iText) |

## Design

- **Data model:** MCD and relational database with five tables — `Categories`, `Clients`, `Vehicules`, `Contrats`, `Factures` — linked by foreign keys.
- **UML:** class diagram, object diagram and sequence diagram (login and rental flow), modelled with Astah.
- **Code structure:** one Swing window per module (`LoginWindow`, `MainApplicationWindow`, `ClientsWindow`, `VehiculesWindow`, `ContratsWindow`, `FacturationWindow`), a static `DBConnection` utility for JDBC access, and an `AppController` separating UI from business logic.

## Tech stack

Java SE 22 · Swing · JDBC (UCanAccess) · Microsoft Access · iTextPDF · Maven · Git · Eclipse · UML (Astah)

## Lessons learned and next steps

The project review identified concrete improvements, which I would apply in a new version:

- hash passwords instead of storing them in plain text;
- move from MS Access to a server database (MySQL / PostgreSQL);
- strengthen input validation and error handling in the database layer;
- add backups and accessibility support (labels, keyboard shortcuts).

---

**Author:** Khaoula Belhaj — final-year engineering student, Communicating Systems & Computer Security, ENSA Fez · [LinkedIn](https://linkedin.com/in/khaoula-belhaj-1999163a6)
