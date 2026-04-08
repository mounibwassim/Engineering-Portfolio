<p align="center">
  <img src="logo.png" width="200" alt="RestoSmart AI Logo">
</p>

# 🍽️ RestoSmart AI - Advanced Customer Support Automation

RestoSmart AI is a **next-generation, multilingual feedback management system** designed for high-performance restaurants. It automates feedback collection, analyzes sentiment using AI, secures data with a robust **JWT-based RBAC (Role-Based Access Control)** system, and provides actionable insights via a premium real-time dashboard.

## Demo & Live Preview

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open-green?style=for-the-badge)](https://resto-ai-analytics.vercel.app)
[![Watch Demo](https://img.shields.io/badge/YouTube-Watch-red?style=for-the-badge&logo=youtube)](https://youtu.be/Sq8YaBC-GmQ?si=6dJMRNa8TW7lxvCh)

---

## ✨ Premium Features

### 🧠 1. Global Multilingual AI Logic
*   **Universal Translator**: Automatically detects languages (French, Spanish, Arabic, Malay, etc.) and analyzes them in English while preserving original text.
*   **Sentiment Analysis**: Classifies feedback as *Positive* or *Negative* instantly.
*   **Smart Actionable Insights**: 
    *   *“Pizza was cold”* → **Action: Check Pizza Station**
    *   *“Waiter was rude”* → **Action: Review Staff Training**
    *   *“Too noisy”* → **Action: Check Music & Ambiance**

### 🛡️ 2. Secure JWT Authentication & RBAC
*   **JWT Protected APIs**: All sensitive data endpoints (Stats, Feedback, Employees) are secured with signed JSON Web Tokens.
*   **Role-Based Access Control (RBAC)**: 
    *   **Manager (Admin)**: Full control. Can manage employees, reset passwords, and wipe data.
    *   **Employee**: Restricted to Overview and History. Access to Settings/Team Management is blocked by a dedicated **Access Denied** guard.
*   **Global Auth Interceptor**: Frontend automatically handles secure sessions.
*   **Master Key Recovery**: Secure password recovery system for authorized personnel.

### 📊 3. Executive Dashboard Suite
*   **Weekly & Yearly Charts**: Track volume trends effortlessly.
*   **Hourly Heatmap**: Identify peak feedback times (e.g., *7:00 PM - 9:00 PM*).
*   **Category Distribution**: See exactly where issues lie (*40% Food Quality, 20% Service*).
*   **NPS Score**: Real-time Net Promoter Score calculation.
*   **Critical Issues Widget**: Auto-highlights "Urgent" 1-star reviews.

### 📝 4. Modern Feedback Collection
*   **Public Portal**: Mobile-responsive, beautiful dark-mode form for customers.
*   **QR Code Integration**: One-click generation in Settings.
*   **Live Inbox**: Real-time feed of incoming messages with "Unread" badges.

### 📅 5. Smart History & Calendar
*   **Red Dot Indicators**: Calendar heatmap showing days with feedback activity.
*   **Search & Filter**: Find specific reviews by keyword (*e.g., "salty"*) or category.

---

## 🛠️ Technology Stack

**Frontend**
*   **React (Vite)**: Ultra-fast SPAs.
*   **Tailwind CSS**: Modern utility-first styling.
*   **Framer Motion**: Premium animations (Fade-ins, Slide-ups).
*   **Recharts**: High-performance data visualization.
*   **Lucide React**: Crisp, vector-based iconography.

**Backend**
*   **Python (FastAPI)**: Async, high-concurrency API.
*   **Pandas & Scikit-Learn**: Data processing & AI modeling.
*   **Deep Translator**: Google Translate integration.
*   **Pydantic**: Robust data validation and serialization.

---

## 🚀 Getting Started

### 1. Backend Setup
```bash
# Create virtual environment
python -m venv .venv
.venv\Scripts\activate  # Windows

# Install dependencies
pip install -r backend/requirements.txt

# Run Server
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

### 2. Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### 3. First-Time Initialization
1.  Open the App.
2.  You will see the **System Setup Screen** (only appears once).
3.  Create your **Root Admin** account (Username/Password).
4.  *Note: Manager Email is optional and defaults to internal system.*

---

## 📖 Manager Guide

### How to Reset Staff Passwords?
1.  Login as **Manager**.
2.  Go to **Settings**.
3.  Scroll to **Team Management**.
4.  Click the 🔑 icon next to the user.
5.  Type the new password and click **Overwrite**.

### How to Delete Bad Data?
1.  Login as **Manager**.
2.  Go to **Settings** or **History**.
3.  Click the 🗑️ icon.
4.  *Note: Only the Manager account can perform this action.*

### How to Use the Master Key?
If you (The Manager) get locked out:
1.  Use the **Console Recovery** mechanism (if enabled in Dev Mode).
2.  Or check `admin_config.json` on the server manually.

---

## 📄 License
**Private Enterprise Software**. Unauthorized distribution is prohibited.
