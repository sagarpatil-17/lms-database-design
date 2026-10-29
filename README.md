# LMS Database Design

A relational database schema for a **Learning Management System (LMS)** using **MySQL** and **Prisma ORM**.

---

## 🛠️ Tech Stack & Features

* **Tech Stack:** MySQL and Prisma ORM.
* **Core Models:** Supports user roles (STUDENT, INSTRUCTOR, ADMIN), multi-layered course organization, enrollments, and granular progress tracking.

---

## 📐 Entity-Relationship (ER) Diagram

🔗 **[View Interactive Live ER Diagram on DrawDB](https://www.drawdb.app/share/eRdmeFpRsjsAdlaxRvxqsuX9)**

---

## 🚀 Getting Started

1. **Clone & Install:**
   ```bash
   git clone https://github.com
   cd lms-database-design
   npm install
   ```
  

2. **Configure & Migrate:** Set up your `.env` file with `DATABASE_URL`, then run:
   ```bash
   npx prisma generate
   npx prisma migrate dev --name init
   ```
  
