# Meeting Planner

A simple starter Django project for planning meetings.

## Prerequisites

- Python 3.8+  
- pip  
- (Optional) Virtual environment tool such as `venv` or `virtualenv`

## Setup

1. **Create and activate a virtual environment** (strongly recommended):

   A virtual environment ensures that your project dependencies are isolated from other Python projects on your system.

   ```bash
   python3 -m venv .venv

   # On Windows
   .venv\Scripts\activate
   
   # On macOS/Linux
   source .venv/bin/activate
   ```

   > If you encounter issues activating the virtual environment, ensure your Python installation is correctly configured in your system’s PATH.

2. **Verify Python and pip versions**:

   Before proceeding, ensure you have the correct versions installed:

   ```bash
   python3 --version
   pip --version
   ```

   You should see Python 3.8+ and a recent version of pip.

3. **Install Django**:

   ```bash
   pip install django
   ```

   This installs the latest version of Django in your virtual environment.

## Starting the Project

Use Django’s built-in admin script to scaffold your project:

```bash
django-admin startproject meeting_planner
```

> The `django-admin` command is a utility provided by Django to help you create and manage projects. This command creates a new directory called `meeting_planner` containing your project files.

## Exploring the Project

1. **Navigate to the project directory**:

   ```bash
   cd meeting_planner
   ```

2. **Verify the project layout**:

   ```bash
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

1. **Start the server**:

   ```bash
   python manage.py runserver
   ```

   - By default, the server runs at `http://127.0.0.1:8000/`.  
   - To stop the server, return to the terminal and press <kbd>Ctrl</kbd>+<kbd>C</kbd>.

2. **Troubleshooting**:

   - If you encounter issues, ensure you are in the `meeting_planner` directory before running the command.
   - If you don’t see any output in your IDE’s file browser (e.g., PyCharm), right-click the project root and choose **Reload from Disk** (or similar).

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