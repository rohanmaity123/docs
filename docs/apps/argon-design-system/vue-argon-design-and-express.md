title: Full-Stack Argon Design in Vue and Express

# Vue Argon Design with Express
Full-Stack App built on top of Argon Design integrated with Express

<br />

## Product Description
---
Full-Stack Argon Design is coded in Vue.js and use Express server in the backend to become a fully functional app. The [original frontend](https://www.creative-tim.com/product/vue-argon-design-system) designed by **Creative-Tim** is enhanced with [JWT authentication](https://jwt.io/introduction/) and communicates with the [Express](https://expressjs.com/) backend via Ajax calls.

The product is built on [Two-Tier Architecture](https://www.techopedia.com/definition/467/two-tier-architecture) where the frontend and the backend are decoupled.

<br />

## How to use it
---
In order to use the app, steps to be followed are:

 - Download, build and start the Express Backend server
 - Download, build and start the Vue Argon Design 

<br />

### Build the Express Backend
---
To build and start the [Express server](https://github.com/app-generator/express-starter) for this Full-Stack application please, read the [README](https://github.com/app-generator/express-starter/blob/master/README.md) file and after, follow the steps:

```
$ git clone https://github.com/app-generator/express-starter.git
cd express-starter

yarn # install dependencies
yarn start # start the app 
```

By default, the backend server starts on **port 3000**, and will expose two methods:

 - api/users/login  - `POST` handler responsible with user authentication 
 - api/users/signup  - `POST`  handler responsible with user registration

<br />

### Build the Vue Argon Frontend
---
Steps to follow to build and use the Vue version of [Argon Design](https://github.com/app-generator/vuejs-argon-design-system) (before the manual build, please read the [README](https://github.com/app-generator/vuejs-argon-design-system/blob/master/README.md) file, first)

```
$ git clone https://github.com/app-generator/vuejs-argon-design-system.git
cd argon-design-system

yarn # install dependencies
yarn start # start the app 
```

By default the app starts on port 8080. If all goes well, you may visit the application on `http://localhost:8080`. 

<br />

## Support
---
For support please access the official [support](https://appseed.us/support) page or contact us directly on [Discord](https://discord.gg/fZC6hup).

<br />

## Related resources
---

- The [product page](https://appseed.us/apps/vuejs/express/argon-design-system-creative-tim)
- [Vue Argon with Express Live DEMO](https://express-vuejs-argon-design.appseed.us/#/)
- Full-Stack [Vue Argon coded with Flask](/apps/argon-design-system/vue-argon-design-and-flask) backend
- Full-Stack [Vue Argon coded with Laravel](/apps/argon-design-system/vue-argon-design-and-laravel) backend
- A comprehensive blog article about [Argon Design](https://blog.appseed.us/argon-design-system/)
- [Full-Stack apps coded with Argon Design](https://appseed.us/apps/argon-design-system) 
- [Github apps](https://github.com/search?q=argon+design+system) coded with Argon Design

