title: Flask Dashboard Dashkit PRO

# [Flask Dashboard Dashkit PRO](https://appseed.us/admin-dashboards/flask-dashboard-dashkit-pro)

**Commercial** Admin Dashboard coded in [Flask Framework](https://palletsprojects.com/p/flask/) on top of [Dashkit Dashboard](https://cssninja.io/themes/dashkit) design (PRO Version) provided by CssNinja Web Agency.

<br />

## Dashboard Features
---

- SQLite, PostgreSQL, SQLAlchemy ORM
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Deployment scripts: Docker, Gunicorn
- UI Kit: **Dashkit Dashboard** provided by **CssNinja**
- License: [Commercial](https://github.com/app-generator/flask-dashboard-dashkit-pro/blob/master/LICENSE.md)
- LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup) and email **< support @ appseed.us >**

<br />

## Dashboard Links
---

- [Flask Dashboard Dashkit PRO](https://appseed.us/admin-dashboards/flask-dashboard-dashkit-pro) - Product page
- [Flask Dashboard Dashkit PRO](https://github.com/app-generator/flask-dashboard-dashkit-pro) - The public repository, used for bug tracking and licensing information
- [Flask Dashboard Dashkit PRO](https://www.youtube.com/watch?v=C-jKyXd3c28) - yTube video presentation

<br />

![Flask Dashboard Dashkit PRO - Admin Panel coded in Flask.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-dashkit-pro-screen.png)

<br />

## Get the source code
---

- Access the [product page](https://appseed.us/admin-dashboards/flask-dashboard-dashkit-pro) and purchase a **license**
- Accept the invitation to the private repository (sent by the [AppSeed](http://appseed.us/) platform, once the purchase is validated)
- Clone the source code and build the [Flask Dashkit Dashboard](https://appseed.us/admin-dashboards/flask-dashboard-dashkit-pro) using the instructions presented here.

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
$ git clone https://github.com/app-generator/priv-flask-dashboard-dashkit-pro.git
$ cd priv-flask-dashboard-dashkit-pro
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv --no-site-packages env
$ # .\env\Scripts\activate
$ 
$ # Install modules
$ # SQLIte version (no PostgreSQL)
$ pip3 install -r requirements-sqlite.txt
$ 
$ # OR with PostgreSQL connector
$ pip install -r requirements.txt
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

## Docker execution
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

Visit `http://localhost:5000` in your browser. The app should be up & running.

<br />

## Flask Dashkit - App Screens
---

<br />

![Flask Dashboard Dashkit PRO - Charts Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-dashkit-pro-screen-1.png)

<br />

![Flask Dashboard Dashkit PRO - Pricing cards Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-dashkit-pro-screen-4.png)

<br />

![Flask Dashboard Dashkit PRO - App Screen-Shot.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-dashkit-pro-screen-3.png)

## Credits & Links
---

<br />

### What is [Flask](https://www.palletsprojects.com/p/flask/)

[Flask](https://www.palletsprojects.com/p/flask/) is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around Werkzeug and Jinja and has become one of the most popular Python web application frameworks.

<br />

### [What is dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))

In information technology, a **[dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))** is a user interface that, somewhat resembling an automobile's dashboard, organizes and presents information in a way that is easy to read. However, a computer dashboard is more likely to be interactive than an automobile dashboard (unless it is also computer-based). To some extent, most graphical user interfaces (GUIs) resemble a dashboard - by [Techtarget](https://searchcio.techtarget.com/definition/dashboard)

<br />

### [Dashkit UI PRO](https://cssninja.io/themes/dashkit)

**[Dashkit](https://cssninja.io/themes/dashkit)** comes bundled with Bulkit as a dashboard starter kit. It offers some original styles and also a catchy user profile. The design has been thought to give the best possible experience either on mobile and on desktop. Dashkit uses the Bulkit theming system, so you can change all colors in a breeze. **[Dashkit](https://cssninja.io/themes/dashkit)** also uses some of Bulkit components. You can add more or remove those that you don't need.

<br />

### [Bulma Css](https://bulma.io/)

Bulma is a free, open-source CSS framework based on Flexbox and built with Sass. It's 100% responsive, fully modular, and available for free.

<br />

---
[Flask Dashboard Black PRO](https://appseed.us/admin-dashboards/flask-dashboard-black-pro) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
