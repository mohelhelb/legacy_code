## Web Application

### Description

This project is a simple blog-based web application built with Flask (Python web framework). It is CRUD compliant, that is to say it is a model that provides four basic types of functionalities: *Create*, *Read*, *Update*, and *Delete* posts. It also allows users to create an account as well as delete their existing one. Despite the fact that it is not a large application, *user authentication* has been carefully taken into account. This project is in progress in that there are a few features that are to be implemented, namely password recovery, change of credentials, software deployment, etc.

### Video Presentation

<img src="pyapp/static/images/presentation.gif" alt="Video Presentation" title="Flask-based Blog">


### Software tools

- Programming Language: Python 3.6+

- Web Framework: Flask 2.x

- CSS Framework: Bootstrap 4.3.x

- Dependencies: Please see the *requirements.txt* file.


### Setup

The steps that should be taken to set up this project are as follows:

- Clone the GitHub repository (preferably into */home/"user"/projects/*).
	~~~
	[mkdir -p ~/projects/]
	git clone git@github.com:mohelhelb/flask_blog_app.git [~/projects/flask_blog_app/]
	~~~
- Isolate the project by creating a virtual environment. 
	~~~ 
	pip install virtualenv 
	virtualenv ~/projects/flask_blog_app/venv/ 
	source ~/projects/flask_blog_app/venv/bin/activate 
	~~~ 
- Install the project's dependencies (See the *requirements.txt* file). 
	~~~ 
	pip install -r ~/projects/flask_blog_app/requirements.txt 
	~~~ 
- Launch Python in interactive mode and create a database.
	~~~
	cd ~/projects/flask_blog_app/
	~~~
	~~~
	Python 3.6.9 (default, Mar 15 2022, 13:55:28) 
	[GCC 8.4.0] on linux
	Type "help", "copyright", "credits" or "license" for more information.
	>>> 
	>>> from pyapp.hub import db
	>>> db.create_all()
	~~~
- Set and export the *FLASK_APP* environment variable.
	~~~
	export FLASK_APP="run_pyapp.py"
	~~~
- Execute the application.
	~~~
	flask run
	~~~
- Enter the IP address that is generated in the browser's search bar.
