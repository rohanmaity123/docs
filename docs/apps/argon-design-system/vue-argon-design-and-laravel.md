title: Full-Stack Argon Design in Vue and Laravel

# Vue Argon Design with Laravel
Full-Stack App built on top of Argon Design integrated with Laravel

<br />

## Product Description
---
Full-Stack Argon Design is coded in Vue.js and use Laravel server in the backend to become a fully functional app. The [original frontend](https://www.creative-tim.com/product/vue-argon-design-system) designed by **Creative-Tim** is enhanced with [JWT authentication](https://jwt.io/introduction/) and communicates with the [Laravel](https://laravel.com/) backend via Ajax calls.

The product is built on [Two-Tier Architecture](https://www.techopedia.com/definition/467/two-tier-architecture) where the frontend and the backend are decoupled.

<br />

## How to use it
---
In order to use the app, steps to be followed are:

 - Download, build and start the Laravel Backend server
 - Download, build and start the Vue Argon Design 

<br />

### Build the Laravel Backend
---
To build and start the [Laravel server](https://github.com/app-generator/laravel-starter) for this Full-Stack application please, read the [README](https://github.com/app-generator/laravel-starter/blob/master/README.md) file and after, follow the steps:

```
$ git clone git clone https://github.com/app-generator/laravel-starter.git
$ cd laravel-starter

$ composer install # install modules
$ php artisan key:generate # this will trigger Laravel magic 
$ php artisan migrate:fresh --seed # build the database

# to run the app, switch to the public directory
$ cd public
$ php -S localhost:3000 # start the app on port 3000
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

- The [product page](https://appseed.us/apps/vuejs/laravel/argon-design-system-creative-tim)
- [Vue Argon with Laravel Live DEMO](https://laravel-vuejs-argon-design.appseed.us)
- Full-Stack [Vue Argon coded with Express](/apps/argon-design-system/vue-argon-design-and-express) backend
- Full-Stack [Vue Argon coded with Flask](/apps/argon-design-system/vue-argon-design-and-flask) backend
- A comprehensive blog article about [Argon Design](https://blog.appseed.us/argon-design-system/)
- [Full-Stack apps coded with Argon Design](https://appseed.us/apps/argon-design-system) 
- [Github apps](https://github.com/search?q=argon+design+system) coded with Argon Design

