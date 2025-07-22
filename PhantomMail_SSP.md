# System Security Plan (SSP): Phantom Mail

**System Name:** Phantom Mail  
**System Type:** Internal Whistleblower Reporting Platform  
**Author:** Rebecca Baldoz  
**Status:** In Progress  

---

## 📄 System Overview

Phantom Mail is a secure internal reporting platform for employees to submit anonymous concerns related to ethics, fraud, harassment, safety, or abuse.  
It is designed to protect the anonymity of reporters while ensuring proper routing and tracking by authorized personnel in HR, Legal, or Compliance roles.

The system is web-based, internally hosted, and includes:
- Encryption in transit and at rest
- Role-based access control (RBAC)
- Limited metadata retention
- Logging of administrative actions
- Escalation workflows for review and tracking

## 📦 Data Types Handled

- Report Content (text, optional file attachments)  
- Case Notes & Follow-ups  
- Timestamps & Routing Data  
- Minimal metadata (no personal identifiers logged)


## 🧭 Boundaries & Dependencies

- Internal network access only (no public interface)  
- Email notifications (internal only)  
- Linked to internal Active Directory for Reviewer access (no reporter login required)

  ## 🔐 NIST 800-53 Control Implementation

### **AC-2: Account Management**

Phantom Mail implements strict account management practices for non-anonymous users (HR, Legal, Admin roles):

- All account creation requires managerial approval and is provisioned through Active Directory (AD).
- Roles are limited to Reviewer (read/report) and Administrator (manage platform settings, view audit logs).
- Access for terminated employees is automatically disabled via AD sync within 24 hours.
- Reviewer accounts are audited quarterly to ensure continued need and appropriate access levels.
- Anonymous users (employees submitting reports) do not require accounts and cannot access platform content.

Phantom Mail uses **Role-Based Access Control (RBAC)** to ensure users are granted access only to the functions required by their job responsibilities.  
This is implemented in accordance with the principle of **Least Privilege**.

**Control Type:** Technical / Operational  
**Control Baseline:** Moderate  
**Implemented:** Yes  
**Responsible Party:** System Administrator, Compliance Officer

Added RBAC control details

 
- Email notifications (internal only)  
- Linked to internal Active Directory for Reviewer access (no reporter login required)
