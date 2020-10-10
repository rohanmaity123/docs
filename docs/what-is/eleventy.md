title: What is Eleventy (11ty)

# What is Eleventy [Eleventy](https://www.11ty.io/)
---

Eleventy was created to be a JavaScript alternative to Jekyll. It’s zero-config by default but has flexible configuration options. Eleventy works with your project’s existing directory structure.

Unlike other JavaScript web frameworks like Gatsby or NuxtJS, 11ty doesn’t come bundled with a front-end library. 11ty is more like a traditional SSG (such as Hugo or Jekyll) where it takes a series of templates, markdown files, and data and renders HTML files to serve.

Eleventy uses independent template engines. We don’t want to hold your content hostage. If you decide to use something else later, having your content decoupled in this way will make migration easier. Eleventy works with multiple template languages. You can pick one or use them all together in a single project: `html`, `Markdown`, `Liquid`, `Mustache`.

<br />

## Eleventy - Reasons to use it
---

Eleventy is a static site generator created for three main reasons (according to the creator, Zach Leaterman)

**Flexibility**

Eleventy allows you to mix and match templating engines to allow easy migration of existing content. Your content templates can use a different templating engine than your layout files!

Previous SSG's are tied to a single template language, as a rule. Jekyll uses Liquid, Hugo uses Go Templates and Gatsby is React entirely.
Eleventy innovates and empower the developer to use his preferred language from a long list:

- HTML
- Markdown
- Liquid (used by Jekyll)
- Nunjucks
- Handlebars
- Mustache
- EJS
- Haml
- Pug

<br />

**Directory structure flexibility**

Eleventy wants to work with your project’s existing directory structure. Is not mandatory to save your content files in a `_posts` directory or a source folder (unless you really want to). You tell Eleventy where your files are and we’ll work with you. This is pretty nice!

All you need to do is to execute `eleventy` and all files from the current directory are translated to `_site` folder. 
This can be customized with ease using `--input` and `--output` arguments. 

<br />

**Eleventy is Javascript**

JavaScript gives you access to npm, a massive ecosystem with many modules and libraries built by open-source enthusiasts.
While Eleventy uses JavaScript in node.js to transform templates into content, importantly (by default) it does not recommend nor force your HTML to include any Eleventy-specific client-side JavaScript.

<br />

## [Install Eleventy](https://www.11ty.io/docs/getting-started/#step-2-install-eleventy)
---

Ready to start? You're one line away:

```bash
$ npm install -g @11ty/eleventy # global installation
```

<br />

## [Eleventy (11ty) starters](/static-site/)
---

- [Static Site Eleventy Ethereal](/static-site/eleventy-html5up-ethereal/) 
    - SSG: Eleventy (11ty) 
    - [HTML5up](https://appseed.us/apps/html5up) Ethereal design 
    - Tooling: Webpack, Babel, LightServer and CSS processors.
- [Static Site Eleventy Paradigm](/static-site/eleventy-html5up-paradigm/) 
    - SSG: Eleventy (11ty) 
    - [HTML5up](https://appseed.us/apps/html5up) Paradigm design 
    - Tooling: Webpack, Babel, LightServer and CSS processors.
- [Static Site Eleventy Highlights](/static-site/eleventy-html5up-highlights/)
    - SSG: Eleventy (11ty) 
    - [HTML5up](https://appseed.us/apps/html5up) Helios design 
    - Tooling: Webpack, Babel, LightServer and CSS processors.
- [Static Sites](https://appseed.us/static-site) - built with **11ty**

<br />

## Eleventy Sample - [Html5 Ethereal](https://appseed.us/static-site/eleventy-html5up-ethereal)
---

Static Site prototyped on top of [Eleventy](https://www.11ty.io/) SSG and Ethereal Design. Boilerplate features:

- Design: HTML5up Ethereal
- SSG: [11ty](https://www.11ty.io/)
- Webpack, Babel
- Light-server - for browser refresh
- PostCSS, Sass/SCSS, CSSnano
- Autoprefixer

<br />

**Links**

- [Eleventy Ethereal](https://appseed.us/static-site/eleventy-html5up-ethereal) - the product page
- [Eleventy Ethereal - Demo](https://eleventy-html5up-ethereal.appseed.us/) - the product page
- [Eleventy Ethereal - Sources](https://github.com/app-generator/eleventy-html5up-ethereal) - the product page

<br />

![Eleventy Html5UP Ethereal - Static Site built in Eleventy.](https://raw.githubusercontent.com/app-generator/eleventy-html5up-ethereal/master/media/eleventy-html5up-ethereal-screen.png)

<br />

## Eleventy (11ty) Links

- [11ty](https://www.11ty.io/) - official website
- [11ty](https://www.11ty.io/docs/) - documentation
- [11ty](https://github.com/11ty/eleventy/) - the Github repository
