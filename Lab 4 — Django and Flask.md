## Lab 4 — Django and Flask
## Create Django Project
```
> django-admin startproject stevens
> cd stevens 
```

## Create and enter python virtual environment
```
stevens> py -m venv env
stevens> .\Scripts\activate
(env) stevens> pip install django
```

## Create Django app
```
(env) stevens> cd stevens
(env) stevens> py manage.py startapp myapp
```

## Copy needed files and create directories
```
(env) stevens> cp ..\urls.py .
(env) stevens> cd myapp
(env) stevens\myapp> cp ../../admin.py .
(env) stevens\myapp> cp ../../models.py .
(env) stevens\myapp> cp ../../views.py .
(env) stevens\myapp> mkdir static templates
(env) stevens\myapp> cd templates
(env) stevens\myapp\templates> mkdir myapp
(env) stevens\myapp\templates> cd myapp
(env) stevens\myapp\templates\myapp> cp ..\..\..\..\index.html .
```
## Run application:
![Screenshot 2023-05-01 112353](https://user-images.githubusercontent.com/32028457/236642446-4e9b5ae9-e138-436a-99c0-02d36a69bebe.png)

## Do similar things for mycpu
![image](https://user-images.githubusercontent.com/32028457/236644158-c35bfd6d-e4e1-45e9-92df-9944e59d9f66.png)

## pip install flask and run hello_world
![image](https://user-images.githubusercontent.com/32028457/236644251-77a105a7-e64d-470a-8f7b-97aaf804c7f3.png)

