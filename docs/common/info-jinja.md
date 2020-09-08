## [What is Jinja](/what-is/jinja/)
---

[Jinja](https://jinja.palletsprojects.com/en/2.11.x/) is a modern and designer-friendly templating language for Python, modelled after Django’s templates. It is fast, widely used and secure with the optional sandboxed template execution environment. Jinja is basically an engine used to generate HTML or XML returned to the user via an HTTP response.

For those who have not been exposed to a templating language before, such languages essentially contain variables as well as some programming logic, which when evaluated (or rendered into HTML) are replaced with actual values. 

<br />

## Why do we need [Jinja](https://jinja.palletsprojects.com/en/2.11.x/)?
---

**Sandboxed Execution** - It provides a protected framework for automation of testing programs, whose behavior is unknown and must be investigated.

**HTML Escaping** -  Jinja has a powerful automatic HTML Escaping, which helps to prevent Cross-site Scripting (XSS Attack). There are special characters like >,<,&, etc. which carry special meanings in the templates. So, if you want to use them as regular text in your documents then, replace them with entities. Not doing so might lead to XSS-Attack.

**Template Inheritance** - This feature helps us to generate new pages starting from a base template that we inherit a common structure.

<br />

## [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) Environment 
---

Being a Python library, Jinja requires Python to run and expose the features. If you're not sure if Python is installed, just open a terminal and type `python --version`. The output should be something like this:

```bash
$ # Check Python version
$ python --version
Python 3.7.2 # <--- All good
```

For a workstation set up, it might be a good idea to take a look at the below links and get back here when your PC is ready for development. In case we've missed something, contact us on [Discord](https://discord.gg/fZC6hup).

- [How to set up Python](/how-to/install-python)
- [Setup CentOS for development](/how-to/setup-centos-for-development/)
- [Setup Ubuntu for development](/how-to/setup-ubuntu-for-development/)
- [Setup Windows for development](/how-to/setup-windows-for-development/)

<br />

**How to get Jinja2**

To start playing with it, just open a terminal and type:

```bash
$ pip install jinja2
```

<br />

**Jinja in action**

Simple runtime replace

```python
>>> from jinja2 import Template
>>> t = Template("Hello {{ token }}!")
>>> t.render(token="Jinja2")
u'Hello Jinja2!'
```

The engine will replace the inner token with value Jinja2. This is quite useful when we use this block for different token values.

<br />
