# 🔐 Authyx: Enterprise Identity & Access Management (IAM) Showcase

![Authyx Logo](https://authyx.vercel.app/app-logo.png)

Authyx is a professional-grade authentication and identity system built using **Modern Component Architecture**. It demonstrates how to leverage industry-standard UI frameworks while architecting a secure, custom-built "Engine" for data and logic.

## Demo & Live Preview

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open-green?style=for-the-badge)](https://authyx.vercel.app)
[![Watch Demo](https://img.shields.io/badge/YouTube-Watch-red?style=for-the-badge&logo=youtube)](https://youtu.be/LByF6lxyZH8)

---

## 🏠 System Architecture: The "Custom Home" Analogy

Building Authyx is like building a **high-end custom home**. 
- **The Design**: We didn't hand-carve every brick; instead, we used the highest quality professional materials (**Launch UI + Shadcn/UI**) to ensure an "Apple-level" premium finish.
- **The Engine**: Inside that beautiful exterior sits a custom-engineered "Heart"—a secure authentication and database system built from scratch to handle real-world enterprise requirements.

### 1. The Design Layer (Launch UI + Shadcn/UI)
For the visual foundation, Authyx utilizes **Launch UI**, a premium collection of components built on top of **Shadcn/UI**. 
*   **Why?** In production environments, engineers use industry-standard component libraries to ensure accessibility, responsiveness, and professional aesthetics, allowing them to focus 100% on security and business logic.

### 2. The Technical Engine (Custom Implementation)
While the look is polished by Launch UI, the functionality is a custom implementation:
*   **Authentication (The Brain)**: NextAuth.js handles secure OAuth handshakes with Google and GitHub.
*   **Database (The Memory)**: Prisma ORM connected to a Supabase PostgreSQL cluster manages persistence and session data.
*   **Security (The Shield)**: A custom-built Middleware layer protects sensitive routes, enforcing strict role-based access.

---

## 🚀 Key Features

- ✅ **OAuth 2.0 Integration**: Secure login with Google and GitHub via NextAuth.
- ✅ **Stateless Session Management**: Hardened JWT-based authentication.
- ✅ **Enterprise Database**: PostgreSQL hosted on Supabase, architected with Prisma.
- ✅ **Route Protection**: Custom Middleware for secure `/dashboard` access.
- ✅ **Professional Branding**: Complete branding purge of legacy assets for a clean, unique identity.
- ✅ **Modern UI**: Built with Next.js 15, Tailwind CSS, and Framer Motion.

---

## 🔧 Getting Started (Local Development)

### 1. Clone the Repository
```bash
git clone https://github.com/mounib-s/Authyx.git
cd Authyx
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment Variables
Create a `.env.local` file with your credentials:
```env
DATABASE_URL=postgresql://user:password@host:port/dbname
DIRECT_URL=...
NEXTAUTH_SECRET=...
NEXTAUTH_URL=http://localhost:3000
GITHUB_ID=...
GITHUB_SECRET=...
GOOGLE_CLIENT_ID=...
GOOGLE_CLIENT_SECRET=...
```

### 4. Prepare the Database
```bash
npx prisma generate
npx prisma db push
```

### 5. Start the Engine
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) to view your site.

---

## 📁 Project Structure

```text
/src/app                → Next.js 15 App Router
/src/components         → Shared UI Components (Launch UI)
/src/features           → Custom logic (Auth, Dashboard)
/src/lib                → Core Utilities (Auth, Prisma)
/prisma                 → Database Schema
/public                 → Branding & Static Assets
```

---

## 🔐 Security & Deployment

- **Infrastructure**: Optimized for serverless stability on **Vercel**.
- **Data Safety**: All secret tokens are handled via environment variables and never exposed to the client.
- **Cleanup**: The system has been fully decoupled from its original template branding for maximum professionalism.

---

## 📜 License
MIT

---
*Built with precision to showcase the balance between modern design and secure engineering.*
