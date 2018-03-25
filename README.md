# django1
Test polls project to get to grips with working on Django

## Django development notes

### On Solus Linux
* Install virtualenv
* Create new virtual environment by running ```virtualenv -p python3 NAME``` where NAME is what you want to call the environment. The -p argument lets you specify which version of python to use.
* Activate the virtual environment by typing ```source bin/activate```
* Install any dependencies you need, including Django ```pip install Django==2.0.3```
* Next ```cd``` into the new directory and create a directory for your code / projects ```mkdir NAME```.
* In your code / projects folder, run ```django-admin startproject NAME```
* After you're finished, end the virtual environment by typing ```deactivate```
* For easier Django development, run ```alias rs="python manage.py runserver"```

### On Windows 10
Sidenote: using virtualenv on Windows seems rrrrrrreaallllyyyyy slow - be prepared to twiddle your thumbs during processes

* Install Python3 if not already present
* Install virtualenv using pip: ```pip install --trusted-host pypi.python.org virtualenv```
  * User guide is here: https://virtualenv.pypa.io/en/stable/userguide/
  * Need to use the trusted host argument otherwise there's an error - more info here: https://stackoverflow.com/questions/25981703/pip-install-fails-with-connection-error-ssl-certificate-verify-failed-certi
* To start a dev environment, open cmd in host folder and then type ```virtualenv NAME``` where NAME is the name of the project environment. Call it whatever you like.
* Activate the dev environment by typing ```Scripts\activate```
* Next, install Django inside the environment: ```pip install --trusted-host pypi.python.org Django==2.0.3```
* Make a directory for your code ```mkdir NAME```
* ```cd projects```
* To create a sample Django app called *mysite*: ```django-admin startproject mysite```

This isn't the end goal, it's just an example site so I can walk through the tutorial (https://docs.djangoproject.com/en/2.0/intro/tutorial01/)

I'm going to follow the tutorial as closely as possible just to get back into the swing of things.

The project generated successfully. The dev server can be activated by running ```python manage.py runserver``` but again, it's very slow - much slower than I've noticed before. I can only chalk this up to the virtualenv environment.

##########
    Change your models (in models.py).
    Run python manage.py makemigrations to create migrations for those changes
    Run python manage.py migrate to apply those changes to the database.
##########

Current progress:
https://docs.djangoproject.com/en/2.0/intro/tutorial03/#write-views-that-actually-do-something
