# CanteenManagementSystem
Vue.Js and Django Rest Framework

<h2>BACKEND (PYTHON DJANGO REST FRAMEWORK)</h2>
Setting up python environment:
- Install Python3
- Install pip
- python3 -m pip install --user virtualenv
- apt-get install python3-venv

Setting up virtual Environment:
- cd CanteenApp/backend
- python3 -m venv django
- source django/bin/activate

Installing Requirements:
- pip install -r requirements.txt 
- pip freeze //to verify the requirements installed or not.
  
Run server:
- python manage.py runserver

For deleting database, delete db.sqlite file inside backend direcory, 
- python manage.py migrate

For creating superuser:
- python manage.py createsuperuser

For adding new user manually without django user, password requirements:
- python manage.py shell
- from django.contrib.auth.models import User
- User.objects.create_user(username='abc', password='abc',first_name= 'abc',last_name='abc')



<h2>RONTEND (VUE CLI3)</h2>
Setting up environment:
- Install npm

Installing Packages and Dependencies:
- npm install

Run server:
- npm run serve
