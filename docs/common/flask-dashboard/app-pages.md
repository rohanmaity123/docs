## Pages & Assets
---

Pages and all assets defined in the UI Kits are served by the app using both blueprints:

- *Home Blueprint* manage the static assets - `app/base/static/assets`
- *Home Blueprint* store the layout `master pages`, HTML chunks (footer. header, scripts) and `login, registration` pages

- *Base Blueprint* serve the HTML pages (index, page-404, etc) and the rest of the pages defined in the UI kit.


```bash
< PROJECT ROOT >
   |
   |-- app/
   |    |-- base/                               # Base Blueprint
   |    |    |-- static/assets/
   |    |    |           |-- css/               # UI Kit css
   |    |    |           |-- JS/                # Javascript files
   |    |    |           |-- images/            # images used by the app
   |    |    |           |-- scss/              # SCSS files (if any)
   |    |    |
   |    |    |-- templates/                      # Templates used to render pages
   |    |         |
   |    |         |-- includes/                  #
   |    |         |    |-- navigation.html       # Top menu component
   |    |         |    |-- sidebar.html          # Sidebar component
   |    |         |    |-- footer.html           # App Footer
   |    |         |    |-- scripts.html          # Scripts common to all pages
   |    |         |
   |    |         |-- layouts/                   # Master pages
   |    |         |    |-- base-fullscreen.html  # Used by Authentication pages
   |    |         |    |-- base.html             # Used by common pages
   |    |         |
   |    |         |-- accounts/                  # Authentication pages
   |    |              |-- login.html            # Login page
   |    |              |-- register.html         # Registration page
   |    |
   |    |-- home/                                # Home Blueprint - serve app pages (private area)
   |         |-- templates/                      # UI Kit Pages
   |              |
   |              |-- index.html                 # Default page
   |              |-- page-404.html              # Error 404 - mandatory page
   |              |-- page-500.html              # Error 500 - mandatory page
   |              |-- page-403.html              # Error 403 - mandatory page
   |              |-- *.html                     # All other HTML pages
   |
   |-- ************************************************************************
```

<br />
