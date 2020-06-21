## Build the app
---

To built and start the app locally, follow the steps:

> **Get the source code**

- Download the ZIP from Github Repository
- Using GIT tool in the terminal to clone the source code

> **Change the current directory** to `source code` directory

```bash
$ # Make sure you are running the commands INSIDE source code directory
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install modules - SQLite Storage
$ pip3 install -r requirements.txt
$
$ # Create tables
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
$
$ # Start the app - custom port
$ # python manage.py runserver 0.0.0.0:<your_port>
$
$ # Access the web app in browser: http://127.0.0.1:8000/
```

At this point, we can visit the app in the browser **`http://127.0.0.1:8000/`**.
By default, the app will redirect guest users to the login page. To access the private pages:

- Create a new user using the **registration page**
- Authenticate using the **login page**

<br />

