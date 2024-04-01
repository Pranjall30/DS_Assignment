# Student Registration Form with Flask and SQL

This project implements a web-based student registration system using Flask for the backend, HTML for the frontend, and MySQL as the database. It allows students to register by filling out a form, and upon submission, the user's information is stored in a MySQL database.

## Table of Contents

- [Requirements](#requirements)
- [Database Setup](#database-setup)
- [Flask Application](#flask-application)
- [HTML Form](#html-form)
- [Additional Features](#additional-features)
- [Installation](#installation)
- [Usage](#usage)

## Requirements

### Database Setup:

- **MySQL Database:** Create a MySQL database named `Pranjal`.

### Flask Application:

- **Python**
- **Flask**: Install Flask using `pip install Flask`.
- **Flask-MySQLdb**: Install Flask-MySQLdb using `pip install Flask-MySQLdb`.

## Database Setup

1. Create a MySQL database named `Pranjal`.
2. Inside `Pranjal`, create a table named `users` with the following columns:
   - id (Auto-incrementing primary key)
   - Student name
   - Father name
   - Mother name
   - Phone number
   - Email
   - Date of birth
   - Address
   - Blood group
   - Department
   - Course
   - Password 

## Flask Application

1. Set up a Flask application with the following endpoints:
   - `/`: Renders the registration form.
   - `/register`: Handles form submission, saves data to the MySQL `users` table, and redirects to the root endpoint.

2. Implement password hashing for secure storage in the database.

3. Implement user login functionality with authentication against the database.

## HTML Form

Create an HTML form (`register.html`) with the following fields:
- Student name
- Father name
- Mother name
- Phone number
- Email
- Date of birth
- Address
- Blood group
- Department
- Course
- Password (input type=password)

Ensure that the form submits data to the `/register` endpoint of the Flask application.


