# Django Cheat Sheet  
My own cheat-sheet for creating web application using Django

## Folder structure
```
learningdjango
└───
README.md
```

## Start a project
```
django-admin startproject portfolio
```
### Files
```
manage.py - runs commands
portfolio/__init__.py - Tells Python that the folder contain Python files
portfolio/wsgi.py - Provides a hook for web servers
portfolio/settings.py - Configures Django
portfolio/urls.py - Routes requests based on URL
```

## Create an App
```
python manage.py startapp portfolio
```

## Pieces of App
| File / Folder | Role
| ------------- |----------------------------------|
| apps.py       | Configuration and Initialization |
| models.py     | Data layer                       |
| admin.py       | Administrative interface |
| urls.py | URL routing |
| views.py | Control layer |
| tests.py | Test the app |
| migrations | Holds migrations files |

## Models, routing, views and templates
learningdjango
