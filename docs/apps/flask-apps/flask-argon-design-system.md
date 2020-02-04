title: Flask Argon Design

# [Flask Argon Design](https://appseed.us/apps/flask-apps/flask-argon-design-system)

**Open-Source Web App** coded in **[Flask Framework](https://palletsprojects.com/p/flask/)** - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

## App Features
---

- UI-Ready, modular code-base
- SQLite, SQLAlchemy ORM
- Session-Based authentication (via **flask_login**)
- Forms validation
- CCA 3.0 License - preserve the footer links (Html5UP, AppSeed)

<br />

## App technology stack
---

- Used Language: [Python3](https://www.python.org/) (Python2 is not supported)
- Web Framework: [Flask](https://www.palletsprojects.com/p/flask/)
- CSS Framework: [Bootstrap CSS](https://getbootstrap.com/)
- Javascript: [jQuery](https://jquery.com/)

<br />

## App Links
---

- [Flask Argon Design](https://appseed.us/apps/flask-apps/flask-argon-design-system) - the product page
- [Flask Argon Design](https://github.com/app-generator/flask-argon-design-system) - the source code
- [Flask Argon Design](https://www.youtube.com/watch?v=PSYbGPvztJ8) - yTube presentation

![Flask Argon Design - Open-Source Web App.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-argon-design-system-screen.png)

<br />

## Prepare your environment
---

The product is built on top of [Flask](https://palletsprojects.com/p/flask/), a popular Python Web Framework. To build the app, Python3 should be installed properly in the workstation. If you are not sure if Python is properly installed, please open a terminal and type `python --version`. The full-list with dependencies and tools required to build the app:

- [Python3](https://www.python.org/) - the programming language used to code the app
- [Git](https://git-scm.com/) - used to clone the source code from the Github repository
- A [Github](https://github.com/) account - the invitation to the source code, will be sent on your account.
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment. 

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

## Support
---

- Free support via eMail < [support @ appseed.us](https://appseed.us/support) > and **Github** issues tracker
- (Paid) LIVE 24/7 Support via [Discord](https://discord.gg/fZC6hup)

<br />

## Credits & Links
---

- [Flask Html5Up Phantom](https://appseed.us/admin-dashboards/flask-argon-design-system) - Product page
- [Flask Framework](https://www.palletsprojects.com/p/flask/) - Offcial website
- [Flask Admin Dashboards](https://appseed.us/admin-dashboards/flask) - provided by AppSeed

<br />

## License
---

@MIT

<br />

## Flask Html5Up Phantom - app screens
---

<br />

![Flask Html5Up Phantom - Calendar Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-argon-design-system-screen-1.png)

<br />

![Flask Html5Up Phantom - Charts Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-argon-design-system-screen-2.png)

<br />

![Flask Html5Up Phantom - Maps Page.](https://raw.githubusercontent.com/app-generator/static/master/products/flask-argon-design-system-screen-3.png)

<br />

---
[Flask Argon Design](https://appseed.us/apps/flask-apps/flask-argon-design-system) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
