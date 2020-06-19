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
$ # Create and activate a Virtualenv (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Create and activate a Virtualenv (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install requirements
$ pip3 install -r requirements.txt
$
$ # Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=run.py
$ (Windows) set FLASK_APP=run.py
$ (Powershell) $env:FLASK_APP = ".\run.py"
$
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$ # (Windows) set FLASK_ENV=development
$ # (Powershell) $env:FLASK_ENV = "development"
$
$ # Run the application
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the app in browser: http://127.0.0.1:5000/
```

At this point, we can visit the app in the browser **`http://127.0.0.1:5000/`**.
By default, the app will redirect guest users to the login page. To access the private pages:

- Create a new user using the **registration page**
- Authenticate using the **login page**

<br />

