title: Flask Boilerplate Dashboard Argon

# [Flask Boilerplate Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon)

Open-Source and Free **[admin dashboard](https://appseed.us/admin-dashboards)** with Argon Design coded in **[Flask](https://palletsprojects.com/p/flask/)**. **Dashboard** features:

<br />

- [SQLite database](https://www.sqlite.org/index.html)
- [SQLAlchemy ORM](https://www.sqlalchemy.org/)
- [Alembic](https://alembic.sqlalchemy.org/) (for db-schema migrations)
- Modular design with [Blueprints](https://flask.palletsprojects.com/en/1.0.x/blueprints/)
- Session Based authentication (via [flask_login](https://flask-login.readthedocs.io/en/latest/)) - [bcrypt](https://flask-bcrypt.readthedocs.io/) hashed passwords
- Forms validation
- Unitary tests
- Deployment scripts: Docker, gunicorn

<br />

![Flask Dashboard Argon - Open-Source Admin Panel](https://raw.githubusercontent.com/app-generator/static/master/products/flask-boilerplate-dashboard-argon-intro.gif)

<br />

## Setup the environment
---

In order to use the boilerplate, we need [Python](/what-is/python/) and [Flask](/what-is/flask/) installed on the workstation. 
The Python can be downloaded from the [official website](https://www.python.org/) and Flask can be easily added using `PIP` command:

```bash
$
$ # Test the Python install 
$ python --version
$ Python 3.7.2
$
$ # install Flask using PIP
$ pip install Flask
$
```

<br />

## Build from sources
---
Note: The boilerplate can be used with [PostgreSQL](https://www.postgresql.org/) and require `requirements.txt` for modules installation. 
For usage with SQLite database, please use `requirements-no-postgres.txt` ([psycopg2](https://pypi.org/project/psycopg2/) is removed from the dependencies) 

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
$ pip install -r requirements-no-postgres.txt
$ 
$ # OR with PostgreSQL connector
$ pip install -r requirements.txt
$
$ # 3. Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=appseed-app.py
$ (Windows) set FLASK_APP=appseed-app.py
$ (Powershell) $env:FLASK_APP = ".\appseed-app.py"
$
$ # 4. Run the application
$ flask run --host=0.0.0.0
$
$ # 5. Go to http://127.0.0.1:5000/, create an account and log in
```

<br />


## Resources

- [Flask Boilerplate Dashboard Argon](https://appseed.us/admin-dashboards/flask-boilerplate-dashboard-argon) - product page
- [Flask Boilerplate Dashboard Argon](https://github.com/app-generator/flask-boilerplate-dashboard-argon) - the source code
- [Flask Boilerplate Dashboard Argon](https://www.youtube.com/watch?v=bnCuQzDE3Ks/) - video presentation

 
