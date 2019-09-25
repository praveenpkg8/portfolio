+++
author = "Praveen Kumar"
categories = ["flask", "python"]
date = "2019-09-25T18:50:00+00:00"
description = "Creating new flask application in python 2 and as well as python 3"
featured = "/img/09/flask-python.png"
featuredalt = ""
featuredpath = ""
linktitle = "Flask Application"
title = "Simple Flask Application"
type = "post"

+++
### Creating a new flask applicaion.

**Step 1** Check for python installed in the system

    $ python --version
      Python 2.7.10 

**Step 2**Create a new project directory.

    $ mkdir flaskapp && cd flaskapp

**Step 3** Next step create a virtual environment. Creating a virtual environment is important in flask application. Reason behind it simple, different project would require different dependency. We can explicitly maintain our project dependency only.

    $ pip insall virtualenv
    $ virtualenv -p flaskEnv
    $ source flaskEnv/bin/activate

**Step 4** After activating your virtual environment install flask.

    $ pip install flask

**Step 5** We have successfully drafted our base for running our flask application. Create a **_app.py_** file and write the following lines of code.

    # app.py
    from flask import Flask
    import json
    app = Flask(__name__)
    
    @app.route('/')
    def hello_world():
        return json.dumps({"hello": "world"})
    
    if __name__ == '__main__':
        app.run()