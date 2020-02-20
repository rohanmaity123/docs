title: Flask Dashboard Argon

# [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-dashboard-argon)

**Open-Source Admin Dashboard** coded in **[Flask Framework](https://palletsprojects.com/p/flask/)** on top of **Argon Dashboard** design (free version) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

<br />

## Dashboard Features
---

- SQLite database
- SQLAlchemy ORM
- Session-Based authentication flow (login, register)
- UI Kit: **[Argon Dashboard](https://flask-dashboard-argon.appseed.us/login)** (Free version) provided by **Creative-Tim**
- **MIT License**
- Support: Free support via **Github** and (Paid) **24/7 LIVE Support** via [Discord](https://discord.gg/fZC6hup)

<br />

> Note: **For enhanced version** (blueprints, deployment scripts) of this dashboard please visit: [Flask Panel Dashboard Argon](https://github.com/app-generator/flask-boilerplate-dashboard-argon). Thank you!

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

- [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-dashboard-argon) - Product page
- [Flask Dashboard Argon](https://github.com/app-generator/flask-argon-dashboard) - Source code (published on Github)
- [Flask Dashboard Argon](https://flask-dashboard-argon.appseed.us/login) - LIVE demo

<br />

![Flask Dashboard Argon - Open-Source Admin Panel](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen.png)

<br />

## Prepare your environment
---

The product is built on top of [Flask](https://palletsprojects.com/p/flask/), a popular Python Web Framework. To build the app, Python3 should be installed properly in the workstation. If you are not sure if Python is properly installed, please open a terminal and type `python --version`. The full-list with dependencies and tools required to build the app:

- [Python3](https://www.python.org/) - the programming language used to code the app
- [Git](https://git-scm.com/) - used to clone the source code from the Github repository
- A [Github](https://github.com/) account - the invitation to the source code, will be sent on your account.
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment.

<br />

> Check Python (using the terminal)

```bash
$ # Check Python version
$ python --version
Python 3.7.2 # <--- All good
```

<br />

> Check GIT command tool (using the terminal)

```bash
$ # Check git
$ git --version
$ git version 2.10.1.windows.1 # <--- All good
```

<br />

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
    |                |---- login.html     # Login page
    |                |---- register.html  # Registration Page
    |                |---- tables.html    # UI Tables
    |                |---- icons.html     # UI Icons
    |
    |--- requirements.txt                 # Modules and dependencies
    |
    |--- run.py                           # bootstrap the app
    |
    |-----------------------------
```

<br />

## Build from sources
---

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/flask-argon-dashboard.git
$ cd flask-argon-dashboard
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

## Flask Dashboard Argon - App Screens
---

<br />

![Flask Dashboard Argon - UI Fonts Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen-1.png)

<br />

![Flask Dashboard Argon - Google Maps Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen-2.png)

<br />

![Flask Dashboard Argon - User Profile Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen-3.png)

<br />

## Credits & Links
---

<br />

## What is [Flask](https://www.palletsprojects.com/p/flask/)

[Flask](https://www.palletsprojects.com/p/flask/) is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around Werkzeug and Jinja and has become one of the most popular Python web application frameworks.

<br />

## [What is dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))

In information technology, a **[dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))** is a user interface that, somewhat resembling an automobile's dashboard, organizes and presents information in a way that is easy to read. However, a computer dashboard is more likely to be interactive than an automobile dashboard (unless it is also computer-based). To some extent, most graphical user interfaces (GUIs) resemble a dashboard - by [Techtarget](https://searchcio.techtarget.com/definition/dashboard)

<br />

## [Argon Dashboard](https://www.creative-tim.com/product/argon-dashboard)

Argon Dashboard is built with over 100 individual components, giving you the freedom of choosing and combining. All components can take variations in color, that you can easily modify using SASS files and it is open source, and free.

<br />

---
[Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
