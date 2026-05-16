# 📝 Flask Todo App

A full-stack todo web application built with Flask, SQLite, and SQLAlchemy.

## Features
- User authentication (login/logout)
- Add, delete, and manage tasks
- Task status tracking (Pending → Working → Done)
- Flash messages for user feedback
- Blueprint-based project structure

## Tech Stack
- **Backend:** Python, Flask
- **Database:** SQLite, Flask-SQLAlchemy
- **Frontend:** HTML, CSS, Jinja2

## Project Structure
```
todo-flask-app/
├── app/
│   ├── __init__.py
│   ├── models.py
│   ├── routes/
│   │   ├── auth.py
│   │   └── tasks.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── login.html
│   │   └── tasks.html
│   └── static/
│       └── css/
│           └── style.css
└── run.py
```

## Setup
```bash
git clone https://github.com/aira-j/todo-flask-app.git
cd todo-flask-app
pip install flask flask-sqlalchemy
python3 -c "from app import create_app, db; app = create_app(); app.app_context().push(); db.create_all()"
python3 run.py
```

## Login Credentials
- **Username:** admin
- **Password:** 1234
