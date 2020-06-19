## Pages & Assets
---

Pages served by the starter are organized using a simple folder structure:

```bash
< PROJECT ROOT >
   |
   |-- app/
   |    |
   |    |-- static/assets/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/
   |    |    |
   |    |    |-- includes/                 # Page chunks, components
   |    |    |    |
   |    |    |    |-- navigation.html      # Top bar
   |    |    |    |-- sidebar.html         # Left sidebar
   |    |    |    |-- scripts.html         # JS scripts common to all pages
   |    |    |    |-- footer.html          # The common footer
   |    |    |
   |    |    |-- layouts/                  # App Layouts (the master pages)
   |    |    |    |
   |    |    |    |-- base.html            # Used by common pages like index, UI
   |    |    |    |-- base-fullscreen.html # Used by auth pages (login, register)
   |    |    |
   |    |    |-- accounts/                 # Auth Pages (login, register)
   |    |    |    |
   |    |    |    |-- login.html           # Use layout `base-fullscreen.html`
   |    |    |    |-- register.html        # Use layout `base-fullscreen.html`  
   |    |    |
   |    |  index.html                      # The default page
   |    |  page-404.html                   # Error 404 page (page not found)
   |    |  page-500.html                   # Error 500 page (server error)
   |    |    *.html                        # All other pages provided by the UI Kit
   |
   |
   |-- ************************************************************************
```

<br />

### Static Assets

The folder contains the assets provided by the UI Kit integrated into the app. AppSeed conversion scripts will modify the original UI kit path to match the structure:

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
