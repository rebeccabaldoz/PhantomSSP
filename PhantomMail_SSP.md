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

---

## 📦 Data Types Handled

- Report Content (text, optional file attachments)  
- Case Notes & Follow-ups  
- Timestamps & Routing Data  
- Minimal metadata (no personal identifiers logged)

---

## 🧭 Boundaries & Dependencies

- Internal network access only (no public interface)  
- Email notifications (internal only)  
- Linked to internal Active Directory for Reviewer access (no reporter login required)
