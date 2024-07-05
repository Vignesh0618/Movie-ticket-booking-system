# Movie Ticket Booking System

A simple Java application for booking and managing movie tickets using MySQL database and JDBC.

## Table of Contents

- [Features](#features)
- [Setup](#setup)
- [Prerequisites](#prerequisites)
- [Database Setup](#database-setup)
- [Running the Application](#running-the-application)
- [Usage](#usage)

## Overview

This Java application allows users to book movie tickets, update ticket details (fare, class, time, theater, phone number), cancel tickets, and view all booked tickets. It uses JDBC to interact with a MySQL database (`Ticket`) locally.

## Features

- **Ticket Booking:** Users can book multiple movie tickets in one session.
- **Ticket Management:** Options to update fare, class, time, theater, and phone number for booked tickets.
- **Cancellation:** Ability to cancel booked tickets.
- **Viewing Tickets:** Display all booked tickets with their details.

## Setup

### Prerequisites

- Java Development Kit (JDK) installed (version 8 or higher).
- MySQL Database Server installed and running.
- MySQL JDBC Driver (included in the project or added through dependency management).

### Database Setup

1. **Create Database:**
   - Open MySQL console or any MySQL management tool (like MySQL Workbench).
   - Execute the following SQL command to create the database:

     ```sql
     CREATE DATABASE Ticket;
     ```

2. **Create Table:**
   - The application automatically creates a table `MovieTicketDetail` if it doesn't exist with the following schema:

     ```sql
     CREATE TABLE IF NOT EXISTS MovieTicketDetail (
       ticket_id VARCHAR(20) NOT NULL,
       peoplename VARCHAR(50) NOT NULL,
       Moviename VARCHAR(50) NOT NULL,
       Theatre VARCHAR(50) NOT NULL,
       class VARCHAR(20) NOT NULL,
       time VARCHAR(30) NOT NULL,
       gender VARCHAR(1) NOT NULL,
       ph_number VARCHAR(10) NOT NULL,
       fare VARCHAR(50) NOT NULL,
       PRIMARY KEY (ticket_id)
     );
     ```

### Running the Application

1. Clone the repository or download the ZIP file and extract it.
2. Navigate to the project directory containing `BookTickets.java`.
3. Compile the Java file:

   ```bash
   javac BookTickets.java



## contact
For any questions or suggestions, feel free to contact me at vijayvignesh88382@gmail.com
