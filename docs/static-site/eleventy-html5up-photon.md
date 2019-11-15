title: Static Site Eleventy Photon

# [Static Site Eleventy Photon](https://appseed.us/static-site/eleventy-html5up-photon)

Static Site prototyped on top of [Eleventy](https://www.11ty.io/) SSG and Photon Design. Boilerplate features:

- Design: HTML5up Photon
- SSG: [11ty](https://www.11ty.io/)
- Webpack, Babel
- Light-server - for browser refresh
- PostCSS, Sass/SCSS, CSSnano
- Autoprefixer

<br />

![Eleventy Html5UP Photon - Static Site built in Eleventy.](https://raw.githubusercontent.com/app-generator/static/master/products/eleventy-html5up-photon-intro.gif)

## Setup the environment
---

In order to use this boilerplate, [Node.js](https://nodejs.org/en/), the `JavaScript runtime`, should be properly installed on the target machine and [Yarn](https://yarnpkg.com/) builder.

### CentOS setup

```bash
$ 
$ # install Nodejs
$ sudo yum install nodejs  
$ 
$ # Install Yarn
$ sudo npm install yarn -g
$
$ # Install npm-run-all
$ sudo npm install npm-run-all -g
```

<br />

### Ubuntu setup

```bash
$ 
$ # install Nodejs
$ sudo apt-get install nodejs  
$ 
$ # Install Yarn
$ sudo npm install yarn -g
$
$ # Install npm-run-all
$ sudo npm install npm-run-all -g
```

<br />

## Build from [sources](https://github.com/app-generator/eleventy-html5up-photon)

```bash
$ # clone the sources
$ git clone https://github.com/app-generator/eleventy-html5up-photon.git
$ cd eleventy-html5up-photon
$
$ # install modules
$ yarn
$
$ # start the project in development mode
$ yarn dev
$ # app is running on http://localhost:4000
$
$ # build the project for production
$ yarn build
```

<br />

## Project Structure

---

The boilerplate code is built with a modular structure that follows the recommended pattern used by many open-source projects. The most important files / directories are listed bellow:

- [.eleventy.js](https://github.com/app-generator/eleventy-html5up-photon/blob/master/.eleventy.js)
- [package.json](https://github.com/app-generator/eleventy-html5up-photon/blob/master/package.json)
- [src /](https://github.com/app-generator/eleventy-html5up-photon/tree/master/src)
- [src / _includes](https://github.com/app-generator/eleventy-html5up-photon/tree/master/src/_includes)
- [src / assets](https://github.com/app-generator/eleventy-html5up-photon/tree/master/src/assets)
- [src / data / data.json](https://github.com/app-generator/eleventy-html5up-photon/blob/master/src/_data/data.json)
- [src / index.njk](https://github.com/app-generator/eleventy-html5up-photon/blob/master/src/index.njk)

<br />

```bash
< ROOT > - Eleventy Photon      # project root folder
    |
    |--- src/                     # website source folder  
    |--- src/_includes            # website partials (footer, header)  
    |--- src/assets               # website assets (scss, javascript files)
    |--- src/index.njk            # index page in NJK format
    |  
    |--- .eleventy.js             # Eleventy (11ty) config file
    |--- package.json             # main script executed by Yarn, Npm
    |
    |-----------------------------
```

<br />

## Support

---

- Free support via eMail < [support @ appseed.us](https://appseed.us/support) > and [Github](https://github.com/app-generator/flask-argon-dashboard/issues/)
- 24/7 Live Support via [Discord](https://discord.gg/fZC6hup) for paid plans and commercial products.

<br />

## Resources

---

- [Eleventy Photon](https://appseed.us/static-site/eleventy-html5up-photon) - Product page
- [Eleventy Photon](https://eleventy-html5up-photon.appseed.us) - Live DEMO
- [Eleventy Photon](https://github.com/app-generator/eleventy-html5up-photon) - The source code

<br />

## License & Credits

---

- [CCY 3.0](https://html5up.net/license) - inherited from Html5Up
- [Deventy](https://github.com/ianrose/deventy) - the initial starter

<br />

---
[Static Site Eleventy Photon](https://appseed.us/static-site/eleventy-html5up-photon) - provided by **AppSeed**
