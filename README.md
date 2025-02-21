# python microblog app start all comands and flow

# https://pypi.org/ (python package manager) where you can search and use package from here

# https://flask.palletsprojects.com/en/stable/quickstart/  (flask quickstart)

--------------------------------------------------------
# 🔹 How to Install a Package?
The general syntax to install a package is:

pip install <package-name>

For example:

pip install flask
--------------------------------------------------------

This tutorial is designed for version 3 of Flask, but should also work with version 2.
The above command will install the latest 3.x version, which should be appropriate for most users.
If for any reason you prefer to follow this tutorial on a 2.x release of Flask,
you can use the following command to install the latest 1.x version:

(venv) $ pip install "flask<3" "werkzeug<3"

--------------------------------------------------------

#1 ===>
$ mkdir microblog (making microblog directory)
$ cd microblog (entering into microblog directory)
$ python -m venv venv (setting the environment in the project)

#2 ===> Now you have to tell the system that you want to use this virtual environment, and you do that by activating it.
If you are using a Microsoft Windows command prompt window, the activation command is slightly different:

$ venv\Scripts\activate
(venv) $ _
If you are on Windows but are using PowerShell instead of the command prompt, then there is yet another activation command you should use:

venv\Scripts\Activate.ps1
(venv) $ _


#2 ===> Now that you have a virtual environment created and activated, you can finally install Flask in it:

(venv) $ pip install flask

#3 ===> 
✅ app/ is a package that will store the Flask application.
✅ mkdir app creates the folder.
✅ __init__.py (to be added later) makes it an importable package.
✅ This structure helps organize the Flask app for larger projects.

#4 ===>
Flask(__name__) creates the Flask app
The __name__ variable helps Flask find resources (templates, static files).

#5 ===>

In most computers port 5000 is available, but there is a possibility that your computer is already running an application that uses this port, in which case the flask run command will fail with an "address already in use" or similar error. If you use a Macintosh computer, some versions of macOS run a service called "Airplay Receiver" on this port. If you are unable to figure out how to remove the software that uses port 5000, you can try running Flask on a different port. For example, here is how to start the server on port 5001:

(venv) $ flask run --port 5001

#6 ===>
1. Installing python-dotenv:
(venv) $ pip install python-dotenv
This installs a Python package called python-dotenv.
It allows Flask to automatically read environment variables from a file instead of you typing them in the terminal every time.

2. Creating the .flaskenv File:
.flaskenv: Environment variables for flask command

FLASK_APP=microblog.py
You’re creating a file named .flaskenv in your project’s main folder.
Inside it, you add:
FLASK_APP=microblog.py

#7 ===> 


