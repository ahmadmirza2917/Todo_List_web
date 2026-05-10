# 📝 Laravel To-Do List Management System

<div align="center">

![Laravel](https://img.shields.io/badge/Laravel-11.x-red?style=for-the-badge&logo=laravel)
![PHP](https://img.shields.io/badge/PHP-8.x-blue?style=for-the-badge&logo=php)
![MySQL](https://img.shields.io/badge/MySQL-Database-orange?style=for-the-badge&logo=mysql)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.x-purple?style=for-the-badge&logo=bootstrap)
![License](https://img.shields.io/badge/License-Educational-green?style=for-the-badge)

### CSC336 — Web Technologies Assignment # 03
### COMSATS University Islamabad, Vehari Campus

</div>

---

# 📌 Project Overview

The **Laravel To-Do List Management System** is a complete web-based task management application developed using the **Laravel PHP Framework** following the **MVC (Model–View–Controller)** architecture.

The system allows users to:

- Create tasks
- Update tasks
- Delete tasks
- Track task status
- Manage task priorities
- Filter tasks
- View dashboard statistics

This project demonstrates practical implementation of Laravel routing, controllers, Eloquent ORM, Blade templating, form validation, and Bootstrap-based UI development.

---

# 🎯 Project Objectives

| Objective ID | Description |
|--------------|-------------|
| PO-1 | Implement complete CRUD functionality using Laravel MVC architecture |
| PO-2 | Add task priority, due dates, filtering, and statistics dashboard |
| PO-3 | Follow clean coding standards and RESTful routing conventions |
| PO-4 | Develop a responsive and user-friendly interface using Bootstrap |

---

# ✨ Features

| Feature | Description |
|---------|-------------|
| ✅ Create Tasks | Add new tasks with title, description, due date, and priority |
| ✅ Read Tasks | Display all tasks in a structured dashboard |
| ✅ Update Tasks | Modify existing task details |
| ✅ Delete Tasks | Remove tasks with confirmation dialog |
| ✅ Priority Management | Low, Medium, High priority levels |
| ✅ Status Tracking | Pending / Completed task states |
| ✅ Status Toggle | One-click task completion toggle |
| ✅ Filtering | Filter tasks by priority and status |
| ✅ Statistics Dashboard | Real-time task statistics |
| ✅ Validation | Server-side form validation |
| ✅ Flash Messages | Success and error notifications |
| ✅ Responsive UI | Mobile-friendly Bootstrap interface |

---

# 🛠️ Technologies Used

| Technology | Version | Purpose |
|------------|----------|---------|
| Laravel | 11.x | PHP Web Framework |
| PHP | 8.x | Backend Programming |
| MySQL | Latest | Database Management |
| Bootstrap | 5.x | Frontend UI Design |
| Blade | Built-in | Templating Engine |
| Composer | Latest | Dependency Manager |
| VS Code | Latest | Code Editor |
| Git & GitHub | Latest | Version Control |

---

# 🏗️ System Architecture

The project follows the **MVC (Model–View–Controller)** architecture.

| Component | Responsibility |
|-----------|---------------|
| Model | Handles database interaction |
| View | Handles user interface |
| Controller | Handles business logic and requests |
| Routes | Define application URLs |
| Database | Stores task records |

---

# 📂 Project Structure

```bash
Todo_List_web/
│
├── app/
│   ├── Http/
│   │   └── Controllers/
│   │       └── TaskController.php
│   │
│   └── Models/
│       └── Task.php
│
├── database/
│   ├── migrations/
│   └── seeders/
│
├── public/
│
├── resources/
│   └── views/
│       ├── layouts/
│       ├── tasks/
│       └── components/
│
├── routes/
│   └── web.php
│
├── .env
├── composer.json
└── README.md
```

---

# ⚙️ Installation Guide

## Step 1 — Clone Repository

```bash
https://github.com/ahmadmirza2917/Todo_List_web.git
```

---

## Step 2 — Navigate to Project Folder

```bash
cd Todo_List_web
```

---

## Step 3 — Install Composer Dependencies

```bash
composer install
```

---

## Step 4 — Create Environment File

```bash
cp .env.example .env
```

---

## Step 5 — Configure Database

Update the `.env` file:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=Todo_List_web
DB_USERNAME=root
DB_PASSWORD=
```

---

## Step 6 — Generate Application Key

```bash
php artisan key:generate
```

---

## Step 7 — Run Database Migrations

```bash
php artisan migrate
```

---

## Step 8 — Run Database Seeder (Optional)

```bash
php artisan db:seed
```

---

## Step 9 — Start Laravel Development Server

```bash
php artisan serve
```

---

## Step 10 — Open Application

```bash
http://127.0.0.1:8000
```

---

# 🗄️ Database Schema

## Table: `tasks`

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| id | BIGINT | Primary Key |
| title | VARCHAR(255) | Task title |
| description | TEXT | Task description |
| due_date | DATE | Task deadline |
| priority | ENUM | Low / Medium / High |
| status | ENUM | Pending / Completed |
| created_at | TIMESTAMP | Record creation time |
| updated_at | TIMESTAMP | Last update time |

---

# 🌐 Application Routes

| HTTP Method | URI | Controller Method | Purpose |
|-------------|-----|------------------|---------|
| GET | / | index() | Show all tasks |
| POST | /tasks | store() | Save new task |
| GET | /tasks/{task}/edit | edit() | Show edit form |
| PUT | /tasks/{task} | update() | Update task |
| PATCH | /tasks/{task}/toggle | toggleStatus() | Toggle task status |
| DELETE | /tasks/{task} | destroy() | Delete task |
| GET | /about | about() | About page |

---

# 🧠 Core Functionalities

## CRUD Operations

| Operation | Description |
|-----------|-------------|
| Create | Add new tasks |
| Read | Display tasks |
| Update | Edit task information |
| Delete | Remove tasks |

---

## Filtering System

| Filter Type | Options |
|-------------|---------|
| Status | All, Pending, Completed |
| Priority | All, High, Medium, Low |

---

## Task Priorities

| Priority | Badge Color |
|----------|-------------|
| High | 🔴 Red |
| Medium | 🟡 Yellow |
| Low | 🟢 Green |

---

# 📸 Screenshots

## 🏠 Dashboard

<img width="1920" height="913" alt="Image" src="https://github.com/user-attachments/assets/660a9b44-b419-4018-bf49-50151fb496f5" />
<img width="1920" height="913" alt="Image" src="https://github.com/user-attachments/assets/d26947c2-143d-4773-a229-74aed1b8ebdd" />


## ➕ Add New Task


<img width="677" height="906" alt="Image" src="https://github.com/user-attachments/assets/1878ec15-6d5d-48cf-9397-689b9586a5d1" />


## ✏️ Edit Task


<img width="716" height="828" alt="Image" src="https://github.com/user-attachments/assets/4161431a-dd36-4efe-a42c-54dcd9144937" />



## 🔍 Filter Feature


<img width="1291" height="748" alt="Image" src="https://github.com/user-attachments/assets/b484c93d-ac6a-4911-a465-b06605204838" />



## ✅ Delete Tasks


<img width="1920" height="903" alt="Image" src="https://github.com/user-attachments/assets/fddf8d70-ee5d-41bf-ae75-9c7f5df22917" />



## ✅ Last 

<img width="1920" height="903" alt="Image" src="https://github.com/user-attachments/assets/f116bd93-5704-4d21-96b0-01e75801f866" />



## ✅About

<img width="1920" height="872" alt="Image" src="https://github.com/user-attachments/assets/2d04af59-5e45-4a0c-a485-09bf004d69a1" />
<img width="1920" height="902" alt="Image" src="https://github.com/user-attachments/assets/82ea4951-87ca-4f3c-959a-e7efe9e6bcec" />


---

# 🔐 Validation Rules

| Field | Validation Rule |
|-------|----------------|
| title | Required |
| priority | Must be Low, Medium, or High |
| due_date | Must be valid date |
| status | Pending or Completed |

---

# 📊 Dashboard Statistics

The application dashboard displays:

| Statistic | Description |
|-----------|-------------|
| Total Tasks | Total number of tasks |
| Pending Tasks | Tasks not completed |
| Completed Tasks | Finished tasks |

---

# 🚀 Laravel Concepts Used

| Concept | Usage |
|---------|------|
| Routing | URL management |
| Controllers | Request handling |
| Models | Database interaction |
| Blade Templates | Dynamic frontend |
| Eloquent ORM | Database queries |
| Query Scopes | Filtering tasks |
| Validation | Secure user input |
| Middleware | Request processing |
| Migrations | Database schema |

---

# 📚 Learning Outcomes

After completing this project, the following concepts were learned:

- Laravel Framework Development
- MVC Architecture
- CRUD Operations
- RESTful Routing
- Database Migrations
- Eloquent ORM
- Blade Templating
- Form Validation
- Bootstrap UI Development
- Git & GitHub Version Control

---

# 🔮 Future Enhancements

| Feature | Description |
|---------|-------------|
| 🔐 Authentication | User login and registration |
| 👥 Role Management | Admin/User roles |
| 🏷️ Categories | Task categories and tags |
| 📄 Pagination | Better task navigation |
| 🔔 Notifications | Due date reminders |
| 📤 Export | Export to PDF/CSV |
| ☁️ Deployment | Cloud hosting support |

---

# 👨‍💻 Author Information

| Field | Details |
|------|---------|
| Name | Ahmad Mirza |
| Student ID | CIIT/SP24-BSSE-002/VHR |
| Degree Program | BS Software Engineering |
| University | COMSATS University Islamabad |
| Campus | Vehari Campus |

---

# 👩‍🏫 Instructor

| Field | Details |
|------|---------|
| Instructor Name | Ma’am Yasmeen Jana |
| Course | CSC336 — Web Technologies |
| Semester | Spring 2026 |

---

# 🔗 GitHub Repository

```bash
https://github.com/ahmadmirza2917/Todo_List_web.git
```

---

# 📄 License

This project is developed for **educational purposes only**.

---

