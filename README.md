# CanteenManagementSystem
Vue.Js and Django Rest Framework

<h3>BACKEND (DJANGO REST FRAMEWORK)</h3>

<strong>Setting up python environment:</strong>
- Install Python3
- Install pip
- python3 -m pip install --user virtualenv
- apt-get install python3-venv

<strong>Setting up virtual Environment:</strong>
- cd CanteenApp/backend
- python3 -m venv django
- source django/bin/activate

<strong>Installing Requirements:</strong>
- pip install -r requirements.txt 
- pip freeze //to verify the requirements installed or not.
  
<strong>Run server:</strong>
- python manage.py runserver

<strong>For deleting database, delete db.sqlite file inside backend direcory,</strong>
- python manage.py migrate

<strong>For creating superuser:</strong>
- python manage.py createsuperuser

<strong>For adding new user manually without django user, password requirements:</strong>
- python manage.py shell
- from django.contrib.auth.models import User
- User.objects.create_user(username='abc', password='abc',first_name= 'abc',last_name='abc')



<h3>FRONTEND (VUE.JS)</h3>

<strong>Setting up environment:</strong>
- Install npm

<strong>Installing Packages and Dependencies:</strong>
- npm install

<strong>Run server:</strong>
- npm run serve
