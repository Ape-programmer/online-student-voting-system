# Online Student Voting System — BSc Final Year Project

A database-backed web application developed as a **BSc Computer Science final-year project** to support student election administration and online voting.

The system demonstrates full-stack web-development fundamentals including authentication, session-based access, relational database integration, candidate and voter management, ballot submission and election reporting.

## Core Functionality

- student/voter registration and authentication;
- administrator authentication and dashboard;
- voter and user management;
- candidate management;
- election/position management;
- ballot interface covering multiple student-union positions;
- one-vote workflow and voter-status tracking;
- election result/reporting functionality.

## Technology Stack

**PHP • MySQL • HTML • CSS • JavaScript • jQuery • Bootstrap • Apache**

## System Workflow

```text
Voter Registration
        ↓
Authentication
        ↓
Eligibility / Voting Status
        ↓
Candidate & Position Selection
        ↓
Ballot Confirmation
        ↓
Vote Storage
        ↓
Voter Status Updated
        ↓
Election Reporting
```

Administrators use a separate management interface for election configuration, users/voters, candidates and reports.

## Repository Structure

```text
online-student-voting-system/
├── README.md
├── SECURITY.md
├── PROJECT_INVENTORY.md
├── .env.example
├── .gitignore
├── database/
│   └── schema.sql
└── src/
    └── application source code
```

## Running Locally

This is a portfolio edition of a legacy academic PHP/MySQL application.

1. Install a local Apache/PHP/MySQL environment such as XAMPP or an equivalent stack.
2. Create a MySQL database.
3. Import `database/schema.sql`.
4. Review the application's database connection files under `src/` and configure them for your local environment.
5. Serve `src/` through Apache.

> The application source is included to demonstrate the project architecture and implementation. Review `SECURITY.md` before attempting any deployment.

## Security & Modernisation

The original project contains legacy security practices that would need improvement before production use. These are documented transparently in [`SECURITY.md`](SECURITY.md), including password hashing, prepared statements, CSRF protection, configuration management and server-side validation.

This demonstrates both the original undergraduate implementation and the stronger security and engineering understanding developed since completing the project.

## Portfolio Context

This project complements my later MSc Artificial Intelligence & Data Science work by showing my earlier foundation in:

- web application development;
- relational databases;
- authentication and sessions;
- CRUD workflows;
- system analysis and design;
- integrating front-end and back-end components.

## Future Improvements

A modern rebuild would include prepared statements/ORM-based database access, `password_hash()` authentication, CSRF protection, role-based authorisation, secure environment configuration, stronger ballot-integrity constraints, automated tests, audit logs, responsive UI improvements and containerised deployment.

## Acknowledgements

This project was developed as part of my BSc Computer Science final-year work. Some interface/template components were adapted from existing educational resources, with original attribution retained within the relevant source files.

## Author

**Abiola Peace Emmanuel**  
BSc Computer Science — Final Year Project  
GitHub: **Ape-programmer**
