
# Introductory Module > Backend Development > Lesson 2

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

## Visual Studio Code

> If you already have Visual Studio Code installed on your operating system, it is not necessary to follow the steps below.

Here are the instructions for installing Visual Studio Code (VSCode) on different operating systems.

### Windows

1. Visit the official VSCode site at [https://code.visualstudio.com/](https://code.visualstudio.com/).
2. Click the download button for Windows.
3. Run the downloaded installer (usually called VSCodeSetup.exe).
4. Follow the installer's instructions, accepting the recommended defaults, such as file associations, unless you have specific preferences.
5. After installation, start Visual Studio Code from the Start menu or the desktop icon.

### macOS

1. Visit the official VSCode site at [https://code.visualstudio.com/](https://code.visualstudio.com/).
2. Click the download button for macOS.
3. Once the .dmg file is downloaded, open it.
4. Drag the Visual Studio Code icon to the "Applications" folder on your Mac.
5. Open VSCode from the "Applications" folder or the Dock.

### Linux

1. The simplest way to install Visual Studio Code on Debian/Ubuntu distributions is to download and install the .deb package (64-bit)
   [Debian or Ubuntu](https://code.visualstudio.com/download). If you use another distribution, [you can find the official documentation with explanations and step-by-step installation here](https://code.visualstudio.com/docs/setup/linux).

## Running the Products API using the Django framework

Access the fastapi-products directory

```
cd /referencial/src/django-produtos
```

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
python manage.py startapp produto
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