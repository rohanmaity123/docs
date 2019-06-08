title: Full-Stack Argon Design in Vue and Flask

# Vue Argon Design with Flask
Full-Stack App built on top of Argon Design integrated with Flask

<br />

## Product Description
---
Full-Stack Argon Design is coded in Vue.js and use Flask server in the backend to become a fully functional app. The [original frontend](https://www.creative-tim.com/product/vue-argon-design-system) designed by **Creative-Tim** is enhanced with [JWT authentication](https://jwt.io/introduction/) and communicates with the [Flask](http://flask.pocoo.org/) backend via Ajax calls.

The product is built on [Two-Tier Architecture](https://www.techopedia.com/definition/467/two-tier-architecture) where the frontend and the backend are decoupled.

<br />

## How to use it
---
In order to use the app, steps to be followed are:

 - Download, build and start the Flask Backend server
 - Download, build and start the Vue Argon Design 

<br />

### Build the Flask Backend
---
To build and start the [Flask server](https://github.com/app-generator/flask-starter) for this Full-Stack application please, read the [README](https://github.com/app-generator/flask-starter/blob/master/README.md) file and after, follow the steps:

```
$ git clone https://github.com/app-generator/flask-starter.git
cd flask-starter

pip install -r requirements.txt
flask run --port 3000
```

The backend server will start on **port 3000**, and expose two methods:

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

- The [product page](https://appseed.us/apps/flask-apps/argon-design-system-creative-tim)
- [Vue Argon with Flask Live DEMO](https://flask-vuejs-argon-design.appseed.us)
- Full-Stack [Vue Argon coded with Express](/apps/argon-design-system/vue-argon-design-and-express) backend
- Full-Stack [Vue Argon coded with Laravel](/apps/argon-design-system/vue-argon-design-and-laravel) backend
- A comprehensive blog article about [Argon Design](https://blog.appseed.us/argon-design-system/)
- [Full-Stack apps coded with Argon Design](https://appseed.us/apps/argon-design-system) 
- [Github apps](https://github.com/search?q=argon+design+system) coded with Argon Design

