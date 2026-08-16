# Django Starter App

A minimal Django application built while learning the framework. One view, one template, and the mechanism for getting data from the backend into the page.

## What it demonstrates

- Django project vs **app** structure (`myApp/` project, `home/` app)
- URL routing — mapping the root route to a view
- A view returning `render()` with a **context dictionary**
- Template consuming that context to render server-side

The single view builds a list of records and hands it to `index.html` through the context — the core "backend passes data to the template" mechanic that everything else in Django builds on.

## Layout

```
myApp/           # project — settings, urls, wsgi/asgi
home/            # app
  views.py       # the home view
  models.py
  templates/
    index.html
manage.py
```

## Running it

```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install django
python manage.py migrate
python manage.py runserver
```

Then open `http://localhost:8000`.

## Scope

This is a learning exercise, kept as a record of working through the Django basics — not an application in use.
