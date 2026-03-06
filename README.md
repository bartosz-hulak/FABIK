# FABIK – Patrol Management System

A lightweight, emergency service-style patrol management web app built with Django. Created as a university project to demonstrate Django basics, simple CRUD, and Firebase integration.

## Features

- Clean, fast UI inspired by emergency service systems
- Real-time patrol status tracking
- Person and vehicle search functionality
- Intervention management with notes
- Polish language UI (codebase in English)
- Firebase integration for real-time data

## Tech Stack

- **Backend**: Django 5.2 (Python 3.13)
- **Database**: SQLite (local development) + Firebase Firestore
- **Frontend**: Django templates + Bootstrap 5
- **Real-time**: Firebase Firestore

## Quick Start (Local)

1. **Clone & install**

   ```bash
   git clone <repo-url>
   cd FABIK
   python -m venv .venv
   .venv\Scripts\Activate.ps1   # Windows
   pip install -r requirements.txt
   ```

2. **Environment setup**

   ```bash
   Create .env file with SECRET_KEY
   Add credentials.json for Firebase
   ```

3. **Database setup**

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

4. **Run**

   ```bash
   python manage.py runserver
   ```
   Visit `http://127.0.0.1:8000` → login → access patrol dashboard.

## Project Structure

```text
FABIK/
├── FABIK/                 # Django project settings
├── Application/
│   ├── models.py         # UserProfile, Message
│   ├── views.py          # Main views
│   ├── templates/        # UI templates
│   └── static/           # CSS + JS
├── templates/            # Global templates
├── requirements.txt
├── .env                  # Local env vars
└── credentials.json      # Firebase key (not tracked)
```

## Notes

- Uses SQLite for simplicity with Firebase for real-time features.
- Firebase credentials stored locally (not in repository).
- Polish interface with English codebase.
- University project - not production ready.
