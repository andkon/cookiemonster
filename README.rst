cookiecutter-django
=======================

.. image:: https://requires.io/github/pydanny/cookiecutter-django/requirements.svg?branch=master
     :target: https://requires.io/github/pydanny/cookiecutter-django/requirements/?branch=master
     :alt: Requirements Status

.. image:: https://travis-ci.org/pydanny/cookiecutter-django.svg?branch=master
     :target: https://travis-ci.org/pydanny/cookiecutter-django?branch=master
     :alt: Build Status

.. image:: https://badges.gitter.im/Join Chat.svg
   :target: https://gitter.im/pydanny/cookiecutter-django?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge


A Cookiecutter_ template for Andrew.

Customizations
--------------

* Options for css
* Some hints for best practices

Usage
------

Let's pretend you want to create a Django project called "redditclone". Rather than using `startproject`
and then editing the results to include your name, email, and various configuration issues that always get forgotten until the worst possible moment, get cookiecutter_ to do all the work.

First, get cookiecutter. Trust me, it's awesome::

    $ pip install cookiecutter

Now run it against this repo::

    $ cookiecutter https://github.com/andkon/cookiemonster

You'll be prompted for some questions, answer them, then it will create a Django project for you.


**Warning**: After this point, change 'Daniel Greenfeld', 'pydanny', etc to your own information.

**Warning**: repo_name must be a valid Python module name or you will have issues on imports.

It prompts you for questions. Answer them::

    Cloning into 'cookiecutter-django'...
    remote: Counting objects: 550, done.
    remote: Compressing objects: 100% (310/310), done.
    remote: Total 550 (delta 283), reused 479 (delta 222)
    Receiving objects: 100% (550/550), 127.66 KiB | 58 KiB/s, done.
    Resolving deltas: 100% (283/283), done.
    project_name [project_name]: Reddit Clone
    repo_name [Reddit_Clone]: reddit
    author_name [Your Name]: Daniel Greenfeld
    email [Your email]: pydanny@gmail.com
    description [A short description of the project.]: A reddit clone.
    domain_name [example.com]: myreddit.com
    version [0.1.0]: 0.0.1
    timezone [UTC]:
    now [2015/11/22]: 2015/11/22
    year [2015]:
    use_whitenoise [y]: n
    use_celery [n]: y
    use_mailhog [n]: n
    use_sentry [n]: y
    use_newrelic [n]: y
    use_opbeat [n]: y
    windows [n]: n
    use_python2 [n]: y


Enter the project and take a look around::

    $ cd reddit/
    $ ls

Create a GitHub repo and push it there::

    $ git init
    $ git add .
    $ git commit -m "first awesome commit"
    $ git remote add origin git@github.com:pydanny/redditclone.git
    $ git push -u origin master

Now look at your repo, and hit the Deploy to Heroku button!
