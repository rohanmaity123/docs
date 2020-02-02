title: Flask Dashboard Material PRO

# [Flask Dashboard Material PRO](https://appseed.us/admin-dashboards/flask-dashboard-material-pro)

**Commercial** Admin Dashboard coded in [Flask Framework](https://palletsprojects.com/p/flask/) on top of [Material Dashboard](https://www.creative-tim.com/product/material-dashboard-pro) design (PRO Version) provided by Creative-Tim Agency.

<br />

## Dashboard Features
---

- SQLite, PostgreSQL, SQLAlchemy ORM
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Deployment scripts: Docker, Gunicorn
- UI Kit: **Material Dashboard** provided by **Creative-Tim**
- License: [Commercial](https://github.com/app-generator/flask-dashboard-material-pro/blob/master/LICENSE.md)
- LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup) and email **< support @ appseed.us >**

<br />

## Dashboard technology stack
---

- Used Language: [Python3](https://www.python.org/) (Python2 is not supported)
- Web Framework: [Flask](https://www.palletsprojects.com/p/flask/)
- CSS Framework: [Bootstrap CSS](https://getbootstrap.com/)
- Design Theme: **Material Dashboard PRO** provided by Creative-Tim

<br />

## Dashboard Links
---

- [Flask Dashboard Material PRO](https://appseed.us/admin-dashboards/flask-dashboard-material-pro) - Product page
- [Flask Dashboard Material PRO](https://github.com/app-generator/flask-dashboard-material-pro) - The public repository, used for bug tracking and licensing information
- [Flask Dashboard Material PRO](https://flask-dashboard-material-pro.appseed.us/) - LIVE demo
- [Flask Dashboard Material PRO](https://www.youtube.com/watch?v=0Ovhjp1hsew) - yTube video presentation

<br />

![Flask Dashboard Material PRO - Admin Panel coded in Flask.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-material-pro-screen.png)

<br />

## Get the source code
---

- Access the [product page](https://appseed.us/admin-dashboards/flask-dashboard-material-pro) and purchase a **license**
- Accept the invitation to the private repository (sent by the [AppSeed](http://appseed.us/) platform, once the purchase is validated)
- Clone the source code and build the [Flask Material Dashboard](https://appseed.us/admin-dashboards/flask-dashboard-material-pro) using the instructions presented here.

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
$ git clone https://github.com/app-generator/priv-flask-dashboard-material-pro.git
$ cd priv-flask-dashboard-material-pro
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
$ git clone https://github.com/app-generator/priv-flask-dashboard-material-pro.git
$ cd priv-flask-dashboard-material-pro
```

> Start the app in Docker

```bash
$ sudo docker-compose pull && sudo docker-compose build && sudo docker-compose up -d
```

Visit `http://localhost:5000` in your browser. The app should be up & running.

<br />

## Support
---

24/7 Live [support](appseed.us/support) via [Discord](https://discord.gg/fZC6hup) and eMail **< support@appseed.us >**

<br />

### Links & Resources
---

- Read more about **Flask** by accessing the [official Flask website](https://palletsprojects.com/p/flask/) or read the [docs](https://flask.palletsprojects.com/).
- Use the FREE version of the app - [Flask Dashboard Material](https://appseed.us/admin-dashboards/flask-dashboard-material-design)
- See the full list with [Flask Admin Dashboards](https://appseed.us/admin-dashboards/flask) - provided by AppSeed

<br />

## Flask Dashboard Material - app screens
---

<br />

![Flask Dashboard Material PRO - Maps Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-material-pro-screen-1.png)

<br />

![Flask Dashboard Material PRO - UI Tables Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-material-pro-screen-2.png)

<br />

![Flask Dashboard Material PRO - UI Widgets Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-material-pro-screen-3.png)
