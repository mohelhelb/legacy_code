## Web Application

### Description

This project is a simple blog-based web application built with Flask (Python web framework). It allows users to create an account as well as delete their existing one. It is also CRUD compliant, that is to say it is a model that provides four basic types of functionalities: *Create*, *Read*, *Update*, and *Delete* posts. Despite the fact that it is not a large application, *user authentication* has been carefully taken into account. It is also worth mentioning that this project is in progress; there are a few features that are to be implemented, namely password recovery, change of credentials, software deployment, etc.

### Video Presentation

<img src="pyapp/static/images/presentation.gif" alt="Video Presentation" title="Flask-based Blog">


### Software tools

- Programming Language: Python 3.6+

- Web Framework: Flask 2.x

- CSS Framework: Bootstrap 4.3.x

- Dependencies: Please see the *requirements.txt* file.


### Setup

The steps that should be taken to set up this projects are as follows:

- Clone the GitHub repository (preferably into */home/"user"/projects/*).
        ```
        [mkdir -p ~/projects/]
        git clone git@github.com:mohelhelb/flask_blog_app.git [~/projects/flask_blog_app/]
        ```
- Isolate the project by creating a virtual environment. 
        ``` 
        pip install virtualenv 
        virtualenv ~/projects/flask_blog_app/venv/ 
        source ~/projects/flask_blog_app/venv/bin/activate 
        ``` 
- Install the project's dependencies (See the *requirements.txt* file). 
        ``` 
        pip install -r ~/projects/flask_blog_app/requirements.txt 
        ``` 
- Launch Python in interactive mode and create a database.
	```
	cd ~/projects/flask_blog_app/
	```
	```
	python
	>>> from pyapp.hub import db
	>>> db.create_all()
	```
- Set and export the *FLASK_APP* environment variable.
	```
	export FLASK_APP="run_pyapp.py"
	```
- Execute the application.
	```
	flask run
	```
- Enter the IP address on the Internet browser.
