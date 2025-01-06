## Project Abstract

This project is a web application built using Flask that allows users to register, log in, and manage contact form submissions. The application provides user authentication using Flask-Login and stores user credentials and contact form data in an SQLite database. Once authenticated, users can submit contact messages, which are saved in the database. The system also includes a dashboard for viewing all submitted contact forms, which is accessible only to logged-in users. This project demonstrates the use of Flask for web development, including session management, database integration with SQLAlchemy, and form handling in a lightweight and secure environment.



## Features

- **User Authentication**: Register, log in, and log out functionality with password-based authentication.
- **Contact Management**: Submit contact forms with user information (name, email, message) and store them in an SQLite database.
- **Dashboard**: View all contact form submissions in a dashboard (accessible only to logged-in users).
- **Flask-SQLAlchemy Integration**: Use SQLAlchemy to manage users and store contact messages in the SQLite database.
- **Flask-Login Integration**: Provides login-required routes and session handling for users.
- **SQLite Database**: A lightweight SQL database that stores user information and contact form submissions.

## Prerequisites

- Python 3.x
- Flask
- Flask-SQLAlchemy
- Flask-Login

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/yourusername/yourrepository.git
    cd yourrepository
    ```

2. Install the required Python packages:

    ```bash
    pip install Flask Flask-SQLAlchemy Flask-Login
    ```

3. Set up your SQLite database:

    ```bash
    python
    >>> from your_script_name import init_sqlite_db
    >>> init_sqlite_db()
    ```

   This command will create the SQLite database and initialize the required tables.

## Project Structure

``
├── app.py                # Main Flask application
├── database.db           # SQLite database file (auto-generated)
├── README.md             # Project README
└── requirements.txt      # Dependencies
