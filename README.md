# Employee Management System

## Overview
The **Employee Management System** enables users to efficiently **add, view, update, and delete** employees and departments via a **React frontend** connected to a **Spring Boot backend**.

## Key Features
- **CRUD Operations**: Manage employees and departments seamlessly.
- **Interactive UI**: Built with **React & Tailwind CSS** for a responsive design.
- **Real-time Data Handling**: Uses **Axios** for API communication with the backend.
- **Data Visualization**: Displays department-wise employee statistics using **Chart.js**.
- **Search & Filtering**: Easily find and manage employees with dynamic filtering.
- **REST API Integration**: Fetches and stores data through secure **Spring Boot APIs**.

## Tech Stack
- **Frontend**: React, Tailwind CSS, Axios, Chart.js
- **Backend**: Spring Boot, Java, REST APIs
- **Database**: PostgreSQL / MySQL (configurable)
- **Deployment**: Docker, Kubernetes (optional)

This system ensures **real-time updates** and a **smooth user experience**, making employee management **efficient and intuitive**.


# Employee Management App  

An Employee Management System built using a **Spring Boot backend** and a **React.js frontend**, designed to manage employees and departments efficiently. This full-stack application includes features like creating, updating, viewing, and deleting employees and departments.  

## Table of Contents  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Project Structure](#project-structure)  
- [Installation](#installation)  
- [Usage](#usage)  
- [API Documentation](#api-documentation)  
- [Screenshots](#screenshots)  

---

## Features  

### Backend:  
- RESTful APIs for CRUD operations on Employees and Departments.  
- Structured service layer for handling business logic.  
- Exception handling with custom error responses.  
- Initial database setup with `data.sql`.  

### Frontend:  
- Responsive UI for managing employees and departments.  
- Dashboard with data visualization using charts.  
- Dynamic forms for adding/editing employees and departments.  
- Global state management for seamless user experience.  
- Styled using Tailwind CSS for modern and clean aesthetics.  

---

## Tech Stack  

### Backend:  
- Java  
- Spring Boot (MVC, JPA, Hibernate)  
- PostgreSQL (or any other RDBMS supported by JPA)  

### Frontend:  
- React.js  
- Tailwind CSS  
- Axios (for API calls)  

---

## Project Structure  

### Backend:  
```plaintext  
backend/  
├── src/  
│   ├── main/java/com/example/employeemanagement/  
│   │   ├── EmployeeManagementApplication.java – Main backend entry point  
│   │   ├── controller/  
│   │   │   ├── EmployeeController.java – Handles API requests for employees  
│   │   │   ├── DepartmentController.java – Handles API requests for departments  
│   │   ├── model/  
│   │   │   ├── Employee.java – Employee entity  
│   │   │   ├── Department.java – Department entity  
│   │   ├── repository/  
│   │   │   ├── EmployeeRepository.java – Database interactions for employees  
│   │   │   ├── DepartmentRepository.java – Database interactions for departments  
│   │   ├── service/  
│   │   │   ├── EmployeeService.java – Business logic for employees  
│   │   │   ├── DepartmentService.java – Business logic for departments  
│   │   ├── exception/  
│   │   │   ├── ResourceNotFoundException.java – Handles API errors  
│   │   ├── resources/  
│   │       ├── application.properties – Database and server config  
│   │       ├── data.sql – Initial database data (optional)  
├── pom.xml – Dependencies and build configuration  
