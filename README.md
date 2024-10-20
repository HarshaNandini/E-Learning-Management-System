# Harsha's E-learning Management System

Welcome to my E-learning Management System that allows students to enroll in and learn courses, add courses to their wishlist, and manage their learning experience. The system supports three modes of operation:
1. **Admin**
2. **Student**
3. **Teacher**

## Table of Contents

- [Tech Stack](#tech-stack)
- [Features](#features)
- [Getting Started](#getting-started)
- [Frontend Setup](#frontend-setup)
- [Backend Setup](#backend-setup)
- [Additional Commands](#additional-commands)
- [Modes of Operation](#modes-of-operation)

## Tech Stack

### Frontend Services
- HTML, CSS
- TypeScript
- jQuery
- Angular Material
- Bootstrap
- Youtube Player API

### Backend Services
- Java
- Spring Boot
- Spring Security
- JWT Bearer Tokens
- MySQL Database

### Development Tools
- Spring Tool Suite (STS)
- Postman
- Visual Studio Code (VSCode)

## Features

### Admin Mode
- Add a Teacher
- Manage Users (Students)
- Manage Teachers
- Add new Courses and Chapters
- View lists of Teachers, Courses, Users
- Approve or reject Teacher registrations
- Admin Dashboard: Overview of total Teachers, Users, Learners, Courses, and Chapters, as well as the most liked courses.

### Teacher Mode
- Register for a new account to access the platform
- View available Users and Courses
- Add new Courses and Chapters
- Manage Profile: View & edit profile details
- Enroll in courses and mark them as favorites
- Check registration approval by the Admin
- Teacher Dashboard: Overview of total Learners, Courses, Chapters, and the most liked courses.

### Student Mode
- Register for a new account
- View available Courses and Learning Content
- Manage Profile: View & edit profile details
- Enroll in new courses and manage favorites
- User Dashboard: Overview of total Learners, Courses, and the most liked courses
- **Additional Feature:** Users can enroll in YouTube tutorial courses embedded directly in the platform.

## Getting Started

Follow the steps below to set up the E-LMS project locally.

### Prerequisites

Ensure you have the following tools installed:
- **Node.js** (for the frontend)
- **Java** (for the backend)
- **MySQL** (for the database)

### Frontend Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/harshanandini/frontend.git
   cd frontend
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the development server:**
   ```bash
   ng serve
   ```
The frontend will be available at http://localhost:4200/

### Backend Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/harshanandini/backend.git
   cd backend
   ```
2. **Configure the database: Open application.properties in the src/main/resources folder and update your MySQL connection:**
   ```bash
    spring.datasource.url=jdbc:mysql://localhost:3306/your-database
    spring.datasource.username=your-username
    spring.datasource.password=your-password
   ```
3. **Run the backend:**
   ```bash
   ./mvnw spring-boot:run
   ```
The backend will be available at http://localhost:8000/.

### Frontend Code scaffolding 
    **Run the following command to generate a new Angular component:** 
   ```bash
   ng generate component component-name
   ```
    **Building the frontend**
    To build the Angular project, run:
    ```bash 
    ng build
    ```
    The build artifacts will be stored in the dist/ directory.

### Modes of Operation
This eLMS supports three modes of operation for different types of users: Admin, Teacher, and Student. Each mode has a dedicated set of features, enabling seamless management of courses and learning activities.

Admin: Manage Teachers, Students, and Courses.
Teacher: Create and manage courses, view available users, and enroll in courses.
Student: Enroll in courses, manage wishlist, and view available learning content.