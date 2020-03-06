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

# How to install the Bootstrap theme in your django app

1. Visit [startbootstrap site](https://startbootstrap.com/), select the theme you like for your project and download the zip file.
3. Go to the downloaded folder and unzip the bootstrap theme you just downloaded.
2. Create a new directory in your django project called 'static/'. Copy the files from the unzipped theme directory to the static directory you just created in your django project: css/, fonts/, js/, img/, scss/ vendor.
3. Create a new folder in your django directory called 'templates/'. Copy the index.html file from unzipped theme directory to the templates directory you just created.

