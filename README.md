# Django-tutorial
My repository for the official Django tutorial 

https://docs.djangoproject.com/en/6.0/intro/

The following notes are written for my own sake. 

Part 1:

Rather than installing Django directly to my computer, I am using Pipenv and running Django inside my project's virtual environment. 

sudo pacman -S python-pipenv

I created this Django-tutorial repository on Github, cloned it to my computer, then navigated to the directory. All of these commands are being run from inside this Django-tutorial directory.

pipenv install # Initialize Pipenv environment
pipenv shell # Opens a shell in the virtualenv
pipenv install django # Installs Django in the virtual environment and adds Django to the Pipfile
pipenv lock # Creates the Pipfile.lock file

This line bootstraps the new project:
django-admin startpoint mysite djangotutorial

^ This created the djangotutorial directory with a project called mysite inside.


/more notes that I'm not taking/



Part 2: Set up the database, create my first model, and learn about Django's automatically-generated admin site.

three-step guide to making model changes:

    Change your models (in models.py).

    Run python manage.py makemigrations to create migrations for those changes

    Run python manage.py migrate to apply those changes to the database.



Part 3: Focus on creating the public interface - "views".

A view is a "type" of web page in your Django application that generally serves a specific function and has a specific template
E.g. (for a blog application): homepage view, entry "detail" view, year/month/day-based archive view, etc.


Part 4: Focus on form processing and cutting down our code.

