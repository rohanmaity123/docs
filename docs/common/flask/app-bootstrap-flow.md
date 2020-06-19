## The bootstrap flow
---

- `run.py` imports the WSGI Application from `app` directory
-  `app/__init__.py` is called and trigger the following actions:
    - invoke Flask Framework constructor
    - Read the configuration from `app/config.py`
    - Invoke [SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
    - Invoke LoginManager exposed by [Flask-Login](https://flask-login.readthedocs.io/en/latest/)  

<br />

> **`app/__init__.py`** (simplified version)

```python
# File: /app/__init__.py

from flask            import Flask        # Import Flask
from flask_sqlalchemy import SQLAlchemy   # For ORM db access  
from flask_login      import LoginManager # Used for authentication

# Directive 1 - Inject Flask magic
app = Flask(__name__)

# Directive 2 - Load the configuraton from `app/config.py`
app.config.from_object('app.config.Config')

# Directive 3 - Flask-SqlAlchemy wrapping
db = SQLAlchemy  (app)

# Directive 4 - Invoke and init the login manager
lm = LoginManager( )
lm.init_app(app)

# Directive 5 - Setup database (create tables)
@app.before_first_request
def initialize_database():
    db.create_all()

# Directive 5 - Start the App
from app import views, models

# At this point we have a valid WSGI app
```

<br />

The **`app/__init__.py`** constructs the app by putting together a short-list of things:

- Invoke Flask
- Load the configuration from **`config.py`**
- Invoke the SqlAlchemy ORM to handle the database content
- Invoke and inject the `Login Manager` into the app
- Check if the database tables are created
- Finally, expose the app by importing views (app routing) and models (app tables)

<br />

