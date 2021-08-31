## Django Custom User Model 

    Django ships with a built-in User model for authentication and if you'd like a basic tutorial on how to implement log in, log out, sign up and so on see the Django Login and Logout tutorial for more.
    However, for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

## Setup 

    -   create and navigate into a dedicated directory called accounts for our code
    -   install Django
    -   make a new Django project called config
    -   make a new app accounts
    -   start the local web server

```
$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ pipenv install django~=3.1.0
$ pipenv shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver
```

## Creating our initial custom user model requires four steps:

    -   update config/settings.py
    -   create a new CustomUser model
    -   create new UserCreation and UserChangeForm
    -   update the admin


