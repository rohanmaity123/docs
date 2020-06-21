## App Configuration
---

The environment configuration file **`.env`** specify a short-list with variables:

- [`SECRET_KEY`](https://docs.djangoproject.com/en/3.0/ref/settings/#secret-key) - Used by Django for [cryptographic signing](https://docs.djangoproject.com/en/3.0/topics/signing/)
- `SERVER` - The public domain/address used in production

```python
# File: core/settings.py

...

# SECRET_KEY value is read from `.env` file
SECRET_KEY = config('SECRET_KEY', default='S#perS3crEt_1122')

...

# Load the production server address from `.env` file
ALLOWED_HOSTS = ['localhost', '127.0.0.1', config('SERVER', default='127.0.0.1')]

...

# The SQLite database, located in the root of the project
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}

```

<br />

The default database is [SQLite](https://www.sqlite.org/) and the name and physical location can be changed by updating `core/settings.py`
The database and associated tables are created during the migration commands, listed in the README file:

```bash
$ # README file, shipped with every Django project

...

$ python manage.py makemigrations
$ python manage.py migrate

...
```

> **Hint**: to visualize the SQLite database content an external tool should be installed: [DB Browser for SQLite](https://sqlitebrowser.org/) it might be a good choice.

<br />
