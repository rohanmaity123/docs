# Flask App - Heroku deploy
Learn how to deploy your app to Heroku

<br />

## What is Heroku
@Todo .. 
 
## App structure

```
<ROOT> / app.py
       / requirements.txt
       / Procfile
```

<br />

The contents of `app.py`
```
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello World!'

if __name__ == '__main__':
    app.run()
```

<br />

The contents of `requirements.txt`
```
Flask==1.0.2
gunicorn==19.9.0
```

<br />

The contents of `Procfile`
```
web: gunicorn app:app --log-file -
```

<br />

## Commands
Before running your app you must set the variable **FLASK_APP**, to inform Flask what should be executed first

### Check the installation 
 - `heroku login`

###  Create a new git project   
 - `git init`
 - `git add .`
 - `git commit -m "initial commit"`

### Create the project on heroku platform 
```
$
$ heroku create learn-flask-heroku-2
$
Creating ⬢ learn-flask-heroku-2... done
https://learn-flask-heroku-2.herokuapp.com/ | https://git.heroku.com/learn-flask-heroku-2.git
$
$
$ git push heroku master # commit changes to live
$
$ Counting objects: 5, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 509 bytes | 0 bytes/s, done.
Total 5 (delta 0), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote:
remote: -----> Python app detected
remote: -----> Installing python-3.6.8
remote: -----> Installing pip
remote: -----> Installing SQLite3
remote: -----> Installing requirements with pip
...
...
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote:
remote: -----> Compressing...
remote:        Done: 45.1M
remote: -----> Launching...
remote:        Released v3
remote:        https://learn-flask-heroku-2.herokuapp.com/ deployed to Heroku
remote:
remote: Verifying deploy... done.
```

### Live update

 - `git diff`
 - `git commit . -m "some message"`
 - `git push heroku master`
  


