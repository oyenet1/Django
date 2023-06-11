# Django Tutorial

## Steps

### 1. Install python and all it's environments. Check whether python and pip is install on your system run

```bash
python --version
and
pip --version
```

### 2. It is suggested to have a dedicated virtual environment for each Django project, and one way to manage a virtual environment is venv, which is included in Python. To check if the virtual environments is already installed type the following command

```bash
# for window
py -m venv yourEnvName

#for mac or unix system
python -m venv yourEnvName
```

#### This will set up a virtual environment, and create a folder named "yourEnvName"

#

#### To install the virtual environment if not already installed, type the following command

```python
pip install virtualenv
```

or

```python
python -m instll virtualenv
```

- Then you have to activate the environment, by typing this command:

```sh
# window
yourEnvName\Scripts\activate.bat
```

or

```bash
# for mac or unix system
source yourEnvName/bin/activate
```

### 3: Install Django project and App

- _**Note:** ` Remember to install Django while you are in the virtual environment!`_

Before install you can check whether django is installed or not by running

```sh
django-admin --version
```

To install Django type the following command

```sh
# Windows
py -m pip install Django
```

```sh
# Mac or unix system
python -m pip install Django
```

To create a project run

```sh
# Windows
django-admin startapp appname
```

To create an app run

```sh
# window
py manage.py startapp appname
```

```sh
# For Mac or unix system
python manage.py startapp appname
```

- To start Django project run

```sh
# Mac or unix system
python manage.py runserver
```

```sh
#to run on different port other than 8000 add port bumber to it
python manage.py runserver 8080
```

<center>and</center>

```sh
# Window
py manage.py runserver
```

## Routing(Request and Response)

To add a view goto the views file inside your newly created app folder and replace the text inside to

```py
from django.shortcuts import render
from django.http import HttpResponse


def members(request):
    return HttpResponse("Hello world!")
```

`members here is a function, it can be anything`
Create a file called _`urls.py`_ in the same folders as _`views.py`_ and typed the following code

```py
from django.urls import path
from . import views

urlpatterns = [
    path('members/', views.members, name='members'),
]
```
