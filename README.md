# healthcare-dashboard
Healthcare Data Anonymisation & Breach Detection Dashboard

---

## Project Overview
This project aims to build a secure, user-friendly dashboard to manage healthcare data, focusing on:

- **Data Anonymisation:** Protect patient privacy by anonymising Personally Identifiable Information (PII) and Protected Health Information (PHI)

- **Security by Design:** Integrate security features throughout the system architecture to uphold the Confidentiality, Integrity, and Availability (CIA) of data

- **Breach Detection:** Monitor data access and detect potential security breaches in near real-time

---

## Features [Minimum Viable Product (MVP)]

1. **Data Anonymisation**
   - Anonymise sensitive patient data as Personally Identifiable Information (PII) and Protected Health Information (PHI) before storage or display to ensure compliance with the General Data Protection Regulation (GDPR)

2. **Breach Detection**
   - Log every access event with key details including user ID, timestamp, IP address, and action performed
   - Identify suspicious activities as access timestamp outside normal working hours or IP address from unknown locations
   - Display alerts in near real-time on the dashboard for any flagged events to enable prompt investigation

3. **Security by Design**
   - Implement Identity and Access Management (IAM) with Role-Based Access Control (RBAC) - e.g., administrator, clinician, auditor
   - Enforce strong password authentication with secure password policies to ensure only authorised users can access the system
   - Encrypt data at rest and during transmission using AES-256 encryption and TLS protocols to protect confidentiality and integrity

---

## Scope

- **Data Anonymisation**
  - Automatic anonymisation of PII and PHI
  - Basic GDPR compliance

- **Role-Based Access Control**
  - Four predefined roles:
    - Clinician
    - Administrator
    - Auditor
    - Super Admin
  - Authentication with secure password policies

- **Breach Detection & Logging**
  - Logging of data access events
  - Detection and flagging of suspicious activities

- **Encryption**
  - AES-256 encryption at rest
  - TLS encryption in transit

- **Dashboard Interface**
   - Basic React dashboard displaying anonymised data and alerts updated in near real-time

---

## User Roles
The system defines the following user roles, each with specific permissions:

- **Clinician**: Accesses anonymised patient data to support clinical decisions
- **Administrator**: Monitors system activity, manages user accounts, and configures breach detection rules
- **Auditor**: Reviews logs and generates compliance reports
- **Super Admin**: Manages system-wide security policies, roles, and oversees system health
- **All Users**: General users who must authenticate securely and manage their own credentials

For detailed role descriptions, see [User Roles & Definitions](docs/user-roles.md).

---

## User Stories
User stories outline the functional needs of each role to guide development:

- Clinicians need to view anonymised data and receive alerts
- Administrators monitor logs and manage users
- Auditors review historical logs for compliance
- Super Admins configure security policies and manage roles
- All users require secure authentication and password management

For detailed user stories, see [User Stories](docs/user-stories.md)
