# Database Design

## Database Engine

PostgreSQL (Supabase)

---

## Security

- Row Level Security (RLS): Enabled
- Authentication: Supabase Auth
- JWT Authentication
- Encrypted Connections (HTTPS)
- Daily Backups

---

## Main Schemas

app

public

auth

storage

---

## Main Tables

### users

Stores platform users.

### roles

Stores user roles.

### permissions

Stores permissions.

### user_roles

Links users to roles.

### projects

Engineering projects.

### contracts

Contracts and agreements.

### road_studies

Road study projects.

### technical_reports

Technical reports.

### documents

Uploaded files.

### audit_logs

Security and activity logs.

---

## Relationships

users
    │
    ├── user_roles
    │
roles
    │
    └── permissions

projects
    ├── contracts
    ├── road_studies
    ├── technical_reports
    └── documents

---

## Security Rules

- Least Privilege Principle
- Role-Based Access Control (RBAC)
- Row Level Security
- Audit Logging
- Secure Storage
