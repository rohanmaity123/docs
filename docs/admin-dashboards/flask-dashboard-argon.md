title: Flask Boilerplate Dashboard Argon

# [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon)

**Open-Source Admin Dashboard** coded in **[Flask Framework](https://palletsprojects.com/p/flask/)** - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

## Dashboard Features
---

- SQLite, PostgreSQL, SQLAlchemy ORM
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Deployment scripts: Docker, Gunicorn
- UI Kit: **Black Dashboard** provided by **Creative-Tim**

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

- [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - the product page
- [Flask Dashboard Argon](https://github.com/app-generator/flask-boilerplate-dashboard-argon) - the source code
- [Flask Dashboard Argon](https://www.youtube.com/watch?v=bnCuQzDE3Ks) - yTube presentation

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
    |--- app/base/                        # base blueprint
    |--- app/base/static/assets           # Img, CSS, Janascript files
    |--- app/base/templates               # Jinja2 files (layouts, login pages)
    |                |---<errors>         # Dir with Error pages: 404, 500
    |                |---<login>          # Dir with Login and Registration pages
    |                |---<site_template>  # Dir with Login and Registration pages
    |
    |
    |--- app/home/                        # home blueprint
    |--- app/home/templates               # Jinja2 files (Pages): index, icons, tables
    |                |---- index.html     # Main dashboard page
    |                |---- maps.html      # Maps page
    |                |---- profile.html   # Profile Page
    |                |---- tables.html    # UI Tables
    |                |---- icons.html     # Ui Icons
    |
    |--- .env                             # store env variables
    |--- config.py                        # app configuration profiles: Debug, Production
    |
    |--- requirements.txt                 # Requirements for production PostgreSQL BDMS
    |--- requirements-sqlite.txt          # Requirements for development - SQLite storage
    |
    |--- run.py                           # bootstrap the app
    |
    |-----------------------------
```

<br />

## How to use it
---

```bash
$ # Get the code
$ git clone https://github.com/app-generator/flask-boilerplate-dashboard-argon.git
$ cd flask-boilerplate-dashboard-argon
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
$ git clone https://github.com/app-generator/flask-boilerplate-dashboard-argon.git
$ cd flask-boilerplate-dashboard-argon
```

> Start the app in Docker

```bash
$ sudo docker-compose pull && sudo docker-compose build && sudo docker-compose up -d
```

Visit `http://localhost:5000` in your browser. The app should be up & running.

<br />

## Support
---

- Free support via eMail < [support @ appseed.us](https://appseed.us/support) > and **Github** issues tracker
- (Paid) LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup)

<br />

## Credits & Links
---

- [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - Product page
- [Flask Framework](https://www.palletsprojects.com/p/flask/) - Offcial website
- [Flask Admin Dashboards](https://appseed.us/admin-dashboards/flask) - provided by AppSeed

<br />

## License
---

@MIT

<br />

## Flask Dashboard Black - app screens
---

<br />

![Flask Dashboard Argon - UI Fonts Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen-1.png)

<br />

![Flask Dashboard Argon - Google Maps Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen-2.png)

<br />

![Flask Dashboard Argon - User Profile Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen-3.png)

<br />

---
[Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
