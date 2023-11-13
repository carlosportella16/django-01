
# Introductory Module > Backend Development

## Python Environment for Development

- After downloading, within [Visual Studio Code](https://code.visualstudio.com/), execute the command to create and use the Python environment.

Command to create the development environment:

```
docker-compose build
```

Command to use the created development environment:

```
docker-compose up -d
```

## Running the Products API using the Django framework

Create the virtual environment

```
python -m venv ./venv
```

To activate the virtual environment

```
source venv/bin/activate
```

Install Django

```
pip install django
```

Create a txt file with the project dependencies

```
pip freeze > requirements.txt
```

To run the Django server

```
python manage.py runserver 0.0.0.0:8000
```

To create an app in Django

```
python manage.py startapp product
```

Create the migration of Django models in the database

```
python manage.py makemigrations
```

```
python manage.py migrate
```

Create a superuser for Django Admin

```
python manage.py createsuperuser
```