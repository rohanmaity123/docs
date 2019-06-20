# Setup Environment
This article, part of the **[Flask - learn by coding](/tutorials/flask-learn-by-coding/index.md)** tutorial, describes hot to organize your future project.

<br />

## Well-Known project Structures
--- 
With Flask, you have the freedom to organize your files in your own way. Total freedom, in other words.

<br />

### Single module structure
---
Suitable for small project, or learning projects, where the minimum number of files are saved in the same directory: 

<br />

```
<ROOT> / app.py
       / config.py
       / requirements.txt
       / static/
       / templates/
```

<br />

### Basic Package structure
---
When you’re working on a project that’s a little more complex, a single module can get messy. You’ll need to define classes for models and forms, and they’ll get mixed in with the code for your routes and configuration.

<br />

```
<ROOT> / run.py
       / requirements.txt
       / 
       / app / __init__.py 
             / views.py
             / models.py
             / forms.py
             / static/ 
             / templates/ 
```
We can see now a much more organized directory structure where each file represents:

 - run.py - script responsible to bundle and start the whole app
 - requirements.txt - the file where all the project requirements are listed
 - app / __init__.py - the Init file that signals to Pyhton that we have a package in the `app` directory  

For our project we will choose the second pattern **Basic Package structure**

<br /> 

### Links
---
 - [First run](/tutorials/flask-learn-by-coding/flask-first-run)
 - Tutorial [Home page](/tutorials/flask-learn-by-coding/)
