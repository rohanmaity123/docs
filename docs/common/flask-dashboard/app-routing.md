## App Routing
---

The routing rules are defined by *Base* and *Home* blueprints as specified below. This is the public zone of the app.

> **Base Blueprint** - routing file `app/base/routes.py`

- `/login` route is resolved by `login()` method
- `/register` route is resolved by `register()` method
- `/logout` route calls the `logout_user()` defined in [flask_login](https://flask-login.readthedocs.io/en/latest/)

*Registered ERROR handlers*

- 404 Error - Page not found
- 403 Error - Access Forbidden
- 500 Error - Internal Error

<br />

> **Home Blueprint** - routing file `app/home/routes.py`

This blueprint will serve requested pages from `app/home/templates` directory to authenticated users. 
The authentication status is checked by `@login_required` decorator.

- `/<template>` route resolved by `route_template()`.
    - If a requested page is not found a default 404 page is returned to the user

<br />
