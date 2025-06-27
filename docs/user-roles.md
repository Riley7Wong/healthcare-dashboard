# User Roles & Definitions

The system defines four key user roles with distinct responsibilities and access levels:

### Clinician
- Frontline healthcare professional using the dashboard to view patient records
- Can view anonymised data only
- No access to system settings, logs, or user management

### Administrator
- Oversees daily system operations
- Can monitor real-time alerts, view access logs, and manage users
- Cannot change encryption or security configurations

### Auditor
- Read-only role for compliance and security auditing purposes
- Can access and export full access logs and reports
- Cannot change any data or system settings

### Super Admin (System Owner)
- Full system privileges
- Responsible for defining and enforcing security policies (RBAC, encryption, password rules)
- Can manage all roles, permissions, and configurations

### All Roles (Non-patient)
- All users must authenticate via secure login
- All roles are subject to role-based access controls
