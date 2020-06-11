title: Flask - Code a simple app |

# Flask - Code a simple web app

This tutorial aims to help beginners to start coding simple apps using Flask, the popular Python framework. Before reading or coding anything suggested in this tutorial, it might be a good idea to access the official Flask resources (docs, quickstart):

- [Flask](https://palletsprojects.com/p/flask/) - the official website
- [Flask Documentation](https://flask.palletsprojects.com/en/1.1.x/)

<br />

## [What is Flask](/what-is/flask/)

---

[Flask](https://palletsprojects.com/p/flask/) is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions.

Flask is a lightweight [WSGI](/what-is/wsgi/) web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications.

<br />

## Flask Installation

---

Being a framework coded in Python, Flask requires Python as a core dependency. The recommended version is the latest version of Python3.
To install [Python](https://www.python.org/), please access the official website and [download](https://www.python.org/downloads/) the proper version for your operating system.

- [Python for MacOS](https://www.python.org/downloads/windows/)
- [Python for Linux](https://www.python.org/downloads/source/)
- [Python for Windows](https://www.python.org/downloads/windows/)

If you are not sure if Python is installed, open a terminal window and type `python`.

```bash
$ python
Python 3.7.2 (tags/v3.7.2:9a3ffc0492, Dec 23 2018, 22:20:52) [MSC v.1916 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

This is the output information printed by Python, where we can check the current version - `3.7.2` for the above example.

<br />

> Install Flask

```bash
$ pip install flask
```

When Flask is installed, some core dependencies are also installed.

- *[Werkzeug](https://palletsprojects.com/p/werkzeug/)* implements WSGI, the standard Python interface between applications and servers.
- *[Jinja](https://palletsprojects.com/p/jinja/)* is a template language that renders the pages your application serves.
- *[MarkupSafe](https://palletsprojects.com/p/markupsafe/)* comes with Jinja. It escapes untrusted input when rendering templates to avoid injection attacks.
- *[ItsDangerous](https://palletsprojects.com/p/itsdangerous/)* securely signs data to ensure its integrity. This is used to protect Flask’s session cookie.
- *[Click](https://palletsprojects.com/p/click/)* is a framework for writing command-line applications. It provides the flask command and allows adding custom management commands.

<br />

> [Virtual environments](https://docs.python.org/3/tutorial/venv.html)

The goel of a [virtual environment](https://docs.python.org/3/tutorial/venv.html) is to manage the project dependencies, both in development and in production.

What problem does a virtual environment solve? The more Python projects you have, the more likely it is that you need to work with different versions of Python libraries, or even Python itself. Newer versions of libraries for one project can break compatibility in another project.

Using a virtual environment, we can safely isolate the app execution, without influencing the execution of other apps installed.

<br />

**Create a Virtual environment on Linux systems**

```bash
$ virtualenv env
$ source env/bin/activate
```

<br />

**Create a Virtual environment on Microsoft systems**

```bash
$ virtualenv env
$ .\env\Scripts\activate
```

<br />

If we install a package after a Virtual Environment activation, that package is available ONLY when the environment is active. If we try to access the dependency in a global scope (no virtual environment activated) we should get a `module not found` error.

<br />

> Install Flask using a Virtual Environment

```bash
$ # Create a working directory
$ mkdir my-project
$ cd my-project
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ pip install flask
```

<br />

> How to check Flask version or installation

**Via the Python interpreter**

```bash
$ # Open the Python console
$ python
>> import flask # if not installed, this line with generate an error
>> flask.__version__
'1.1.1' # <-- This is the current version
```

<br />

**Via `pip freeze` command**

```bash
$ # This works on Linux alike system - Windows don't have grep
$ pip freeze | grep flask
Flask==1.1.1 # <-- This is the current version
```

<br />

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

<br />

> What this code means

- Flask module is imported
- the app (WSGI compliant) is constructed by Flask
- a (default) route is defined that returns a friendly message to the user: `Hello from Flask`

When a request is received by our app, usually sent by the browser, the Flask core tries to match the path and execute the right handler.

<br />

> Execute our minimal app

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

> Resources

### Flask - [Jinja2 Theme](https://github.com/app-generator/theme-jinja2-coreui)

---

A super minimal Flask application provided as a template project for rendering UI themes converted to jinja. The app has no database, authentication or any other module that can confuse beginners and might be a good choice to start coding something simple in Flask.

- [Source code](https://github.com/app-generator/theme-jinja2-coreui)
- [LIVE Demo](https://github.com/app-generator/theme-jinja2-coreui)

<br />

### [Flask App Boilerplate](https://github.com/app-generator/boilerplate-code-flask)

---

A template project, coded on top of a nice UI kit, enhanced with an SQLite database, ORM, authentication - *app links*:

- [Source code](https://github.com/app-generator/boilerplate-code-flask)
- [LIVE Demo](https://boilerplate-code-flask.appseed.us/)

<br />

### [Flask Dashboard Boilerplate](https://github.com/app-generator/boilerplate-code-flask-dashboard)

---

A template project, coded on top of an admin dashboard UI kit, enhanced with an SQLite database, ORM, authentication - *app links*:

- [Source code](https://github.com/app-generator/boilerplate-code-flask-dashboard)
- [LIVE Demo](https://github.com/app-generator/boilerplate-code-flask-dashboard/)

<br />


> For support and more resources please access the [AppSeed](https://appseed.us) platform or join our community on [Discord](https://github.com/app-generator/boilerplate-code-flask-dashboard).
