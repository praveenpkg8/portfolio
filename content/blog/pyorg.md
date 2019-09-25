+++
author = "Praveen Kumar"
categories = ["google app engine", "flask", "python"]
date = "2019-09-24T18:30:00+00:00"
description = "Ultimate savior for hosting your Flask Python Application in Google App Engine "
featured = ""
featuredalt = ""
featuredpath = ""
linktitle = ""
title = "Python APP in Google App Engine"
type = "post"

+++
# **How to run a python flask app in google app engine ?**

  
It was easy for me to design and implement a python flask application. I always don't know what to do next. I used to scratch my head, how am I going to host it. How can I give the link to some one, so that I can boast that it was done by me.

Lets us start from the scratch. A simple hello world application is our ultimate choice to check some thing out for the first time.

Buckle up friends we are going to start a journey.

> ##### what is flask ? 
>
> Flask is a lightweight [WSGI](https://wsgi.readthedocs.io/) web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around [Werkzeug](https://palletsprojects.com/p/werkzeug) and [Jinja](https://palletsprojects.com/p/jinja) and has become one of the most popular Python web application frameworks. \[to know more\]([http://flask.palletsprojects.com/en/1.1.x/](http://flask.palletsprojects.com/en/1.1.x/ "http://flask.palletsprojects.com/en/1.1.x/"))

#### lets create a simple hello world application in **flask using  python.X** ?

Flask really done care about what python version we are using. Then Where does the problem lies in ?.  

The Culprit here is Google App Engine. For Google App Engine it really matters what python version we are using. Whether Python3 or Python2.  

> The Article is split in to two section. **First section is for Python 2** and guess what **Second section for Python 3.**

***

### Creating a new flask applicaion. 

**Step 1** Check for python installed in the system

    $ python --version
      Python 2.7.10 

**Step 2**Create a new project directory.

    $ mkdir flaskapp && cd flaskapp

**Step 3** Next step create a virtual environment