# 📝 Laravel To-Do List Management System

A complete **Laravel-based To-Do List Management System** developed for the course **CSC336 – Web Technologies** at COMSATS University Islamabad, Vehari Campus.

This project demonstrates the implementation of a modern web application using the **Laravel PHP Framework** following the **MVC (Model–View–Controller)** architecture. The system provides full CRUD functionality along with task priority management, status tracking, filtering, and dashboard statistics.

---

# 📌 Features

✅ Create new tasks  
✅ View all tasks in a structured dashboard  
✅ Update task details  
✅ Delete tasks with confirmation dialog  
✅ Task priority levels (Low / Medium / High)  
✅ Task status management (Pending / Completed)  
✅ Status toggle functionality  
✅ Filter tasks by priority and status  
✅ Real-time statistics dashboard  
✅ Server-side form validation  
✅ Flash success/error messages  
✅ Responsive UI using Bootstrap 5  

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Laravel 11.x | PHP Framework |
| PHP 8.x | Backend Programming |
| MySQL | Database Management |
| Blade Template Engine | Dynamic Views |
| Bootstrap 5 | Frontend Styling |
| Composer | Dependency Management |
| Git & GitHub | Version Control |

---

# 📂 Project Structure

```bash
Todo_List_web/
│
├── app/
│   ├── Http/Controllers/
│   ├── Models/
│
├── database/
│   ├── migrations/
│   ├── seeders/
│
├── resources/
│   ├── views/
│
├── routes/
│   └── web.php
│
├── public/
├── .env
├── composer.json
└── README.md

⚙️ Installation Guide
Step 1 — Clone Repository
git clone https://github.com/your-username/todo-list-laravel.git
Step 2 — Move to Project Folder
cd todo-list-laravel
Step 3 — Install Dependencies
composer install
Step 4 — Configure Environment File

Copy .env.example file:

cp .env.example .env

Then update database configuration inside .env:

DB_DATABASE=todo_list_web
DB_USERNAME=root
DB_PASSWORD=
Step 5 — Generate Application Key
php artisan key:generate
Step 6 — Run Database Migrations
php artisan migrate
Step 7 — (Optional) Run Seeder
php artisan db:seed
Step 8 — Start Development Server
php artisan serve

Now open:

http://127.0.0.1:8000
🗄️ Database Schema
Table: tasks
Column	Type	Description
id	BIGINT	Primary Key
title	VARCHAR	Task Title
description	TEXT	Task Description
due_date	DATE	Due Date
priority	ENUM	Low / Medium / High
status	ENUM	Pending / Completed
created_at	TIMESTAMP	Record Created Time
updated_at	TIMESTAMP	Last Updated Time
🚀 Application Routes
Method	Route	Purpose
GET	/	Show all tasks
POST	/tasks	Store new task
GET	/tasks/{task}/edit	Edit task form
PUT	/tasks/{task}	Update task
PATCH	/tasks/{task}/toggle	Toggle task status
DELETE	/tasks/{task}	Delete task
GET	/about	About page
📸 Screenshots
Dashboard

Add Task

Edit Task

Filter Feature

Completed Tasks

🧠 Key Concepts Implemented
MVC Architecture
Laravel Routing
Controllers & Models
Blade Templating
Eloquent ORM
Query Scopes
Form Validation
RESTful APIs
CRUD Operations
Bootstrap UI Design
📚 Learning Outcomes

Through this project, the following concepts were learned:

Laravel Framework Development
CRUD-based Web Applications
Database Design & Migration
Query Filtering using Eloquent Scopes
Server-side Validation
Responsive Frontend Design
Git & GitHub Version Control
🔮 Future Improvements
User Authentication
Role-Based Access Control
Task Categories & Tags
Pagination
Due Date Notifications
Export to PDF/CSV
Cloud Deployment
