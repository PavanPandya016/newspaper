# Newspaper

A simple Django-based news website that supports article posting, comments, user accounts and page management. This repository implements a small, easy-to-run project intended for learning and demonstration purposes.

## Features

- User registration, login and password management
- Create, edit and delete articles
- Commenting on articles
- Admin site for managing content
- Simple, responsive templates and static assets

## Requirements

- Python 3.8+
- Django (see `requirments.txt` for exact versions)

## Setup

1. Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate
```

2. Install dependencies:

```bash
pip install -r requirments.txt
```

3. Apply migrations and create the database:

```bash
python manage.py migrate
```

4. (Optional) Create a superuser to access the admin:

```bash
python manage.py createsuperuser
```

5. Collect static files (for deployment):

```bash
python manage.py collectstatic
```

6. Run the development server:

```bash
python manage.py runserver
```

Open http://127.0.0.1:8000 in your browser to view the site.

## Project Structure

- `accounts/` — user registration, login and profile views
- `articles/` — article models, views and comment functionality
- `pages/` — simple content pages and routing
- `django_project/` — project settings and root URL configuration
- `templates/` — HTML templates used by the app
- `static/` — CSS and static assets
- `db.sqlite3` — default SQLite database (created after migrations)

## Tests

Run the Django test suite with:

```bash
python manage.py test
```
