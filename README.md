# School Management System

> **Note**: This project is not responsive. Simple HTML and CSS are used for the frontend.

---

## Overview

The **School Management System** is a Laravel-based application designed to streamline the management of students, teachers, classes, timetables, and attendance. It incorporates role-based access control to ensure that users have appropriate permissions based on their roles.

---

## Database Setup

1. Go to the `database` folder in the project.
2. Locate the `school_management_system_task` file.
3. Open MySQL in XAMPP and import this file into your database.

---

## Login Details

### Admin:
- **Email**: `admin123@gmail.com`
- **Password**: `admin123`

### Teacher:
- **Email**: `maazrehan@gmail.com`
- **Password**: `12345678`

---

## Features

### 1. Role-Based Access Control

- **Admin**:
  - Full access to all modules, including student, teacher, class, and timetable management.

- **Teacher**:
  - Access to their assigned class schedules and student lists.
  - Ability to mark and view attendance.

---

### 2. Modules

#### a. Student Management
- Add, edit, delete, and view students.
- Assign students to specific classes.
- Manage student details like:
  - Name, Roll Number, Class, Date of Birth, and Parent Contact.

#### b. Teacher Management
- Add, edit, delete, and view teachers.
- Assign teachers to specific classes.
- Manage teacher details like:
  - Name, Email, Subject Expertise, and Contact Number.

#### c. Class Management
- Add, edit, delete, and view classes.
- Assign a teacher and students to each class.
- Track class details, including:
  - Class Name, Assigned Teacher, and Student List.

#### d. Timetable Management
- Create and manage timetables for each class.
- Assign subjects, teachers, and time slots for classes.

#### e. Attendance System
- Teachers can:
  - Mark daily attendance for their students.
  - View attendance history for the current month.

---

## Frontend Features

### Admin Dashboard:
- Displays an overview of total students, teachers, and classes.
- Provides quick links to manage modules.

### Teacher Dashboard:
- Lists assigned classes and schedules.
- Includes attendance marking functionality.

---

## Database Design

The application uses **Eloquent Relationships** in Laravel for efficient data handling:

- **Users** (stores admin and teacher details).
- **Students**.
- **Classes**.
- **Subjects**.
- **Timetable**.
- **Attendance**.

### Key Relationships:
- **One-to-Many**:
  - Class ↔ Students, Teacher ↔ Classes.
- **Many-to-Many**:
  - Subjects ↔ Classes.
