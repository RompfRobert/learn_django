# Meeting Planner

A simple starter Django project for planning meetings.

## Prerequisites

- Python 3.8+  
- pip  
- (Optional) Virtual environment tool such as `venv` or `virtualenv`

## Setup

1. **Create and activate a virtual environment** (strongly recommended):

   ```bash
   python3 -m venv .venv

   # On Windows
   .venv\Scripts\activate
   
   # On macOS/Linux
   source .venv/bin/activate
   ```

2. **Install Django**:

   ```bash
   pip install django
   ```

## Starting the Project

Use Django’s built-in admin script to scaffold your project:

```bash
django-admin startproject meeting_planner
```

> This creates a new directory called `meeting_planner` containing your project files.

## Exploring the Project

```bash
# Move into the project directory
cd meeting_planner

# Verify the layout
tree .  # or use your IDE’s file-explorer
```

You should see something like:

```
meeting_planner/
├── manage.py
├── db.sqlite3            # Auto-created when you run the server
└── meeting_planner/      # Inner folder—your actual Django project
    ├── __init__.py
    ├── asgi.py
    ├── settings.py       # Main configuration file
    ├── urls.py           # URL routing
    └── wsgi.py
```

## Running the Development Server

```bash
python manage.py runserver
```

- By default, the server runs at `http://127.0.0.1:8000/`  
- To stop the server, return to the terminal and press <kbd>Ctrl</kbd>+<kbd>C</kbd>.

If you don’t see any output in your IDE’s file browser (e.g. PyCharm), right-click the project root and choose **Reload from Disk** (or similar).

## Next Steps

- Create new Django apps with:
  ```bash
  python manage.py startapp <app_name>
  ```
- Apply database migrations:
  ```bash
  python manage.py makemigrations
  python manage.py migrate
  ```
- Open `meeting_planner/settings.py` to configure:
  - Installed apps
  - Database settings
  - Static files, templates, etc.
- Define URL patterns in `meeting_planner/urls.py`.

Happy coding!  