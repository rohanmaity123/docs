title: Flask Boilerplate Dashboard Argon

# [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon)

**Open-Source Admin Dashboard** coded in **[Flask Framework](https://palletsprojects.com/p/flask/)** - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

## Dashboard Features

- SQLite, PostgreSQL, SQLAlchemy ORM
- Alembic (DB schema migrations)
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Deployment scripts: Docker, Gunicorn
- UI Kit: **Black Dashboard** provided by **Creative-Tim**

<br />

## Dashboard Links

- [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - the product page
- [Flask Dashboard Argon](https://github.com/app-generator/flask-boilerplate-dashboard-argon) - the source code
- [Flask Dashboard Argon](https://www.youtube.com/watch?v=bnCuQzDE3Ks) - yTube presentation

<br />


![Flask Dashboard Argon - Open-Source Admin Panel](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-screen.png)

<br />

## Dependencies and Environment
---

To use the apps, the workstation (or the deployment server) must have [Python3](https://www.python.org/) installed and basic development tools required to compile the Python packages. If you are not sure or familiar with the `development environment` concept, please access the links and learn how to set up your workstation.  

- Learn [how to install Python](/how-to/install-python)
- Set up [CentOS](/how-to/setup-centos-for-development), [Ubuntu](/how-to/setup-ubuntu-for-development) or [Windows OS](/how-to/setup-windows-for-development) for development

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

- Free support via eMail < [support @ appseed.us](https://appseed.us/support) > and **Github** issues tracker
- (Paid) LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup)

<br />

## Credits & Links

- [Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - Product page
- [Flask Framework](https://www.palletsprojects.com/p/flask/) - Offcial website
- [Flask Admin Dashboards](https://appseed.us/admin-dashboards/flask) - provided by AppSeed

<br />

## License

@MIT

<br />

---
[Flask Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
