## App Routing
---

The file **`app/views.py`** defines the application routing. Here is the list with defined paths and associated handlers

<br />

### Route `/login.html`

The route handles the app authentication using a simple flow:

- Loads `LoginForm` defined in `app/forms.py`
- GET request
    - loads the page `app/tempates/accounts/login.html`
- POST request
    - Validate the input data: `username`, `password`
    - Locate the user in the database
    - Verify the password against the database version
    - For success, authenticate the user
    - For errors, reload the login page and inform the user

<br />

### Route `/register.html`

The route handles the app authentication using a simple flow:

- Loads `RegisterForm` defined in `app/forms.py`
- GET request
    - loads the page `app/tempates/accounts/register.html`
- POST request
    - Validate the input data: `username`, `password`, `email`
    - Check if `username` or `email` is already registered
    - Hash the password provided by the user
    - Save the user in the database
    - Reload the registration page and inform the user

<br />

### Route `/logout.html`

The route delete the user session and redirect the user to the `login.html`

<br />

### Default Route `/`

The route will serve all pages defined in the `app/templates` for the authenticated users using a simple flow:

- Check user is authenticated
- Redirect to `/login.html` guests users
- Load the requested page from `app/templates` folder
- Return Error 404 and associated page if requested page cannot be located
- Return Error 500 if a critical error occurred during the page load

<br />
