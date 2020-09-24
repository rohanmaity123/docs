title: What is Django

---

# What is [Django](https://www.djangoproject.com/)
---

Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of Web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source.  

<br />

## Set up PC for [Django](https://www.djangoproject.com/)
---

Being a Python framework, Django requires Python to run and expose his magic. Django is compatible with Python2, Python3 (the recommended version).

<br />

**Install Python**

To get started working with Python3, you’ll need to have access to the Python interpreter (the console, and related tools and libraries). We can accomplish this in several ways:

- Download the installer from the official [download](https://www.python.org/downloads/) page.
- Use a package manager like yum, apt on Linux systems
- Homebrew for MacOS users.
- Build Python from sources, a method used by super-geeks.

<br />

### Install Python on Windows
---

To install Python on our windows workstation, a few simple steps should be followed:

- Navigate to the official [download](https://www.python.org/downloads/) page, using a web browser
- Select the installer that matches the OS (32b or 64b)
- Execute the installer (using the default options, should be enough in most of the cases)
- Test the installation by typing `python --version` in a terminal

<br />

### Install Python on Linux
---

There is a very good chance your Linux distribution has Python installed already, but it probably won’t be the latest version, and it may be Python 2 instead of Python3. To check the installed versions, just type:

```bash
$ python --version
$ python3 --version
```

<br />

### Install on CentOS
---

To install, you should first update your system with the `yum` package manager:

```bash
$ sudo yum install python36u
$ sudo yum install python36u-pip
```

If you still have issues set up your workstation for Python, feel free to join the [Discord](https://discord.gg/fZC6hup) server and ask for support.

<br />

**Other useful links**

- [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/) - hosted by RealPython
- [How to install Python](https://realpython.com/installing-python/) - a complete guide for many OS: Fedora, MacOS, Ubuntu

<br />

## Install [Django](https://www.djangoproject.com/)
---

To install Django, we can use `PIP`, the official Python package manager:

```bash
$ pip install Django
```

<br />

## [Django](https://www.djangoproject.com/) - A minimal Application
---

**How to check Django is installed**

```bash
$ python -m django --version
```

In case of any errors, just run the previous command `pip install Django`

<br />

**How to create first Django project**

```bash
$ django-admin startproject site1
```

This will create a **site1** directory in your current directory.

The files created by *startproject* command

```bash
site1/                  # The root directory (we can change the name)
    manage.py           # Django utility file
    site1/              # This is the actual Django project
        __init__.py     # 
        settings.py     # Store app settings
        urls.py         # Define app routes
        asgi.py         # Used in deployment 
        wsgi.py         # Used in deployment  
```

<br />

The meaning of each file:

- The outer `site1/` root directory is a container for your project. Its name is not important, we can rename it without causing any damages to the project.
- `manage.py`: A command-line utility that lets you interact with this Django project:
    - create databases
    - create migrations (for database updates)
- The inner mysite/ directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).
- `site1/__init__.py`: An empty file that tells Python that this directory should be considered a Python package. 
- `site1/settings.py`: Settings/configuration for this Django project. Django settings will tell you all about how settings work.
- `site1/urls.py`: The URL declarations for this Django project; a “table of contents” of your Django-powered site. 
- `site1/asgi.py`: An entry-point for ASGI-compatible web servers to serve your project. 
- `site1/wsgi.py`: An entry-point for WSGI-compatible web servers to serve your project. 

<br />

**Start the app**

```bash
$ python manage.py runserver
```

At this point we have the most simple Django project, up and running. 

<br />

## Django Seed Projects
---

- [Django Dashboard Argon](/admin-dashboards/django-dashboard-argon/) - open-source project
- [Django Dashboard Black](/admin-dashboards/django-dashboard-black/) - open-source project
- [Django Dashboard Atlantis](/admin-dashboards/django-dashboard-atlantis/) - open-source project
- [Django Dashboard CoreUI](/admin-dashboards/django-dashboard-coreui/) - open-source project
- [Django Dashboard Light](/admin-dashboards/django-dashboard-light/) - open-source project

<br />

### [Django](https://www.djangoproject.com/) - Resources & Support
---

- [Django](https://www.djangoproject.com/) - the official page
- [Django Tutorial](https://docs.djangoproject.com/en/3.1/intro/tutorial01/) - learn Django by coding a simple project
- For assistance, feel free to join [AppSeed](https://appseed.us/) platform
- Join [Discord](https://discord.gg/fZC6hup) for LIVE Support - 24/7 Service
