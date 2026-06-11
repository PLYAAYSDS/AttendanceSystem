# Attendance Management System

## Overview
Attendance Management System is a web-based application built using React, NestJS, PostgreSQL, and JWT Authentication.

### Frontend
- React.js
- Axios
- React Router

### Backend
- NestJS
- PostgreSQL
- JWT Authentication

## Features

### Authentication
- Login using email and password
- JWT-based authentication
- Protected routes
- Role-based access control

### Employee Features
#### Attendance
- Check In
- Check Out

#### Attendance History
- View attendance records
- Filter by date range (From / To)

#### Profile Management
- View profile
- Update phone number
- Upload profile picture
- Change password

### Admin Features
#### Employee Management
- View employee list
- Create employee
- View employee attendance history

#### Employee Attendance History
Endpoint:

POST /api/employees/{employeeId}/attendance

Request:
```json
{
  "from": "2026-06-01",
  "to": "2026-06-30"
}
```

### Security
All protected endpoints require:

Authorization: Bearer <JWT_TOKEN>

## Application Flow

Login
 -> JWT Token Issued
 -> Dashboard
    -> Attendance
    -> Attendance History
    -> Profile
    -> Employee Management (Admin)
