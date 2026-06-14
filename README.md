# Hospital Management System

A simple Java Console-Based Hospital Management System developed using JDBC and MySQL. This project demonstrates CRUD operations, database connectivity, and appointment booking functionality.

## Features

* Add new patients
* View all patients
* View all doctors
* Book appointments
* Check doctor availability before booking
* MySQL database integration using JDBC

## Technologies Used

* Java
* JDBC
* MySQL
* Object-Oriented Programming (OOP)

## Project Structure

```
HospitalManagementSystem/
│
├── HospitalManagementSystem.java
├── Patient.java
├── Doctor.java
└── Database (MySQL)
```

## Database Tables

### Patients

* id
* name
* age
* gender

### Doctors

* id
* name
* specialization

### Appointments

* id
* patient_id
* doctor_id
* appointment_date

## How It Works

1. User selects an option from the menu.
2. Patient and doctor details are fetched from the database.
3. Before booking an appointment, the system checks whether the doctor already has an appointment on the selected date.
4. If available, the appointment is booked successfully.

## Setup Instructions

1. Install MySQL Server.
2. Create a database named:

```sql
CREATE DATABASE hospital;
```

3. Create the required tables (patients, doctors, appointments).
4. Update database credentials in `HospitalManagementSystem.java`:

```java
private static final String url = "jdbc:mysql://localhost:3306/hospital";
private static final String username = "root";
private static final String password = "root";
```

5. Add MySQL JDBC Driver to the project.
6. Run `HospitalManagementSystem.java`.

## Sample Menu

```
Hospital Management System

1. Add Patient
2. View Patients
3. View Doctors
4. Book Appointment
5. Exit
```

## Learning Outcomes

* JDBC Connectivity
* PreparedStatement Usage
* ResultSet Handling
* SQL CRUD Operations
* Java OOP Concepts
* Exception Handling

## Future Enhancements

* Appointment Time Slots
* Update/Delete Records
* Search Functionality
* GUI using Java Swing/JavaFX
* Doctor and Patient Authentication

## Author

Sahiljeet Singh
Java Full Stack Developer (Fresher)
