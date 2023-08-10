#  <h1 align= "center">🎥 Cinema-App 🎥

## Introduction
REST web application for ticket reservation. It implements the main functions, such as:
- displaying movies that are currently at the box office.
- shopping cart with the ability to add tickets to it and create an order based on the added tickets.
- searching for available movie sessions by date.

## 🌐 Project structure:
- DAO (Data Access Object) - DAO is the data access layer responsible for interacting with the database. This layer implements operations related to retrieving, storing, updating, and deleting data.
- Service - The service layer is responsible for the business logic of the application. It handles data processing, executes business rules, and coordinates actions between the DAO and other components of the application.
- Controller - The Controller layer serves as the entry point for external requests to the application.

## 📝 Database Schema:
![img_1.png](img_1.png)

Endpoint description (with roles and http-methods):

User and Admin Endpoints:
- POST: /register - User registration.
- GET: /cinema-halls - View cinema halls.
- GET: /movies - View movies.
- GET: /movie-sessions/available - View available movie sessions.

Admin-only Endpoints:
- POST: /cinema-halls - Add a new cinema hall.
- POST: /movies - Add a new movie.
- POST: /movie-sessions - Add a new movie session.
- PUT: /movie-sessions/{id} - Update a movie session.
- DELETE: /movie-sessions/{id} - Delete a movie session.
- GET: /users/by-email - Find a user by their email address.

User-only Endpoints:
- GET: /orders - View user's orders.
- POST: /orders/complete - Complete an order.
- PUT: /shopping-carts/movie-sessions - Update the shopping cart with movie sessions.
- GET: /shopping-carts/by-user - View the shopping cart for a specific user.

Project structure:
- src/main/java - contains the entire source code of the program.
- src/main/resources - contains properties for connecting to the database.

## 💻 Technologies used:

- Java 17
- Tomcat 9.0.75
- MySQL 8.0.22
- Maven 3.1.1
- Java Servlet 4.0.1
- Spring 5.3.20
- Spring-Web 5.3.20
- Spring-Security 5.6.10
- Hibernate 5.6.14.Final
- JDBC

## 🚀 Instructions for launching the project:

1) Clone the project from GitHub.
2) Install Apache Tomcat version 9.x.x.
3) Install MySql.
4) Install Postman for sending requests.
5) Create an empty database.
6) Set up Database connectivity in src/main/resources/db.properties file with your own URL, username, password and JDBC driver.
7) Configure Tomcat server.
8) Add New Configuration/Tomcat Server/Local/Setup deployment configurations.
9) Run the project.
