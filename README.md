# 🏢 Salesforce Lease Management System

A **Salesforce-based cloud application** designed to automate the **property lease management process** — including **property creation**, **tenant registration**, **lease tracking**, **payment management**, and **approval workflows** — using Salesforce’s declarative and programmatic tools.

---

## 🚀 Project Overview

The **Lease Management System** allows admins to:
- Create and manage property and tenant records  
- Automate rent payment confirmations  
- Manage lease periods with date validation  
- Approve or reject tenant leave requests  
- Send monthly rent reminders automatically  

All of this is achieved using **Salesforce Flows**, **Approval Processes**, **Apex Triggers**, and **Apex Scheduler** for complete process automation.

---

## 🧩 Features

| Feature | Description |
|----------|-------------|
| 🏠 **Property Management** | Manage property details such as location, rent, and type |
| 👤 **Tenant Management** | Add and manage tenants with email, phone, and property lookup |
| 📄 **Lease Management** | Store lease duration and validate date consistency |
| 💰 **Payment Tracking** | Update payment status and send automatic confirmation emails |
| 📧 **Email Automation** | Predefined templates for approvals, payments, and reminders |
| ⏰ **Apex Scheduler** | Sends monthly rent reminders automatically |
| ✅ **Approval Process** | Handles tenant leave approval and rejection with email alerts |
| 🔒 **Validation Rules** | Prevents invalid data like incorrect lease dates |
| ⚙️ **Apex Trigger** | Ensures only one tenant can occupy a property |

---

## ⚙️ System Architecture

### 🔹 Workflow Overview

```mermaid
flowchart TD
    A[Admin] --> B[Property Object]
    B --> C[Tenant Object]
    C --> D[Lease Object]
    D --> E[Payment Object]
    E --> F[Flow]
    F --> G[Email Template]
    G --> H[Tenant Email Inbox]
    F --> I[Approval Process]
    I --> J[Admin Approval]
    J --> K[Apex Scheduler]
    K --> L[Monthly Rent Reminder]
