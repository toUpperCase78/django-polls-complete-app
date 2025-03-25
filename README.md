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

Details about each file will be shared at a later time.
