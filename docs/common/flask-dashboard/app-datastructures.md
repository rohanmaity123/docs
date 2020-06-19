## Data Structures
---

The Flask starter exposes a short-list with data structures used globally across the app:

<br />

### `current_user` object

Constructed by [Flask-Login](https://flask-login.readthedocs.io/en/latest/) can be used to detect if the current request is executed by an authenticated user or not. The object has global visibility and can be used in all app controllers and handlers but also in views.

<br />

> **How it works**

`app/base/models.py` define the callback functions required by **Flask-Login** library:

```python
# File: app/base/models.py

@login_manager.user_loader
def user_loader(id):
    return User.query.filter_by(id=id).first()

@login_manager.request_loader
def request_loader(request):
    username = request.form.get('username')
    user = User.query.filter_by(username=username).first()
    return user if user else None

```

<br />

> **Usage in contoler** (Sample file)

```python

def sample_method(path):

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
