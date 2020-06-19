## The bootstrap flow
---

- `run.py` loads the `.env` file
- Initialize the app using the specified profile: *Debug* or *Production*
    - If env.DEBUG is set to *True* the SQLite storage is used
    - If env.DEBUG is set to *False* the specified DB driver is used (MySql, PostgreSQL)
- Call the app factory method `create_app` defined in app/__init__.py
- Redirect the guest users to Login page
- Unlock the pages served by *home* blueprint for authenticated users

<br />

> **`.env`** (saved in the root of the project)

```bashrc
# File: `.env`

DEBUG=True              # Enable/Disable the development environment

SECRET_KEY=S3cr3t_Key   # The Key used by Flask to encrypt session information

# Database production settings (If DEBUG=False)

DB_ENGINE=postgresql    # DBMS
DB_NAME=appseed-flask   # Database Name
DB_HOST=localhost       # Database Host
DB_PORT=5432            # Database Port
DB_USERNAME=appseed     # DB Username
DB_PASS=pass            # DB Password

```

<br />

> **`run.py`** (simplified version)

```python
# File: run.py

DEBUG = config('DEBUG', default=True)

# Create the WSGI app, using the app factory pattern
app = create_app( app_config )

# Migrate automaticaly the app using Flask Migrate library
Migrate(app, db)
```

<br />

> **`app/__init__.py`** (simplified version)

```python
# File: app/__init__.py

db            = SQLAlchemy()        # Invoke SQLAlchemy
login_manager = LoginManager()      # Invoke Login Manager

def register_extensions(app):
    db.init_app(app)                # Inject SQLAlchemy magic
    login_manager.init_app(app)     # Add Login Manager to the app

# Register app blueprints: `base`, `home`
def register_blueprints(app):
    for module_name in ('base', 'home'):
        module = import_module('app.{}.routes'.format(module_name))
        app.register_blueprint(module.blueprint)

# Create the tables (automaticaly)
def configure_database(app):

    @app.before_first_request
    def initialize_database():
        db.create_all()

# Create the WSGI app using the factory pattern
def create_app(config):
    app = Flask(__name__, static_folder='base/static')
    app.config.from_object(config)
    register_extensions(app)
    register_blueprints(app)
    configure_database(app)
    return app
```

<br />

The **`app/__init__.py`** constructs the app by putting together a short-list of things:

- Invoke SQLAlchemy
- Invoke and inject the `Login Manager` into the app
- Load the configuration from `config.py` file
- Register the app blueprints
- Check if the database tables are created
- return the WSGI app

<br />
