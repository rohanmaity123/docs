title: Flask Dashboard Light

# [Flask Dashboard Light](https://appseed.us/admin-dashboards/flask-dashboard-light-bootstrap)

**Open-Source Admin Dashboard** coded in **[Flask Framework](https://palletsprojects.com/p/flask/)** - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

## Dashboard Features
---

- SQLite database
- SQLAlchemy ORM
- Session-Based authentication flow (login, register)
- UI Kit: **Light Bootstrap Dashboard** (Free version) provided by **Creative-Tim**

<br />

## Dashboard technology stack
---

- Used Language: [Python3](https://www.python.org/) (Python2 is not supported)
- Web Framework: [Flask](https://www.palletsprojects.com/p/flask/)
- CSS Framework: [Bootstrap CSS](https://getbootstrap.com/)
- Javascript: [jQuery](https://jquery.com/)

<br />

## Dashboard Links
---

- [Flask Dashboard Light](https://appseed.us/admin-dashboards/flask-dashboard-light-bootstrap) - the product page
- [Flask Dashboard Light](https://github.com/app-generator/flask-dashboard-light-bootstrap) - the source code
- [Flask Dashboard Light](https://flask-dashboard-light.appseed.us/login.html) - LIVE Demo

![Flask Dashboard Light - Open-Source Admin Panel](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-light-bootstrap-screen.png)

<br />

## Prepare your environment
---

The product is built on top of [Flask](https://palletsprojects.com/p/flask/), a popular Python Web Framework. To build the app, Python3 should be installed properly in the workstation. If you are not sure if Python is properly installed, please open a terminal and type `python --version`. The full-list with dependencies and tools required to build the app:

- [Python3](https://www.python.org/) - the programming language used to code the app
- [Git](https://git-scm.com/) - used to clone the source code from the Github repository
- A [Github](https://github.com/) account - the invitation to the source code, will be sent on your account.
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment. 

For more information on how to set up your environment please access the resources listed below. In case we've missed something, contact us on Discord.

- [How to set up Python](/how-to/install-python)
- [Setup CentOS for development](/how-to/setup-centos-for-development/)
- [Setup Ubuntu for development](/how-to/setup-ubuntu-for-development/)
- [Setup Windows for development](/how-to/setup-windows-for-development/)

<br />

## Project Structure
---

The boilerplate code is built with a modular structure that follows the recommended pattern used by many open-source projects. The most important files and  directories are shown below:

<br />

```bash
< PROJECT ROOT >                          # application root folder
    |
    |--- app/__init__.py                  # application constructor  
    |--- app//assets                      # Img, CSS, Janascript files
    |--- app/templates                    # Jinja2 files
    |            |---<includes>           # Page chunks, components
    |            |---<layouts>            # Layouts
    |            |---<pages>              # Pages
    |                |---- index.html     # Main dashboard page
    |                |---- login.html
    |                |---- register.html
    |                |---- tables.html
    |                |---- notifications.html
    |
    |--- requirements.txt                 # Modules and dependencies
    |
    |--- run.py                           # bootstrap the app
    |
    |-----------------------------
```

<br />

## How to use it
---

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/flask-dashboard-light-bootstrap.git
$ cd flask-dashboard-light-bootstrap
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv --no-site-packages env
$ # .\env\Scripts\activate
$ 
$ # Install requirements
$ pip3 install -r requirements.txt
$
$ # Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=run.py
$ (Windows) set FLASK_APP=run.py
$ (Powershell) $env:FLASK_APP = ".\run.py"
$
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$ # (Windows) set FLASK_ENV=development
$ # (Powershell) $env:FLASK_ENV = "development"
$
$ # Run the application
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the app in browser: http://127.0.0.1:5000/
```

<br />

## Deployment
---

The app is provided with a basic configuration to be executed in [Docker](https://www.docker.com/), [Gunicorn](https://gunicorn.org/), and [Waitress](https://docs.pylonsproject.org/projects/waitress/en/stable/).

<br />

### [Docker](https://www.docker.com/) execution
---

The application can be easily executed in a docker container. The steps:

> Get the code

```bash
$ git clone https://github.com/app-generator/flask-dashboard-light-bootstrap.git
$ cd flask-dashboard-light-bootstrap
```

> Start the app in Docker

```bash
$ sudo docker-compose pull && sudo docker-compose build && sudo docker-compose up -d
```

Visit `http://localhost:5005` in your browser. The app should be up & running.

<br />

### [Gunicorn](https://gunicorn.org/)
---

Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX.

> Install using pip

```bash
$ pip install gunicorn
```
> Start the app using gunicorn binary

```bash
$ gunicorn --bind 0.0.0.0:8001 run:app
Serving on http://localhost:8001
```

Visit `http://localhost:8001` in your browser. The app should be up & running.


<br />

### [Waitress](https://docs.pylonsproject.org/projects/waitress/en/stable/)
---

Waitress (Gunicorn equivalent for Windows) is meant to be a production-quality pure-Python WSGI server with very acceptable performance. It has no dependencies except ones that live in the Python standard library.

> Install using pip

```bash
$ pip install waitress
```
> Start the app using [waitress-serve](https://docs.pylonsproject.org/projects/waitress/en/stable/runner.html)

```bash
$ waitress-serve --port=8001 run:app
Serving on http://localhost:8001
```

Visit `http://localhost:8001` in your browser. The app should be up & running.

<br />

## App screens
---

> User Profile Page

![Light Bootstrap Dashboard - User Profile Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-light-bootstrap-screen-1.png)

> UI Notifications

![Light Bootstrap Dashboard - Typography Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-light-bootstrap-screen-2.png)

> UI Typography

![Light Bootstrap Dashboard - Maps Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-light-bootstrap-screen-3.png)

<br />

## Links & Resources
---

### [Flask Framework](https://www.palletsprojects.com/p/flask/)

[Flask](/what-is/flask) is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions.

<br />

### [Light Bootstrap Dashboard](https://www.creative-tim.com/product/light-bootstrap-dashboard)

**Light Bootstrap Dashboard** is a Bootstrap4 admin dashboard template designed to be beautiful and simple. It is built on top of Bootstrap 4 and it is fully responsive. It comes with a big collection of elements that will offer you multiple possibilities to create the app that best fits your needs. It can be used to create admin panels, project management systems, web applications backend, CMS or CRM.

<br />

### More [Flask Dashboards](https://appseed.us/admin-dashboards/flask)

- [Flask Dashboard Material](https://appseed.us/admin-dashboards/flask-dashboard-material-design) - Free, MIT License
- [Flask Dashboard Material Dark](https://appseed.us/admin-dashboards/flask-dashboard-material-dark) - Free, MIT License
- [Flask Dashboard Material PRO](https://appseed.us/admin-dashboards/flask-dashboard-material-pro) - Commercial Product
- [Flask Dashboard Dashkit PRO](https://appseed.us/admin-dashboards/flask-dashboard-dashkit-pro) - Commercial Product

<br />

---
[Flask Dashboard Light](https://appseed.us/admin-dashboards/flask-dashboard-light-bootstrap) - Provided by AppSeed [Web App Generator](https://appseed.us/app-generator).
