{% for _ in cookiecutter.project_name %}*{% endfor %}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}*{% endfor %}

{{ cookiecutter.project_description }}

Getting Started
===============

Prerequisites
-------------

* Python >= 3.6.0 <https://docs.python.org/3/index.html>
* Postgres >= 10.0 <https://www.postgresql.org/docs/>

Installing
----------

1. Create the database and the virtual environment. We recommend using `virtualenvwrapper <http://virtualenvwrapper.readthedocs.io/en/latest/index.html>`_.

2. Create an .env file and set variables. Examples can be found in :code:`.env.example`.

3. Setup the environment:

   .. code-block:: bash

      $ pip install -r requirements.txt
      $ python manage.py migrate

4. Start the server:

   .. code-block:: bash

      $ python manage.py runserver

The site will be available on <http://localhost:8000> or <http://127.0.0.1:8000>.

Deploy
======

TODO

Translations
============

Example of how to make messages for spanish (es):

   .. code-block:: bash

      $ django-admin makemessages --locale=es

Django translations should be compiled automatically during the deployment. If
you want to compile messages, use the compilemessages command:

   .. code-block:: bash

      $ django-admin compilemessages --locale=es

Tests
=====

TODO
