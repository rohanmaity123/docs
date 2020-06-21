# [AppSeed Docs](https://docs.appseed.us)

The official documentation repo for all web apps and boilerplate code 

<br />

## How to build the docs

The project uses [Mkdocs](https://www.mkdocs.org/) to generate the HTML pages from Markdown files. To build locally the project, Nodejs must be installed.

```bash
$ # Clone Sources
$ git clone https://github.com/app-generator/docs.git
$ cd docs
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install requirements (mkdoks & related extensions)
$ pip3 install -r requirements.txt
$
$ # Install modules
$ yarn
$
$ # Start the app
$ yarn start
$
$ # Please visit http://localhost:8000 in browser
```

<br />

## How to contribute

Each page provides *Edit on github* shortcut button in the top bar (see below). By clicking on it, the user is redirected to Github and invited to fork, edit the page and make a pull request to notify the owner that the content is updated.

![AppSeed Docs - Edit on Github Option.](https://raw.githubusercontent.com/app-generator/docs/master/static/docs-edit-page-option.jpg)

The *pull request* triggered by the change will be merged in the documentation after validation.

> For more information please contact the Support team on [Discord](https://discord.gg/fZC6hup) server.

<br />

## Latest Products

- [Flask Dashboard StarAdmin PRO](https://docs.appseed.us/admin-dashboards/flask-dashboard-staradmin-pro/) - product help, [LIVE Demo](https://flask-dashboard-staradmin-pro.appseed.us/)
- [Flask Dashboard StarAdmin Black PRO](https://docs.appseed.us/admin-dashboards/flask-dashboard-staradmin-black-pro/) - product help, [LIVE Demo](https://flask-dashboard-staradmin-black-pro.appseed.us/)
- [Flask Dashboard StarAdmin Boxed PRO](https://docs.appseed.us/admin-dashboards/flask-dashboard-staradmin-boxed-pro/) - product help, [LIVE Demo](https://flask-dashboard-staradmin-boxed-pro.appseed.us/)

<br />

## Latest Content Items

- [Flask Boilerplate](https://docs.appseed.us/boilerplate-code/flask/) - Help page
- [Flask Dashboard Boilerplate](https://docs.appseed.us/boilerplate-code/flask/) - Help page
- [Django Boilerplate](https://docs.appseed.us/boilerplate-code/django/) - Help page
- [Django Dashboard Boilerplate](https://docs.appseed.us/boilerplate-code/django-dashboard/) - Help page
- [Code a simple app in Flask](https://docs.appseed.us/tutorials/flask-understand-flask-code-simple-app/)
- [Install Python38 on Ubuntu](https://docs.appseed.us/how-to/install-python38-ubuntu/)
- [Admin Dashboards](https://docs.appseed.us/admin-dashboards/) - the index was updated with new items
- [Flask Dashboard Black](https://docs.appseed.us/admin-dashboards/flask-dashboard-black/) - product help
- [Flask Dashboard Argon](https://docs.appseed.us/admin-dashboards/flask-dashboard-argon/) - product help
- [Flask Dashboard Material](https://docs.appseed.us/admin-dashboards/flask-dashboard-material/) - product help
- [Flask Dashboard CoreUI](https://docs.appseed.us/admin-dashboards/flask-dashboard-coreui/) - product help

<br />

## Latest update - Mkdocs core

### [Support include of markdown files](https://github.com/mkdocs/mkdocs/issues/777)

> [Help Snippet](https://github.com/mkdocs/mkdocs/issues/777#issuecomment-308266201) - Extracted from Mkdocs Github repository

```yaml
# File: mkdocs.yml

markdown_extensions:
    - markdown_include.include:
        base_path: docs
```

**Usage**

```md
# File: Markdown File Sample

{!some/dir/in/docs/filename.md!}

```

<br />

---
[AppSeed Docs](https://docs.appseed.us) - Provided by the [AppSeed](https://appseed.us)
