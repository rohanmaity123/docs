title: Flask Dashboard Light

# [Flask Dashboard Light](https://appseed.us/admin-dashboards/flask-dashboard-black)

Open-Source Admin Dashboard with Light Dashboard Design coded in **[Flask](https://palletsprojects.com/p/flask/)** - features:

<br />

- [SQLite database](https://www.sqlite.org/index.html)
- [SQLAlchemy ORM](https://www.sqlalchemy.org/)
- Session based authentication flow (login, register)
- Static Build via Frozen-Flask

<br />

![Flask Dashboard Light - Open-Source Admin Panel](https://raw.githubusercontent.com/app-generator/flask-dashboard-light-bootstrap/master/screenshots/light-dashboard-flask-dashboard-intro.gif)

<br />

## Setup the environment
---

In order to use the boilerplates, we need [Python](/what-is/python/) and [Flask](/what-is/flask/) installed on the workstation. The Python can be downloaded from the official website and Flask can be easily added using `PIP` command:


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

```bash
$ # clone the sources
$ git clone https://github.com/app-generator/flask-dashboard-light-bootstrap.git
$ cd flask-dashboard-light-bootstrap
$
$ # install modules using a virtualenv
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # install deps 
$ pip install -r requirements.txt
$
$ # Create SQLite database using the Flask console
$ flask shell
>> from app import db
>> db.create_all()
>> quit() 
$
$ # SQLite database.db should be created in the app folder:
$ # app\database.db
$
$ # Set the FLASK_APP environment variable
$ (Windows) set FLASK_APP=app.py
$ (Unix) export FLASK_APP=app.py
$ (Powershell) $env:FLASK_APP = ".\app.py"
$ 
$ flask app.py
$ # app is running on port 5000
```

<br />

## Resources

- [Flask Dashboard Light](https://appseed.us/admin-dashboards/flask-dashboard-light-bootstrap) - product page
- [Flask Dashboard Light](https://flask-dashboard-light-bootstrap.appseed.us/) - live DEMO
- [Flask Dashboard Light](https://github.com/app-generator/flask-dashboard-light-bootstrap) - the source code published on Github

