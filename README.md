# Todo App

A clean and responsive Todo application built with Django. The app provides a simple interface for creating, editing, deleting, and clearing tasks, with a glass-style panel and modern office background design.

## Preview

The interface includes:

- A centered translucent Todo panel
- Responsive layout for desktop and mobile screens
- Purple add and clear controls
- Orange edit controls
- Red delete controls
- Live task count

## Features

- Add new tasks
- Edit existing tasks inline
- Delete individual tasks
- Clear all tasks at once
- Store tasks in a SQLite database
- Display the current number of tasks
- Responsive styling for smaller screens
- CSRF protection on POST forms
- Visual focus and hover states

## Built With

- Python
- Django 6.1.1
- SQLite
- HTML
- CSS
- JavaScript

## Project Structure

```text
todo_project/
├── manage.py
├── db.sqlite3                 # Local database, ignored by Git
├── CHANGES.md                 # Project change notes
├── README.md                  # Project documentation
├── static/
│   └── style.css              # Application styling
├── todo/
│   ├── migrations/
│   ├── templates/todo/
│   │   └── list.html          # Todo page
│   ├── models.py              # Todo database model
│   ├── urls.py                # Todo URL routes
│   └── views.py               # Todo operations
└── todo_project/
    ├── settings.py
    ├── urls.py
    ├── asgi.py
    └── wsgi.py
```

## Requirements

- Python 3.10 or newer
- pip
- Git

## Installation

Clone the repository:

```powershell
git clone https://github.com/M-Junaid/todo-app.git
cd todo-app
```

Create and activate a virtual environment:

```powershell
python -m venv env
.\env\Scripts\Activate.ps1
```

Install Django:

```powershell
python -m pip install django
```

Apply the database migrations:

```powershell
python manage.py migrate
```

## Run the Application

Start the Django development server:

```powershell
python manage.py runserver
```

Open the application in your browser:

```text
http://127.0.0.1:8000/
```

## How to Use

1. Enter a task in the input field.
2. Select the `+` button to add it.
3. Select the orange edit button to update a task.
4. Select the red delete button to remove one task.
5. Select `Clear All` to remove every task.
