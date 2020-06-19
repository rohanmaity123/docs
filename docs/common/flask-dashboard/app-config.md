## App Configuration
---

The configuration file **`config.py`** (in the root of the project) define a dual configuration controlled via the `.env` file ( `DEBUG` variable)

> **DebugConfig** - default configuration used for development

This configuration becomes active if `.env` file has the `DEBUG` file set to *True*

```python
# Development/Debug configuration

# Set up the App SECRET_KEY
SECRET_KEY = config('SECRET_KEY', default='S#perS3crEt_007')

# This will create a file in <app> FOLDER
SQLALCHEMY_DATABASE_URI = 'sqlite:///' + os.path.join(basedir, 'db.sqlite3')
SQLALCHEMY_TRACK_MODIFICATIONS = False

```

During the first request, the SQLite database and tables are automatically created in the root in the project.

> *Hint*: to visualize the SQLite database content an external tool should be installed: [DB Browser for SQLite](https://sqlitebrowser.org/) it might be a good choice.

<br />

> **ProductionConfig** - production configuration

This configuration becomes active if `.env` file has the `DEBUG` file set to *False*

```python
# Production configuration

SESSION_COOKIE_HTTPONLY  = True
REMEMBER_COOKIE_HTTPONLY = True
REMEMBER_COOKIE_DURATION = 3600

# PostgreSQL database
SQLALCHEMY_DATABASE_URI = '{}://{}:{}@{}:{}/{}'.format(
    config( 'DB_ENGINE'   , default='postgresql'    ),
    config( 'DB_USERNAME' , default='appseed'       ),
    config( 'DB_PASS'     , default='pass'          ),
    config( 'DB_HOST'     , default='localhost'     ),
    config( 'DB_PORT'     , default=5432            ),
    config( 'DB_NAME'     , default='appseed-flask' )
)

```

In this configuration profile, the database defaults to a PostgreSQL DBMS. Make sure the `.env` has the right credentials to access the database.

<br />

