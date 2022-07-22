Todo API
===
Abstract:Se creó e implementó un back-end de la Todo API que contiene un punto de conexión de la API de lista para todas las tareas y puntos de conexión dedicados para cada tarea individual. Se incorporo intercambio de origenes cruzados CORS. Se configuro para usar postgres en producion con heroku y Sqlite3 en local.
## Information
- Title:  `Todo`
- Author:  `jocnn`
- Heroku: [https://zza-todo.herokuapp.com/api/](https://zza-todo.herokuapp.com/api/)

## Install & Dependence
- asgiref==3.5.2
- black==22.6.0
- click==8.1.3
- dj-database-url==0.5.0
- dj-email-url==1.0.5
- Django==4.0.6
- django-cache-url==3.4.2
- django-cors-headers==3.10.1
- djangorestframework==3.13.1
- environs==9.3.5
- gunicorn==20.1.0
- marshmallow==3.17.0
- mypy-extensions==0.4.3
- packaging==21.3
- pathspec==0.9.0
- platformdirs==2.5.2
- psycopg2==2.9.3
- pyparsing==3.0.9
- python-dotenv==0.20.0
- pytz==2022.1
- sqlparse==0.4.2
- tomli==2.0.1
- whitenoise==5.3.0

## Use
- for run localhost
  ```
  (.venv) > python manage.py runserver
  ```
- for test
  ```
  (.venv) > python manage.py test
  ```
- for heroku
  ```
  https://zza-todo.herokuapp.com/api/    - api
  https://zza-todo.herokuapp.com/api/1/  - detail
  ```

## Directory Hierarchy
```
|—— .env
|—— .gitignore
|—— .venv
|—— Procfile
|—— db.sqlite3
|—— django_project
|    |—— __init__.py
|    |—— __pycache__
|        |—— __init__.cpython-310.pyc
|        |—— settings.cpython-310.pyc
|        |—— urls.cpython-310.pyc
|        |—— wsgi.cpython-310.pyc
|    |—— asgi.py
|    |—— settings.py
|    |—— urls.py
|    |—— wsgi.py
|—— manage.py
|—— requirements.txt
|—— runtime.txt
|—— scheenshots
|    |—— Detail Todo - Todo.png
|    |—— List Todo – Todo.png
|—— static
|    |—— css
|        |—— base.css
|    |—— js
|        |—— base.js
|—— staticfiles
|    |—— css
|        |—— base.css
|    |—— js
|        |—— base.js
|    |—— staticfiles.json
|—— todos
|    |—— __init__.py
|    |—— __pycache__
|        |—— __init__.cpython-310.pyc
|        |—— admin.cpython-310.pyc
|        |—— apps.cpython-310.pyc
|        |—— models.cpython-310.pyc
|        |—— serializers.cpython-310.pyc
|        |—— tests.cpython-310.pyc
|        |—— urls.cpython-310.pyc
|        |—— views.cpython-310.pyc
|    |—— admin.py
|    |—— apps.py
|    |—— migrations
|        |—— 0001_initial.py
|        |—— __init__.py
|        |—— __pycache__
|            |—— 0001_initial.cpython-310.pyc
|            |—— __init__.cpython-310.pyc
|    |—— models.py
|    |—— serializers.py
|    |—— tests.py
|    |—— urls.py
|    |—— views.py
```
### Screenshots

TodoApi List: localhost:8000/api/
===
![Image text](https://github.com/jocnn/django_rest_todo/blob/main/scheenshots/List%20Todo%20%E2%80%93%20Todo.png)

TodoApi Detail: localhost:8000/api/1/
===
![Image text](https://github.com/jocnn/django_rest_todo/blob/main/scheenshots/Detail%20Todo%20-%20Todo.png)
