# Signup Form Project

This project is a simple web-based signup form created using HTML, CSS, and PHP. The form captures user information such as name, address, phone number, age, and email, and stores the data in a MySQL database.

## Project Structure

- **signup.html**: The HTML file that contains the form layout and structure.
- **signup.php**: The PHP script that handles form submissions and stores data in the MySQL database.
- **signup_database.sql**: SQL script to create the required database and table.

## Getting Started

### Prerequisites

- A web server with PHP support (e.g., XAMPP, WAMP, or LAMP)
- MySQL database

### Setup

1. **Clone the repository** or download the files.

2. **Create the Database:**
   - Use the following SQL script to create the `signup_database` and `users` table:
   ```sql
   CREATE DATABASE signup_database;

   USE signup_database;

   CREATE TABLE users (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100) NOT NULL,
       address TEXT NOT NULL,
       phone_number VARCHAR(15) NOT NULL,
       age INT NOT NULL,
       email VARCHAR(100) NOT NULL UNIQUE
   );
