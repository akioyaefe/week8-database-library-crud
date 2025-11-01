# 📚 Week 8 Database: Library Management CRUD System

This project is a simple **Library Management System** built as part of the **Power Learn Project (PLP) Week 8 Database Design & Programming with SQL** assignment.

It demonstrates how to design a **relational database** in **MySQL** and implement full **CRUD (Create, Read, Update, Delete)** operations using **Node.js (Express)**.

---

## 🎯 **Project Overview**

The **Library Management System** allows users to:
- Add new books and members
- View all books and members
- Update book or member information
- Delete records as needed

The database is fully normalized and includes **primary keys**, **foreign keys**, and **relationships** between tables.

---

## 🧱 **Database Design**

### Database Name:
`library_management`

### Tables:
1. **Books**
   - `book_id` (Primary Key)
   - `title`
   - `author`
   - `genre`
   - `year_published`
   - `available_copies`

2. **Members**
   - `member_id` (Primary Key)
   - `name`
   - `email`
   - `phone`
   - `join_date`

3. **BorrowRecords**
   - `borrow_id` (Primary Key)
   - `book_id` (Foreign Key → Books)
   - `member_id` (Foreign Key → Members)
   - `borrow_date`
   - `return_date`

Each relationship is properly constrained to ensure **referential integrity**.

---

## ⚙️ **Technologies Used**
- **MySQL** — Relational database
- **Node.js (Express)** — Backend framework
- **Postman** — API testing tool
- **GitHub** — Version control & submission

---

## 🚀 **Setup Instructions**

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/week8-database-library-crud.git
cd week8-database-library-crud
