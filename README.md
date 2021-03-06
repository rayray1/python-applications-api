# Python Applications API

A small RESTful API python applications api that allows uploading and listing
android applications.

## Features

* Django 2.0 and Python 3.6
* Django-rest-framework
* Pipenv for virtualenvs

## First-time setup

1.  Make sure Python 3.6x and Pipenv are already installed
2.  Clone the repo and configure the virtualenv

```
git clone https://github.com/rayray1/python-applications-api.git
cd python-applications-api
pipenv install
pipenv shell
```

3.  Set up the initial migration and build the database

```
python manage.py makemigrations applications
python manage.py migrate
```

4.  Confirm everything is working

```
python manage.py runserver
```

Load the site at http://127.0.0.1:8000/api/applications


# DOCKER

To run api application with docker

```
cd python-applications-api
docker-compose build
docker-compose up
```

## Docker Recommendations

* If using docker on windows remember to add ip hostname to allowed hosts on settings

![](media/screenshot.png)
<!-- ![screenshot](media/screenshot.png) -->
