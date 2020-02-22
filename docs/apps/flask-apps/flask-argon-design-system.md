title: Flask Argon Design

# [Flask Argon Design](https://appseed.us/apps/flask-apps/flask-argon-design-system)

**Open-Source Web App** coded in **[Flask Framework](https://palletsprojects.com/p/flask/)** on top of **Argon Design System** design (free version) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

## App Features
---

- UI-Ready, SQLite database
- SQLAlchemy ORM
- Session-Based authentication flow (login, register)
- Forms validation
- UI Kit: **[Argon Design System](https://flask-argon-design-system.appseed.us/login.html)** (Free version) provided by **Creative-Tim**
- **MIT License**
- Support: Free support via **Github** and (Paid) **24/7 LIVE Support** via [Discord](https://discord.gg/fZC6hup)

<br />

## App technology stack
---

- Used Language: [Python3](https://www.python.org/)
- Web Framework: [Flask](https://www.palletsprojects.com/p/flask/)
- CSS Framework: [Bootstrap CSS](https://getbootstrap.com/)
- Javascript: [jQuery](https://jquery.com/)

<br />

## App Links
---

- [Flask Argon Design](https://appseed.us/apps/flask-apps/flask-argon-design-system) - Product page
- [Flask Argon Design](https://github.com/app-generator/flask-argon-design-system) - Source code (published on Github)
- [Flask Argon Design](https://flask-argon-design-system.appseed.us/login.html) - LIVE demo

<br />

![Flask Argon Design - Open-Source Web App.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-argon-design-system-screen.png)

<br />

## Prepare your environment
---

The product is built on top of [Flask](https://palletsprojects.com/p/flask/), a popular Python Web Framework. To build the app, Python3 should be installed properly in the workstation. If you are not sure if Python is properly installed, please open a terminal and type `python --version`. The full-list with dependencies and tools required to build the app:

- [Python3](https://www.python.org/) - the programming language used to code the app
- [Git](https://git-scm.com/) - used to clone the source code from the Github repository
- A [Github](https://github.com/) account - the invitation to the source code, will be sent on your account.
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment.

<br />

> Check Python (using the terminal)

```bash
$ # Check Python version
$ python --version
Python 3.7.2 # <--- All good
```

<br />

> Check GIT command tool (using the terminal)

```bash
$ # Check git
$ git --version
$ git version 2.10.1.windows.1 # <--- All good
```

<br />

For more information on how to set up your environment please access the resources listed below. In case we've missed something, contact us on Discord.

- [How to set up Python](/how-to/install-python)
- [Setup CentOS for development](/how-to/setup-centos-for-development/)
- [Setup Ubuntu for development](/how-to/setup-ubuntu-for-development/)
- [Setup Windows for development](/how-to/setup-windows-for-development/)

<br />


## Project Structure
---

The boilerplate code is built with a modular structure that follows the recommended pattern used by many open-source projects. The most important files and  directories are shown below:

<br />

```bash
< PROJECT ROOT >                            # application root folder
    |
    |--- app/__init__.py                    # application constructor  
    |--- app//static                        # Assets Directory: Img, CSS, Javascript, sitemap.xml
    |--- app/templates                      # Jinja2 files
    |            |---<includes>             # Page chunks, components (footer, navigation)
    |            |---<layouts>              # Layouts (default.html)
    |            |---<accounts>             # Authentication Pages
    |            |     |---- login.html     # Login page
    |            |     |---- register.html  # Register page
    |            |
    |            |---<pages>                # Pages
    |                  |---- index.html     # Index page
    |                  |---- about.html     # Simple about page
    |                  |---- elements.html  # UI Kit elements
    |
    |--- requirements.txt                   # Modules and dependencies
    |
    |--- run.py                             # bootstrap the app
    |
    |-----------------------------
```

<br />

## How to use it
---

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/flask-argon-design-system.git
$ cd flask-argon-design-system
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv --no-site-packages env
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

<br />

## Credits & Links
---

<br />

### [Flask Framework](https://www.palletsprojects.com/p/flask/)

[Flask](/what-is/flask) is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions.

<br />

## [What is dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))

In information technology, a **[dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))** is a user interface that, somewhat resembling an automobile's dashboard, organizes and presents information in a way that is easy to read. However, a computer dashboard is more likely to be interactive than an automobile dashboard (unless it is also computer-based). To some extent, most graphical user interfaces (GUIs) resemble a dashboard - by [Techtarget](https://searchcio.techtarget.com/definition/dashboard)

<br />

### [Argon Design System](https://www.creative-tim.com/product/argon-design-system)

Free and open-source design system for Bootstrap4 - Argon Design System is built with over 100 individual components, giving you the freedom of choosing and combining. All components can take variations in color, that you can easily modify using SASS files. Start your development with a Design System for Bootstrap 4. It is open-source, free and it features many components that can help you create amazing websites - provided by **Creative-Tim**.

<br />

---
[Flask Argon Design](https://appseed.us/apps/flask-apps/flask-argon-design-system) - Provided by AppSeed [Web App Generator](https://appseed.us/app-generator).
