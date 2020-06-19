## Data Structures
---

The Flask starter exposes a short-list with data structures used globally across the app:

<br />

### `current_user` object

Constructed by [Flask-Login](https://flask-login.readthedocs.io/en/latest/) can be used to detect if the current request is executed by an authenticated user or not. The object has global visibility and can be used in all app controllers and handlers but also in views.

<br />

> **How it works**

`app/views.py` define a callback function required by **Flask-Login** library:

```python
# File: app/views.py

# *****************************************
# `lm` is constructed in `app/__init__.py`
#
# lm = LoginManager(   ) # flask-loginmanager
# lm.init_app(app)       # init the login manager
#
# *****************************************
#
# provide login manager with load_user callback
@lm.user_loader
def load_user(user_id):
    return User.query.get(int(user_id))
```

<br />

> **Usage in contoler**

```python
# File: app/views.py

def index(path):

    # Redirect guests users to login page
    if not current_user.is_authenticated:
        return redirect(url_for('login'))
```

<br />

> **Usage in view**

```html
    <div class="collapse navbar-collapse" id="navigation">
        <ul class="navbar-nav ml-auto">

        <!-- The Usage of <current_user> object -->
        {% if current_user.is_authenticated %}

            <!-- Html chunk rendered for authenticated users-->

            <li class="nav-item">
                <a href="/" class="nav-link text-primary">
                    <i class="tim-icons icon-minimal-left"></i> Back to Dashboard
                </a>
            </li>

        {% else %}

            <!-- Html chunk rendered for guests users-->

            <li class="nav-item ">
                <a href="{{ url_for('register') }}" class="nav-link">
                    <i class="tim-icons icon-laptop"></i> Register
                </a>
            </li>
            <li class="nav-item ">
                <a href="{{ url_for('login') }}" class="nav-link">
                    <i class="tim-icons icon-single-02"></i> Login
                </a>
            </li>

        {% endif %}

        </ul>
    </div>
```

<br />
