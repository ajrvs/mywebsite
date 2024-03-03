# mywebsite
Portfolio website using Django

## Setup and local execution:

- Clone the repo: `git clone https://github.com/ajrvs/mywebsite.git`
- Go to the project directory: `cd mywebsite`
- Run server: `python manage.py runserver`
- It will be running at Port 8000 (http://127.0.0.1:8000)

## Documentation

`virtualenv env`

`env\Scripts\activate`

`pip install django`

`django-admin startproject mywebsite .`

`python manage.py runserver`

`python manage.py startapp base`

add created app `base` in `INSTALLED_APPS` list in `settings.py`

create templates: `mywebsite/base/templates/base`

configure URL routing:
- create `urls.py` in the app dir `base`
- include this base urls (`mywebsite/base/urls.py`) in the main project `urls.py` (`mywebsite/mywebsite/urls.py`)

create static files

Update path of `STATIC_URL` in settings.py (if it's different than `static/`) and `STATICFILES_DIRS`

Make desired changes and run the server. Tweak and play!