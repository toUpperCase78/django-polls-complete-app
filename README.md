# Django Polls - Complete App

**The completed web polls application with Python Django from tutorials**

![Django Polls](polls/static/polls/images/django_polls_logo.png)

## Overview

**Django** is one of the well-known and high-level Python web framework for rapid development and clean, pragmatic design. It takes care many steps of the web development, enabling to focus on writing applications without requiring to reinvent something. Moreover, Django is popular by being free and open-source.

This repository contains the files which correspond to the web polls application and all parts of the tutorial, which are available in Django's [official documentation](https://docs.djangoproject.com/en/5.1/), were followed to get the application working as intended and make it fully functional. Notice that there is a main project called ``mysite`` and inside, the ``polls`` application is available.

After the completion of this tutorial, I've implemented a few more things to present a much better design; such as different font in all pages, a static logo image that appears at the top, green buttons, table structure in poll results...

_The polls application was developed with Django version 5.1._

## Usage

Go to the directory where ``manage.py`` is available, and in the command prompt or terminal screen, type ``python manage.py runserver``.

When the server is up, then go to ``http://localhost:8000/polls/`` which is the main page and the starting point of web polls application. You should see several poll questions created already...

Try clicking one of the questions, select an option and click the Vote button. There should be the poll results page for how many votes have been given so far for the question. After that, you may vote again or move to another question.

### Administration Panel

To access the administration panel, go to ``http://localhost:8000/admin/`` and enter these credentials:

```
Username: doganyigityenigun
Password: django123456
```

There, you should see the ``Questions`` model and when you click on it, all the created questions will appear. Here, you can add a new question, define the corresponding choices. In the meantime, you can alter the existing questions and their choices and vote counts as you wish.

Keep in mind that the application only shows up to 5 questions in the main page, ordered by the publication date. Additionally, the questions from the future date will not appear in the poll list until it has been reached with the real date.

## Screenshots

The screenshots below could give an idea of which pages will be encountered throughout the web polls application.

![Django Polls SS1](/Screenshots/django_polls_web(1).png)

![Django Polls SS2](/Screenshots/django_polls_web(2).png)

![Django Polls SS3](/Screenshots/django_polls_web(3).png)

## Details

There are many files and directories to properly operate the project and the web polls application itself.

**The root directory**

* ``manage.py``: The command-line utility for interacting with the Django project in various ways.
* ``db.sqlite3``: The database file to store the questions, choices and their related vote counts. Note that this app is using the default SQLite database system.

**``mysite`` directory**

* ``__pycache__``: This directory stores the compiled bytecode of imported modules within ``mysite``.
* ``__init__.py``: An empty file to tell Python that this directory should be considered as a Python package.
* ``asgi.py``: An entry point for ASGI-compatible web servres to serve the project.
* ``settings.py``: Settings and configurations for this Django project.
* ``urls.py``: The URL declarations for this Django project; think of it as a table of contents of this Django-powered site.
* ``wsgi.py``: An entry point for WSGI-compatible web servers to serve the project.

**``polls`` directory**

* ``__pycache__``: This directory stores the compiled bytecode of imported modules within ``polls``.
* ``migrations\0001_initial.py``: The details about the changes of the defined models are presented here; created after executing ''makemigrations``.
* ``static\polls``: This directory holds the static files (e.g. CSS, JavaScript methods, images).
* ``template\polls``: This directory contains the HTML page templates (with some Python code blocks) that correspond to the views for rendering (total of 3 pages).
* ``__init__.py``: An empty file to tell Python that this directory should be considered as a Python package.
* ``admin.py``: The customizations of polls administration page are contained here (items to display, filters, search fields, inlines).
* ``apps.py``: The application file for ``polls`` to be registered as installed app for the project.
* ``models.py``: The models and their attributes (fields) inside are implemented here; can contain additional self methods and foreign keys.
* ``tests.py``: Several test methods for ``Question`` model and ``Index`` view to make sure the application is working as expected by simulating user behaviors.
* ``urls.py``: The URL declarations for the web polls app, bound to their views. Currently, the generic views are being used for rendering pages.
* ``views.py``: The structures of all views are written here. Currently, the generic views are adopted for the purpose of less coding. In addition, there is also ``views_old1.py`` file that represents the traditional version of these views.

**``templates\admin`` directory**

This directory contains two files ``base_site.html`` and ``index.html`` in order to alter the structure of the admin pages. These were taken from the Django's source files. Only the title was changed to ``Polls Administration``.
