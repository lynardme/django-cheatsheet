# Django Cheat Sheet  
My own cheat-sheet for creating web application using Django

## Folder structure
```
learning-django
└─── portfolio
    └─── portfolio
         ─ settings.py
         ─ urls.py
         ─ wsgi.py
    └─── db.sqlite3
    └─── manage.py
└─── .gitignore
└─── README.md
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
__URL Patterns__ - portfolio/urls.py  
__Views__ - portfolio/views.py  
__Templates__ - portfolio/templates  
__Models__ - portfolio/model.py  

### Models
- Create the data layer of an app
- Define database structure
- Allow us to query the database

### Field Types
| Field | Example Values |
|-------| ---------------|
| IntegerField | -1, 0, 1, 20 |
| DecimalField | 0.5, 3.14 |
| CharField | "Product Name" |
| TextField | "To elaborate on my point..." |
| EmailField | "hello@email.com" |
| URLField | www.example.com |
| BooleanField | True, False |
| DateTimeField | datetime(1960, 1, 1, 8, 0, 0) |
| ForeignKey | 1 (id of another table) |
| ManyToMany | NA |

### Migrations
Generate scripts to change the database structure  
### Migration commands ###
```
python manage.py makemigrations  
python manage.py migrate
```