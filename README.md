# E-Commerce-Day6

Employee Management System


Overview

This project is an Employee Management System built using Java with Jakarta Persistence API (JPA) for database operations. It manages relationships between employees, departments, projects, and insurance information.

Project Structure

Entity Models

The system consists of four main entities:

Employee

Primary attributes: employee number, name, age, salary, gender


Relationships:

Many-to-One with Department

Many-to-Many with Project

One-to-One with Insurance

Department

Primary attributes: ID, name, establishment date

Relationships:

One-to-Many with Employee (a department has many employees)

Project

Primary attributes: ID, name, total cost

Relationships:

Many-to-Many with Employee (a project has many employees)

Insurance

Primary attributes: ID, type

Relationships:

One-to-One with Employee

Entity Relationships

An employee belongs to one department, but a department can have multiple employees

An employee can work on multiple projects, and a project can have multiple employees

An employee can have one insurance policy

Technologies Used

Java

Jakarta Persistence API (JPA)

[Database Technology] (e.g., MySQL,)

[Framework] (e.g., Spring Boot)

Setup Instructions

Clone the repository

Configure your database connection in application.properties or application.yml

Run the application

Database Schema

The application uses the following tables:

Employee,
Department,
Project,
Employee_Project (join table for the many-to-many relationship),
Insurance
