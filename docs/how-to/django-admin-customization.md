# Customize Django Admin Interface

<br>

## Download your favorite template
Download your favorite template which usually contains **css**, **js**, **images** and **fonts** files.
For example, I used one of the ready-made and very beautiful [Creative-Tim](https://www.creative-tim.com/) templates.

I used the free version of **[Black Dashboard](https://www.creative-tim.com/product/black-dashboard)** Template.

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


## Let's Override Admin Template
* In the previous, we added all the required information to our project. Now we want to override the Django admin template and add our template.
To do this, you need to know that all Django admin template files are located at:

```djangourlpath
venv/lib64/python3.6/site-packages/django/contrib/admin/templates
```

In this section you will see two folders that include **admin** and **registration**.
As it is clear from the name, the **admin** folder is related to the admin templates and the **registration** folder is related to registration, such as *password_reset_form.html*, *logged_out.html* and etc templates.


