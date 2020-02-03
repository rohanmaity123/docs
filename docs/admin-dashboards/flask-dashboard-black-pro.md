title: Flask Dashboard Black PRO

# [Flask Dashboard Black PRO](https://appseed.us/admin-dashboards/flask-dashboard-black-pro)

**Commercial** Admin Dashboard coded in [Flask Framework](https://palletsprojects.com/p/flask/) on top of [Black Dashboard](https://themes.getbootstrap.com/product/black-dashboard-pro-premium-bootstrap-4-admin/) design (PRO Version) provided by Creative-Tim Agency.

<br />

## Dashboard Features
---

- SQLite, PostgreSQL, SQLAlchemy ORM
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Deployment scripts: Docker, Gunicorn
- UI Kit: **Black Dashboard** provided by **Creative-Tim**
- License: [Commercial](https://github.com/app-generator/flask-dashboard-black-pro/blob/master/LICENSE.md)
- LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup) and email **< support @ appseed.us >**

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

- [Flask Dashboard Black PRO](https://appseed.us/admin-dashboards/flask-dashboard-black-pro) - Product page
- [Flask Dashboard Black PRO](https://github.com/app-generator/flask-dashboard-black-pro) - The public repository, used for bug tracking and licensing information
- [Flask Dashboard Black PRO](https://flask-dashboard-black-pro.appseed.us/) - LIVE demo
- [Flask Dashboard Black PRO](https://www.youtube.com/watch?v=JAVUaUfY1zY) - yTube video presentation

<br />

![Flask Dashboard Black PRO - Admin Panel coded in Flask.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-black-pro-screen.png)

<br />

## Get the source code
---

- Access the [product page](https://appseed.us/admin-dashboards/flask-dashboard-black-pro) and purchase a **license**
- Accept the invitation to the private repository (sent by the [AppSeed](http://appseed.us/) platform, once the purchase is validated)
- Clone the source code and build the [Flask Black Dashboard](https://appseed.us/admin-dashboards/flask-dashboard-black-pro) using the instructions presented here.

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
< PROJECT ROOT >                  # application root folder
    |
    |--- app/__init__.py          # application constructor  
    |--- app/base/                # base blueprint
    |--- app/home/                # home blueprint
    |
    |--- .env                     # store env variables
    |--- config.py                # app configuration profiles: Debug, Production
    |
    |--- requirements.txt         # Requirements for production PostgreSQL BDMS
    |--- requirements-sqlite.txt  # Requirements for development - SQLite storage
    |
    |--- run.py                   # bootstrap the app
    |
    |-----------------------------
```

<br />

## How to use it
---

```bash
$ # Get the code
$ git clone https://github.com/app-generator/priv-flask-dashboard-black-pro.git
$ cd priv-flask-dashboard-black-pro
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
$ git clone https://github.com/app-generator/priv-flask-dashboard-black-pro.git
$ cd priv-flask-dashboard-black-pro
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
- Use the FREE version of the app - [Flask Dashboard Black](https://appseed.us/admin-dashboards/flask-dashboard-black)
- See the full list with [Flask Admin Dashboards](https://appseed.us/admin-dashboards/flask) - provided by AppSeed

<br />

## Flask Dashboard Black - app screens
---

<br />

![Flask Dashboard Black PRO - Charts Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-black-pro-screen-1.png)

<br />

![Flask Dashboard Black PRO - Pricing cards Screen.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-black-pro-screen-4.png)

<br />

![Flask Dashboard Black PRO - App Screen-Shot.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-dashboard-black-pro-screen-3.png)

<br />

---
[Flask Dashboard Black PRO](https://appseed.us/admin-dashboards/flask-dashboard-black-pro) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
