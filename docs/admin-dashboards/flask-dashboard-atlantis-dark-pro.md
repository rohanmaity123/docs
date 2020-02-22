title: Flask Atlantis Dark PRO

# [Flask Atlantis Dark PRO](https://appseed.us/admin-dashboards/flask-dashboard-atlantis-dark-pro)

**Commercial** Admin Dashboard coded in [Flask Framework](https://palletsprojects.com/p/flask/) on top of [Atlantis Dark Dashboard](https://themekita.com/atlantis-bootstrap-dashboard.html) design (PRO Version) provided by ThemeKita Agency.

<br />

## Dashboard Features
---

- SQLite, PostgreSQL, SQLAlchemy ORM
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Deployment scripts: Docker, Gunicorn
- UI Kit: **Black Dashboard** provided by **ThemeKita**
- License: [Commercial](https://github.com/app-generator/flask-dashboard-atlantis-dark-pro/blob/master/LICENSE.md)
- LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup) and email **< support @ appseed.us >**

<br />

## Dashboard technology stack
---

- Used Language: [Python3](https://www.python.org/) (Python2 is not supported)
- Web Framework: [Flask](https://www.palletsprojects.com/p/flask/)
- CSS Framework: [Bootstrap CSS](https://getbootstrap.com/)
- Design Theme: **Atlantis Black Dashboard** provided by ThemeKita

<br />

## Dashboard Links
---

- [Flask Dashboard Atlantis Dark PRO](https://appseed.us/admin-dashboards/flask-dashboard-atlantis-dark-pro) - Product page
- [Flask Dashboard Atlantis Dark PRO](https://github.com/app-generator/flask-dashboard-atlantis-dark-pro) - The public repository, used for bug tracking and licensing information
- [Flask Dashboard Atlantis Dark PRO](https://www.youtube.com/watch?v=YTYMeku9iMU) - yTube video presentation

<br />

![Flask Dashboard Atlantis Dark PRO - Admin Panel coded in Flask.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-atlantis-dark-pro-screen.png)

<br />

## Get the source code
---

- Access the [product page](https://appseed.us/admin-dashboards/flask-dashboard-atlantis-dark-pro) and purchase a **license**
- Accept the invitation to the private repository (sent by the [AppSeed](http://appseed.us/) platform, once the purchase is validated)
- Clone the source code and build the [Flask Atlantis Dark Dashboard](https://appseed.us/admin-dashboards/flask-dashboard-atlantis-dark-pro) using the instructions presented here.

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

## How to use it
---

```bash
$ # Get the code
$ git clone https://github.com/app-generator/priv-flask-dashboard-atlantis-dark-pro.git
$ cd priv-flask-dashboard-atlantis-dark-pro
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv --no-site-packages env
$ # .\env\Scripts\activate
$
$ # Install modules - SQLite Database
$ pip3 install -r requirements.txt
$
$ # OR with PostgreSQL connector
$ # pip install -r requirements-pgsql.txt
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
$ # Start the application (development mode)
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the dashboard in browser: http://127.0.0.1:5000/
```

<br />

### [Docker](https://www.docker.com/) execution
---

The application can be easily executed in a docker container. The steps:

> Get the code

```bash
$ git clone https://github.com/app-generator/priv-flask-dashboard-dashkit-pro.git
$ cd priv-flask-dashboard-dashkit-pro
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
> Start the app using `gunicorn` binary

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

## Flask Atlantis Dark - app screens
---

<br />

![Flask Dashboard Atlantis Dark PRO - Charts Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-atlantis-dark-pro-screen-1.png)

<br />

![Flask Dashboard Atlantis Dark PRO - Pricing cards Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-atlantis-dark-pro-screen-4.png)

<br />

![Flask Dashboard Atlantis Dark PRO - App Screen-Shot.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-atlantis-dark-pro-screen-3.png)

## Credits & Links
---

<br />

### What is [Flask](https://www.palletsprojects.com/p/flask/)

[Flask](https://www.palletsprojects.com/p/flask/) is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around Werkzeug and Jinja and has become one of the most popular Python web application frameworks.

<br />

### [What is dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))

In information technology, a **[dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))** is a user interface that, somewhat resembling an automobile's dashboard, organizes and presents information in a way that is easy to read. However, a computer dashboard is more likely to be interactive than an automobile dashboard (unless it is also computer-based). To some extent, most graphical user interfaces (GUIs) resemble a dashboard - by [Techtarget](https://searchcio.techtarget.com/definition/dashboard)

<br />

### [Atlantis Dashboard PRO](https://themekita.com/demo-atlantis-bootstrap)

Atlantis PRO is a beautiful Bootstrap 4 admin dashboard that is beautifully and elegantly designed to display various metrics, numbers or data visualization. Atlantis PRO admin dashboard has 4 layouts, many plugins, pages and a huge colection of UI components to help developers create dashboards quickly and effectively so they can save development time and also help users to make the right and fast decisions based on existing data.

<br />

---
[Flask Atlantis Dark PRO](https://appseed.us/admin-dashboards/flask-dashboard-atlantis-dark-pro) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
