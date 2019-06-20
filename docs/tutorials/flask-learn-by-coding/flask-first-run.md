# Flask App - First Run
This article describe the minimum required setup to have a running Flask application.

<br />

## Project structure
The minimal project requires only two files: `run.py` (the app launcher) and `__init__.py` the init file for our app
 
```
<ROOT> / run.py
       / app /
       / app / __init__.py
```

<br />

The contents of `run.py`
```
from app import app

if __name__ == "__main__":
    app.run()
```

<br />

The contents of `__init__.py`
```
from app import app

if __name__ == "__main__":
    app.run()
```

<br />

## Environment set up
Before running your app you must set the variable **FLASK_APP**, to inform Flask what should be executed first

 - Set up for Unix: `export FLASK_APP=run.py`
 - Set up for Windows CMD `set FLASK_APP=hello.py` 
 - Set up for Windows Powershell `$env:FLASK_APP = "run.py"` 

<br />

Navigate to the directory where `run.py` was saved, and type **`flask run`**.
By visiting `locahost:5000` in your preferred browser you should see the app running.

<br />



### Related content
---
 - [Integrate a design](/tutorials/flask-learn-by-coding/flask-integrate-design)
 - Tutorial [Home page](/tutorials/flask-learn-by-coding/)
