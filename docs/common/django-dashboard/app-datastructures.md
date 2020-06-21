## Data Structures
---

The starter exposes a short-list with data structures used globally across the app:

<br />

### `request.user` object

Constructed by [AuthenticationMiddleware](https://docs.djangoproject.com/en/3.0/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) can be used to detect if the current request is executed by an authenticated user or not. The object has global visibility and can be used in all app controllers and handlers but also in views.

<br />

> **Usage in contoler**

```python
# Sample File

from django.http import HttpResponse

def testme(path):

    # Redirect guests users to login page
    if request.user.is_authenticated:
        return HttpResponse("User authenticated")
    else:
        return HttpResponse("Access forbidden - please authenticate")
```

<br />

> **Usage in view**

```html
    <div class="collapse navbar-collapse" id="navigation">
        <ul class="navbar-nav ml-auto">

        <!-- The Usage of <current_user> object -->
        {% if request.user.is_authenticated %}

            <!-- Html chunk rendered for authenticated users-->

            <li class="nav-item">
                <a href="/" class="nav-link text-primary">
                    <i class="tim-icons icon-minimal-left"></i> Your Dashboard
                </a>
            </li>

        {% else %}

            <!-- Html chunk rendered for guests users-->

            <li class="nav-item ">
                <a href="{% url 'register' %}" class="nav-link">
                    <i class="tim-icons icon-laptop"></i> Register
                </a>
            </li>
            <li class="nav-item ">
                <a href="{% url 'login' %}" class="nav-link">
                    <i class="tim-icons icon-single-02"></i> Login
                </a>
            </li>

        {% endif %}

        </ul>
    </div>
```

<br />
