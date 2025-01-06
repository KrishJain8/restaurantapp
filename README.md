# Flask User Authentication and Contact Management System

This project is a web-based contact management system built using Flask. It includes user authentication (registration, login, and logout) along with a system to submit and store contact messages in a SQLite database. The application uses Flask-Login for user session management and Flask-SQLAlchemy for ORM database operations.

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

```bash
.
├── templates
│   ├── login.html        # Login page
│   ├── register.html     # Registration page
│   ├── contact.html      # Contact submission page (home)
│   └── dashboard.html    # Dashboard to view all submissions
├── app.py                # Main Flask application
├── database.db           # SQLite database file (auto-generated)
├── README.md             # Project README
└── requirements.txt      # Dependencies
