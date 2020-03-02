# How-to

You can find quick guidelines on <b> how-to </b> start on the project or fix technical issues. I will list all the issues that I came across while building this web application and the potential solutions to solve them.

Virtual environment
```
# create a virtual environment
python3 -m venv name_of_virtual_env

# activate a virtual environment
source name_of_virtual_env/bin/activate
```

Django installation
```
# install django
pip install django

# check django version installed in your system
python3 -m django --version
```

Create Django project
```
django-admin startproject mysite
```

Create a Portfolio app
```
# cd into mysite directory, you will see manage.py file
python3 manage.py startapp portfolio
```

Run your development server
```
python3 manage.py runserver
```


Create Model and Register your app
```
# define models in your application. In our project, we will define models in file located in::
# mysite/portfolio/models.py file

# Register your app in settings file in your project. In our project, we will register portfolio app in setting file located in:
# mysite/mysite/settings.py
```

Install libraries to work with image uploading in your app.
note: You can skip this step if you are not going to work with images.
```
pip install pillow
```

Make migrations
```
# Run migrations command to create migrations for above changes
python3 manage.py makemigrations portfolio

python3 manage.py migrate
```