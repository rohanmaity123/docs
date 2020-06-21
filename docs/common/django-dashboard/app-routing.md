## App Routing
---

The settings file **`core/settings.py`** specify the routing file `core/urls.py` via *ROOT_URLCONF* variable:

```python
# File: core/settings.py
...

ROOT_URLCONF = 'core.urls'

...
```

<br />

> **`core/urls.py`** file

The core routing file agregates the routing from all apps defined in the project:

```python
# File: core/urls.py

urlpatterns = [
    # Django admin routes - inherited from Django default modules
    path('admin/', admin.site.urls),

    # Authentication routes - login / register
    # exposed by `authentication` app
    path("", include("authentication.urls")),

    # App routes - the modules that serve the UI Kit pages
    path("", include("app.urls"))
]

```

<br />
