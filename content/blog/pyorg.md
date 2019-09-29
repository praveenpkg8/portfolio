+++
author = "Praveen Kumar"
categories = ["google app engine", "flask", "python"]
date = "2014-09-28"
description = "Ultimate savior for hosting your Flask Python Application in Google App Engine "
featured = "pic03.jpg"
featuredalt = "Pic 03"
featuredpath = "date"
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

## Creating a Simple flask application.

> Hola, I have Just wrote a separate article about it check that out \[here\]([https://praveenpkg.netlify.com/blog/simple-flask-application/](https://praveenpkg.netlify.com/blog/simple-flask-application/ "here")

## Before you begin with GAE

1. To set up your Google Cloud Platform project, use the GCP Console:
   1. Create a GCP project, create an App Engine app, and then enable billing in that project.  
      [GO TO APP ENGINE](https://console.cloud.google.com/projectselector/appengine/create?lang=flex_python&st=true&_ga=2.181341410.-470095340.1568349525)

      When prompted, select the [region](https://cloud.google.com/appengine/docs/locations) where you want your App Engine app located, and then enable billing. After your GCP project is created, the **Dashboard** opens.
   2. Enable the Cloud Datastore, Cloud Storage JSON and Cloud SQL Admin APIs.

      [ENABLE THE APIS](https://console.cloud.google.com/flows/enableapi?apiid=datastore.googleapis.com,datastore,storage_api,sqladmin.googleapis.com&redirect=https://console.cloud.google.com&_ga=2.181341410.-470095340.1568349525)
2. Download, install, and initialize the Cloud SDK.  
   [DOWNLOAD THE CLOUD SDK](https://cloud.google.com/sdk/docs/)
3. Acquire local credentials for authenticating with GCP services.

       $ gcloud auth application-default login
4. Verify that your default project is correct.

       $ gcloud config list

   If the project ID listed in the output isn't the project that you intended to use for this tutorial, set the project.

       gcloud config set project [YOUR_PROJECT_ID]

   where `[YOUR_PROJECT_ID]` is the ID of the project that you created or chose to use for this tutorial.