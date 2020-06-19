## App Configuration
---

The configuration file **`app/config.py`** specify a short-list with variables:

- `SECRET_KEY` - Required by Flask for [session management](https://flask.palletsprojects.com/en/1.1.x/quickstart/#sessions)
- `SQLALCHEMY_DATABASE_URI` - The database URI used to [configure Flask-SqlAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/config/#configuration)

This configuration is loaded by **`app/__init__.py`** during the app initialization:

```python
# File: /app/__init__.py

...

# Directive 2 - Load the configuraton from `app/config.py`
app.config.from_object('app.config.Config')

...

```

<br />

The default database is [SQLite](https://www.sqlite.org/), configured by the `SQLALCHEMY_DATABASE_URI` variable:

```python
# File: /app/config.py

...

SQLALCHEMY_DATABASE_URI = 'sqlite:///' + os.path.join(basedir, 'db.sqlite3')
SQLALCHEMY_TRACK_MODIFICATIONS = False

...

```

The database and associated tables, defined in `app/models.py` are automatically created at the first request in the physical file specified in the configuration - default location `app/db.sqlite3`.

> **Hint**: to visualize the SQLite database content an external tool should be installed: [DB Browser for SQLite](https://sqlitebrowser.org/) it might be a good choice.

<br />
