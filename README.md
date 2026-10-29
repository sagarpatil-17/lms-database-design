# LMS Database Design

A robust, relational database schema for a **Learning Management System (LMS)** designed with **MySQL** and managed via **Prisma ORM**. 

This repository contains the data models, entity relationships, and database configurations required to power a modern online learning platform, featuring robust tracking for users, courses, enrollments, lessons, and progress.

---

## 🛠️ Tech Stack

* **Database:** [MySQL](https://mysql.com) (Relational database for structured, ACID-compliant data management)
* **ORM:** [Prisma](https://prisma.io) (Next-generation Node.js and TypeScript ORM for type-safe database queries and migrations)

---

## 📐 Core Data Model Features

The schema is architected to handle the essential operations of an LMS ecosystem:

* **User Management:** Flexible role-based infrastructure supporting `STUDENT`, `INSTRUCTOR`, and `ADMIN`.
* **Course Architecture:** Multi-layered course organization containing modules, lessons, and multimedia attachments.
* **Enrollment Tracking:** Explicit many-to-many relationship mapping between students and courses with active status flags.
* **Progress Logging:** Granular completion tracking per lesson to monitor student advancement.

---

## 🚀 Getting Started

### Prerequisites

* [Node.js](https://nodejs.org) (v18.0.0 or higher)
* [MySQL Server](https://mysql.com) running locally or hosted in the cloud.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd lms-database-design
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory and add your MySQL connection string:
   ```env
   DATABASE_URL="mysql://USER:PASSWORD@HOST:PORT/DATABASE_NAME"
   ```

4. **Initialize Prisma & Generate Client:**
   ```bash
   npx prisma generate
   ```

5. **Push Schema to MySQL (Run Initial Migration):**
   ```bash
   npx prisma migrate dev --name init
   ```

---

## 📂 Project Structure

```text
├── prisma/
│   ├── schema.prisma       # Core database schema definitions (Models & Relations)
│   └── migrations/         # Auto-generated SQL migration history files
├── .env                    # Local environment variables (git-ignored)
├── .gitignore              # Standard Git exclusion file
├── package.json            # Node.js project configuration and scripts
└── README.md               # Project documentation
```
