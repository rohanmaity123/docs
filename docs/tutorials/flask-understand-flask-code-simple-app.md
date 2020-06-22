title: Flask - Code a simple app

# [Flask](https://palletsprojects.com/p/flask/) - Code a simple web app

This tutorial aims to help beginners to start coding simple apps using Flask, the popular Python framework. Before reading or coding anything suggested in this tutorial, it might be a good idea to access the official Flask resources (docs, quickstart):

- [Flask](https://palletsprojects.com/p/flask/) - the official website
- [Flask Documentation](https://flask.palletsprojects.com/en/1.1.x/)

<br />

{!info-flask.md!}

{!env-settings.md!}

## Flask - a minimal app
---

The most simple app, coded in Flask, looks like this:

```python
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello from Flask!'
```

We save this source code in `hello.py`. The name is not important, but we will reference the file name in the next section of this tutorial.  

> **What this code means**

- Flask module is imported
- the app (WSGI compliant) is constructed by Flask
- a (default) route is defined that returns a friendly message to the user: `Hello from Flask`

When a request is received by our app, usually sent by the browser, the Flask core tries to match the path and execute the right handler.

> **Execute our minimal app**

```bash
$ export FLASK_APP=hello.py
$ flask run
 * Running on http://127.0.0.1:5000/
```

Please notice that export before we start the app using Flask development server. Flask itself should be informed (via the environment) what file should load and execute. In our sample is `hello.py`.

At this moment, we can visit the app in the browser, on port `5000`, the default port used by Flask to serve apps. To start the app on a different port, we must call Flask using `--port` argument.

```bash
$ export FLASK_APP=hello.py
$ flask run --port=9999
 * Running on http://127.0.0.1:9999/
```

This time, the app is started on port `9999`.

<br />

## Where to go from here
---

By accessing the [AppSeed](https://appseed.us) platform anyone, even without an account can access and use many Flask starters pre-built with a basic set of modules like authentication, database and deployment scripts.

### Flask - [Jinja2 Theme](https://github.com/app-generator/theme-jinja2-coreui)
---

A super minimal Flask application provided as a template project for rendering UI themes converted to jinja. The app has no database, authentication or any other module that can confuse beginners and might be a good choice to start coding something simple in Flask.

- [Source code](https://github.com/app-generator/theme-jinja2-coreui)
- [LIVE Demo](https://github.com/app-generator/theme-jinja2-coreui)

<br />

### [Flask App Boilerplate](/boilerplate-code/flask/)
---

A template project, coded on top of a nice UI kit, enhanced with an SQLite database, ORM, authentication - *app links*:

- [Source code](https://github.com/app-generator/boilerplate-code-flask)
- [LIVE Demo](https://boilerplate-code-flask.appseed.us/)

<br />

### [Flask Dashboard Boilerplate](/boilerplate-code/flask-dashboard/)
---

A template project, coded on top of an admin dashboard UI kit, enhanced with an SQLite database, ORM, authentication - *app links*:

- [Source code](https://github.com/app-generator/boilerplate-code-flask-dashboard)
- [LIVE Demo](https://github.com/app-generator/boilerplate-code-flask-dashboard/)

<br />

> For support and more resources please access the [AppSeed](https://appseed.us) platform or join our community on [Discord](https://github.com/app-generator/boilerplate-code-flask-dashboard).

