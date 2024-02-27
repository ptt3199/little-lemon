# Backend course by meta
Noted and changed to my own understanding and style.

-> Aim to create a cookiecutter template for django project
## Setup a django project
### 1. Setup poetry
To keep the .venv folder in the project directory, create a poetry config file: `poetry.toml`
```bash
[virtualenvs]
in-project = true
path = ".venv"
```
Run init 
```bash
poetry init
```

### 2. Add django and other packages to the project
```bash
poetry add django
```
### 3. Create a django project
```bash
django-admin startproject LittleLemon .
```
### 4. Start app and run all the migrations
```bash
python manage.py startapp LittleLemonAPI
python manage.py migrate
```

## Run the server
```bash
python manage.py runserver 8001
```