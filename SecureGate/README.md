# 🛡️ SecureGate Enterprise
### Advanced User Management & Role-Based Access Control System

![SecureGate Banner](./assests/img/banner.png)

SecureGate is a high-performance, enterprise-grade User Management System engineered with **CodeIgniter**. Designed for scalability and security, it provides a centralized gateway for managing authentication, user lifecycles, and administrative oversight with a premium, modern SaaS aesthetic.

## Demo & Live Preview

[![Watch Demo](https://img.shields.io/badge/YouTube-Watch-red?style=for-the-badge&logo=youtube)](https://youtu.be/Iu7IFzhikZU)

---

## 💎 Core Value Propositions

*   **⚡ Modern UX/UI**: Powered by a refined glassmorphism design system for both User and Administrative portals.
*   **🔐 Unified Security**: Robust role-based access control (RBAC) ensuring data integrity and restricted access.
*   **📊 Live Analytics**: Real-time data visualization of system performance and user registration trends.
*   **👤 Self-Service Portal**: Comprehensive profile management, including secure credential updates and data oversight.
*   **🛠️ Administrative Power**: Full-cycle user management, status toggling, and system-wide monitoring.

---

## 🚀 Quick Start Guide

### 1. Prerequisites
- **Server Environment**: XAMPP / WAMP / MAMP (PHP 7.4+ recommended).
- **Database**: MySQL / MariaDB.
- **Portals**:
    - **Main Application**: `http://localhost/SecureGate/`
    - **Admin Control**: `http://localhost/SecureGate/admin/login`

### 2. Standard Installation
1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/mounibwassim/SecureGate.git
    ```
2.  **Server Placement**: Deploy the project to your server's root directory (e.g., `xampp/htdocs/SecureGate`).
3.  **Database Migration**:
    - Access [phpMyAdmin](http://localhost/phpmyadmin).
    - Create a database named `securegate`.
    - Import the `/Sql File/securegate.sql` schema.
4.  **Automatic Synchronization**: Ensure the folder name remains `SecureGate` to maintain internal routing integrity.

---

## 🔐 Credentials for Verification

### 🏢 Administration Portal
- **Username**: `admin`
- **Password**: `Test@12345`
- *Alternate*: `tigeradmin@mmu` / `tigeradmin`

### 👤 User Portal (Sample Account)
- **Username**: `tiger@mmu`
- **Password**: `tigerstudent`

---

## 🛠️ Technical Architecture

| Component | Technology |
| :--- | :--- |
| **Logic Layer** | PHP 7.x (CodeIgniter Framework) |
| **Data Layer** | MySQL 5.7+ |
| **Presentation** | Bootstrap 5, FontAwesome 6, Chart.js, jQuery |
| **Security** | Session-level guards, CSRF Protection, Password Hashing |
| **UI Kit** | Custom Glassmorphism Theme (Dark/Fluid) |

---

## 📈 System Roadmap
- [x] **Phase 1**: Core Engine & Authentication
- [x] **Phase 2**: Admin Analytics & User Management
- [x] **Phase 3**: Premium UI/UX Polish & Flash Message Guard
- [ ] **Phase 4**: Multi-Tenant Architecture Support
- [ ] **Phase 5**: API v1 Implementation (JSON REST)

---
Developed with precision for secure enterprise environments.
