# Customize Django Admin Interface

<br>

## Download your favorite template
Download your favorite template which usually contains **css**, **js**, **images** and **fonts** files.
For example, I used one of the ready-made and very beautiful [Creative-Tim](https://www.creative-tim.com/) templates.

I used the free version of **[Black Dashboard](https://www.creative-tim.com/product/black-dashboard)** Template.

![Django Admin Black](https://raw.githubusercontent.com/app-generator/django-dashboard-black/master/media/django-dashboard-black-screen.png)

> Please note that you may have to change the template slightly to do this. Because the relevant template must be usable for Django Admin features.

<br>

## Let's Start
Create a Django project to start. Then make a new application in it with the a name (note it can be anything like 'admin_black'):

```bash
$ python manage.py startapp admin_black
```

* Make a 'templates', 'static' and 'templatetages' folders in it. The application folders structure is like this:

```
admin_black/
    migrations/
        __init__.py
    static/
        # we gonna add something here
    templates/
        # we gonna add something here
    templatetags/
        __init__.py
        # we gonna add something here
    __init__.py
    admin.py
    apps.py
    models.py
    tests.py
    utils.py  # To add public and commonly used functions.
    views.py
```

* Add your application (admin_black) to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'django.contrib.admin'):

```python
INSTALLED_APPS = [
    # ...
    'admin_black.apps.AdminBlackConfig',
    'django.contrib.admin',
]
```

* Now your application is ready to add a template. To do this, you need to add your template assets files like **css**, **js**, **images** and **fonts** in your application static folder.
> The folders' structure of this section is completely arbitrary.

```
admin_black/
    ...
    static/
        admin/ # In this section you can override the admin assets file like css, js and etc.
            css/
        admin_black/  # This section is for your template assets. You can choose your own name.
            assets/
                css/
                demo/
                fonts/
                img/
                js/
                scss/
            LICENSE.md
        libs/  # this section is for libs like jQuery, jQuery-confirm or etc
    ...
```

> This is my structure and you can make your own structure.

<br>

## Let's Override Django Admin Templates
* In the previous, we added all the required information to our project. Now we want to override the Django admin template and add our template.
To do this, you need to know that all Django admin template files are located at:

```djangourlpath
venv/lib64/python3.6/site-packages/django/contrib/admin/templates
```

In this section you will see two folders that include **admin** and **registration**.
As it is clear from the name, the **admin** folder is related to the admin templates and the **registration** folder is related to registration, such as *password_reset_form.html*, *logged_out.html* and etc templates.

* In Django admin, to override the templates, just create the same files with the same address in your application. For example, to change the *base.html*, just create such a file in your application:

```
admin_black/
    ...
    templates/
        admin/
            base.html  # change this
        registration/
    ...
```

> Note that you must pay attention to the blocks.

* base.html is a file that you can start with. All other files import this file to use assets. So, you can add your own template files in it.
> Note you can create your own blocks.

**base.html:** *meta*, *css*, *fonts* and etc
```html
<!DOCTYPE html>
<html lang="{{ LANGUAGE_CODE|default:"en-us" }}">

<head>
    <meta charset="utf-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <link rel="apple-touch-icon" sizes="76x76" href="{% static "admin_black/assets/img/apple-icon.png" %}">
    <link rel="icon" type="image/png" href="{% static "admin_black/assets/img/favicon.png" %}">

    <title>{% block title %}{% endblock %}</title>

    <link href="https://fonts.googleapis.com/css?family=Poppins:200,300,400,600,700,800" rel="stylesheet"/>
    <link href="https://use.fontawesome.com/releases/v5.0.6/css/all.css" rel="stylesheet">

    {% if LANGUAGE_BIDI %}
        <link href="{% static "admin_black/assets/css/bootstrap-rtl.css" %}" rel="stylesheet"/>
    {% endif %}

    <link href="{% static "admin_black/assets/css/nucleo-icons.css" %}" rel="stylesheet"/>
    <link href="{% static "admin_black/assets/css/black-dashboard.css" %}" rel="stylesheet"/>
    <link href="{% static "admin_black/assets/demo/demo.css" %}" rel="stylesheet"/>
    <link href="{% static "admin_black/assets/css/styles.css" %}" rel="stylesheet"/>

    {% block extrastyle %}{% endblock %}
    {% block extrahead %}{% endblock %}
    {% block blockbots %}
        <meta name="robots" content="NONE,NOARCHIVE">
    {% endblock %}
</head>
```

**base.html:** *Javascripts*, *jQuery* and etc.
```html
...
<script src="{% static "admin_black/assets/js/core/jquery.min.js" %}"></script>
<script src="{% static "admin_black/assets/js/core/popper.min.js" %}"></script>
<script src="{% static "admin_black/assets/js/core/bootstrap.min.js" %}"></script>
<script src="{% static "admin_black/assets/js/plugins/perfect-scrollbar.jquery.min.js" %}"></script>
<script src="{% static "admin_black/assets/js/plugins/chartjs.min.js" %}"></script>
<script src="{% static "admin_black/assets/js/plugins/bootstrap-notify.js" %}"></script>
<script src="{% static "admin_black/assets/js/black-dashboard.min.js" %}"></script>
<script src="{% static "admin_black/assets/demo/demo.js" %}"></script>
<script src="https://cdn.trackjs.com/agent/v3/latest/t.js"></script>
<script src="{% static "admin_black/assets/js/scripts.js" %}"></script>

{% block extrascript %}{% endblock %}
</body>
</html>
```

> Note that in sections head and footer I created a new block so that I can make changes to these sections on other pages.

* **You see**. It is not very difficult. You can do this on other pages as well, and even change parts of HTML.
You can also use **templatetags** to do some things. For example, I used a **templatetags** to create dashboards sidebar and navigation.
To do this, I created a file with the name in admin_black.py in templatetags folder and I import it wherever I want to use it, like this:

```
admin_black/
    ...
    templatetags/
        __init__.py
        admin_black.py
    ...
```

**sidebar.html**
```html
{% load admin_black %}

<div class="sidebar">
    <div class="sidebar-wrapper">
        ...
        {% admin_black_get_menu as app_list %}
        {% if app_list %}
            ...
        {% endif %}
        ...
    </div>
</div>
```

* This way you can override the Django admin template and import your own template.


<br>

## Author
* This part was written by **[Iman Karimi](https://www.linkedin.com/in/iman-karimi/)**.
