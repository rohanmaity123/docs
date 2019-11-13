title: Flask Boilerplate Dashboard Argon

# [Flask Boilerplate Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon)

**[Open-Source Admin Dashboard](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon)** coded in **Flask Web Framework** on top of **Argon Dashboard** design, crafted by Creative-Tim agency. **Dashboard** features:

- SQLite, PostgreSQL
- SQLAlchemy ORM
- Alembic
- Modular design with **Blueprints**
- Session-Based authentication (via **flask_login**)
- Forms validation
- Unitary tests
- Deployment scripts: Docker, Gunicorn
- **License MIT**

<br />

![Flask Dashboard Argon - Open-Source Admin Panel](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-intro.gif)

<br />

## Setup the environment
---

In order to use the boilerplate, we need [Python3](/what-is/python/) and `virtualenv` python library.

<br />

> *Note*: **Python2 is not supported**, the EOL of this version announced [here](https://www.python.org/doc/sunset-python-2/). In order to use our kits, please migrate to Pyhton3. Thank you!

<br />

```bash
$ # Test the Python install
$ python --version
$ Python 3.7.2
$
$ # install Virtualenv using PIP
$ pip install virtualenv
```

<br />

## Build from [sources](https://github.com/app-generator/flask-boilerplate-dashboard-argon/)
---

> *Note*: The production setup (PostgreSQL Database) require `requirements.txt` for modules installation.
For local (SQLite DB) please use `requirements-sqlite.txt`.

<br />

```bash
$ # 1. Get the code
$ git clone https://github.com/app-generator/flask-boilerplate-dashboard-argon.git
$ cd flask-boilerplate-dashboard-argon
$
$ # install modules using a virtualenv
$ virtualenv --no-site-packages env
$ source env/bin/activate
$ 
$ # 2. Install requirements
$ # SQLIte version (no PostgreSQL)
$ pip install -r requirements-sqlite.txt
$ 
$ # OR with PostgreSQL connector
$ pip install -r requirements.txt
$
$ # 3. Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=run.py
$ (Windows) set FLASK_APP=run.py
$ (Powershell) $env:FLASK_APP = ".\run.py"
$
$ # 4. Run the application
$ flask run --host=0.0.0.0
$
$ # 5. Go to http://127.0.0.1:5000/, create an account and log in
```

<br />

## Project Structure
---

The boilerplate code is built with a modular structure that follows the recommended pattern used by many open-source projects. The most important files / directories are listed bellow:

- [run.py](https://github.com/app-generator/flask-boilerplate-dashboard-argon/blob/master/run.py)
- [config.py](https://github.com/app-generator/flask-boilerplate-dashboard-argon/blob/master/config.py)
- [app /](https://github.com/app-generator/flask-boilerplate-dashboard-argon/tree/master/app)
- [app / __init__.py](https://github.com/app-generator/flask-boilerplate-dashboard-argon/blob/master/app/__init__.py)
- [app / base](https://github.com/app-generator/flask-boilerplate-dashboard-argon/tree/master/app/base)
- [app / home](https://github.com/app-generator/flask-boilerplate-dashboard-argon/tree/master/app/home)

<br />

```bash
< ROOT > - Flask Dashboard Argon  # application root folder
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

## Support
---

- Free support via eMail < [support @ appseed.us](https://appseed.us/support) > and [Github](https://github.com/app-generator/flask-boilerplate-dashboard-argon/issues/)
- 24/7 Live Support via [Discord](https://discord.gg/fZC6hup) for paid plans and commercial products.

<br />

## Resources
---

- [Flask Boilerplate Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - Product page
- [Flask Boilerplate Dashboard Argon](https://github.com/app-generator/flask-boilerplate-dashboard-argon) - Source code
- [Flask Boilerplate Dashboard Argon](https://www.youtube.com/watch?v=bnCuQzDE3Ks/) - Video presentation (Youtube)
- [Flask Framework](https://www.palletsprojects.com/p/flask/) - Offcial website
- [Flask Dashboard - Open-Source Boilerplates](https://dev.to/sm0ke/flask-dashboard-open-source-boilerplates-dkg) - A popular article published on Dev.to platform
- [Flask Dashboard](https://admin-dashboards.com/tags/flask-dashboard) - Index provided by **Admin-Dashboards.com**
