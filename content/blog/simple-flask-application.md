+++
author = "Praveen Kumar"
categories = ["flask", "python"]
date = 2019-09-25T18:50:00Z
description = "Creating new flask application in python 2 and as well as python 3"
featured = "flask-python.png"
featuredalt = ""
featuredpath = ""
linktitle = "Flask Application"
title = "Simple Flask Application"
type = "post"

+++
### Creating a new flask application.

When I came to know about the tech industry, I  was more of a frontend guy. I never knew about what is the backend, how would a backend work. My first backend application that ran successfully was a hello world app in a flask world. Why does someone need to pick python as their backed language? It is simple and more comfortable to learn. Working on python as a base language would ease you in many ways. Python community on the internet is pretty strong and supportive.

Starting a flask application is pretty simple. Anyone just needs 10 lines of code to start backend server. In this post, I am just going to show how could someone start the server.

**Step 1** Check for python installed in the system

    $ python --version
      Python 2.7.10 

**Step 2**Create a new project directory.

    $ mkdir flaskapp && cd flaskapp

**Step 3** Next step to create a virtual environment. Creating a virtual environment is important in flask application. The reason behind it simple, different project would require different dependency. We can explicitly maintain our project dependency only.

    $ pip insall virtualenv
    $ virtualenv -p flaskEnv
    $ source flaskEnv/bin/activate

**Step 4** After activating your virtual environment install flask.

    $ pip install flask

**Step 5** We have successfully drafted our base for running our flask application. Create an **_app.py_** file and write the following lines of code.

>     # app.py
>     from flask import Flask
>     import json
>     app = Flask(__name__)
>     
>     @app.route('/')
>     def hello_world():
>         return json.dumps({"hello": "world"})
>     
>     if __name__ == '__main__':
>         app.run()

My next post would address how we could structure our application so that anyone can use the boilerplate to start an application
