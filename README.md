# CRUD-on-Django-Query-Spanning-Relationships
### Runnable either on IBM Cloud or in VS Code Standalone, database using Postgres (Cloud or local standalone)

## Go to Project folder
- pip install --upgrade distro-info
- pip3 install --upgrade pip==23.2.1 replace with python.exe -m pip install --upgrade pip==23.3.1 --user
- wget "https://______/IBM-CD0251EN-SkillsNetwork/labs/m3_django_orm/lab3_template.zip"  
replace with 
- wget -O Downloads/lab3_template.zip "https://_____/IBM-CD0251EN-SkillsNetwork/labs/m3_django_orm/lab3_template.zip"
Conduct wget -O outside project folder
_The zip file will be in 'Downloads' folder outside/before project folder_
- unzip lab3_template.zip
- rm lab3_template.zip _(remove if necessary)_

## Go to specific project Folder & build Django environment
- cd/project/lab2_template
## Setup Django Environment inside the specific project's directory

- pip install virtualenv
- pip install django
- virtualenv djangoenv replace with python -m venv djangoenv
- source djangoenv/bin/activate replace with .\djangoenv\Scripts\activate
- pip install Django psycopg2-binary
- python3 manage.py makemigrations crud replace with python manage.py makemigrations crud
- python3 manage.py migrate replace with python manage.py migrate

## Migration
In Django environment remember to migrate to python3 manage.py migrate for several major Python .py changes
- python3 manage.py makemigrations related_objects replace with python manage.py makemigrations related_objects
- python3 manage.py migrate replace with python manage.py migrate

## Should be showing:
Operations to perform:
  Apply all migrations: related_objects
Running migrations:
  Applying related_objects.0001_initial... OK

- python3 write.py

## should be showing:
Course objects saved... 
Instructors objects saved...
Learners objects saved...
Lessons objects saved...
Course-instructor relationships saved... 
Course-learner relationships saved...
