## Pages & Assets
---

Pages served by the starter are organized using a simple folder structure:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app logic and serve the static assets
   |    |
   |    |-- static/assets/
   |    |    |-- css
   |    |    |-- JS
   |    |    |-- images
   |    |    |-- SCSS
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                  # Master pages
   |         |    |-- base-fullscreen.html # Used by Authentication pages
   |         |    |-- base.html            # Used by common pages
   |         |
   |         |-- accounts/                 # Authentication pages
   |         |    |-- login.html           # Login page
   |         |    |-- register.html        # Register page
   |         |
   |      index.html                       # The default page
   |     page-404.html                     # Error 404 page
   |     page-500.html                     # Error 404 page
   |       *.html                          # All other HTML pages
   |
   |-- app/                                # A simple app that serve HTML files
   |    |
   |    |-- views.py                       # Serve HTML pages for authenticated users
   |    |-- urls.py                        # Define some super simple routes  
   |
   |-- ************************************************************************
```

<br />

### Static Assets

The folder that contains all assets provided by the UI Kit is located in the `core` directory

- `static/assets` - the root directory for all files (JS, images)
- `static/assets/css` - CSS files that style the app
- `static/assets/img` - Images and Icons
- `static/assets/js` - javascript files provided by the UI Kit
- `static/assets/scss` - SCSS files, if provided by the UI Kit vendor

<br />

### `Templates` Folder

All pages served by the application are located inside this folder.

- `templates/layouts` - the directory with app masterpages
- `templates/includes` - the directory with HTML chunks and components
- `templates/accounts` - store the authentication pages (login, registration)
- `templates/` - all pages defined/served by the app are saved in the root of the `templates` folder

<br />

### Common pages

This section lists the common pages defined in all Flask applications prototyped on top of this generic starter.

- login.html, rendered with `layouts/base-fullscreen.html`
- register.html, rendered with `layouts/base-fullscreen.html`
- index.html, rendered with `layouts/base.html`
- page-404.html, rendered with `layouts/base.html`
- page-403.html, rendered with `layouts/base.html`

<br />
