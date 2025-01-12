# Flask Login App

This is a simple Flask login application that demonstrates user registration and login functionality.

## Prerequisites

* Python 3.6 or later
* Flask
* Flask-SQLAlchemy
* python-dotenv
* mysql-connector-python

## Installation

1. Clone this repository.
2. Create a virtual environment and activate it.
3. Install the required dependencies:

```bash
pip install flask flask-sqlalchemy python-dotenv mysql-connector-python
Create a file named .env in the root directory of your project. Add the following environment variables to the .env file, replacing the placeholders with your actual database credentials:
FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your_secret_key
SQLALCHEMY_DATABASE_URI=mysql://username:password@host/database_name
Running the application
Start the development server:
Bash

flask run
The application will be accessible at http://localhost:8888 by default.
Functionality
The application provides two main functionalities:

User Registration: Users can create new accounts by providing their name, email, and password.
User Login: Existing users can log in using their email and password.1   
1.
github.com
github.com
Code Structure
The application code is organized into the following files:

app.py: The main Flask application file.
database.py: Contains functions for interacting with the database, such as finding users and adding new users.
.env: Stores sensitive configuration variables like database credentials.
Database Schema
The application uses a simple database schema with a single table named users. The users table has the following columns:

id: (Integer, Primary Key) The unique identifier for the user.
name: (String) The user's name.
email: (String) The user's email address.
password: (String) The user's password (hashed).
