# **Express Lunch.ly Reservation System**

## **Overview**

Lunchly is an Express app that is not an API server, nor is it RESTful.
Instead, it’s a server-side templated application with custom URLs.

## **Requirements**

- app.js
  - Our application object; can be imported from other files/tests
- models/
  - Model objects as as classes, to “abstract away” database handling
- routes.js
  - Routes for the web interface
- server.js
  - Functionality to start the server (this is the file that is run to start it)
- templates/
  - Jinja templates, rendered with the JS “Nunjucks” library
- seed.py
  - File to create sample data

## **Technologies Used:**

- [Node.js](https://nodejs.org/en/)
- [PostgreSQL](https://node-postgres.com)
- [Express](https://expressjs.com/en/4x/api.html)
- [Nunjucks](https://mozilla.github.io/nunjucks/)
- [Body Parser](https://www.npmjs.com/package/body-parser)
- [VSCode](https://code.visualstudio.com/docs)

## **How to Run**
This is the Express backend for Lunchly.
To run this:

```bash
# Clone Repository
$ git clone https://github.com/cng008/35.5_express-lunchly.git
$ npm install
$ createdb lunchly
$ psql < data.sql
$ node server.js
open http://localhost:3000/ in API viewer such as Insomnia or Postman
```

Tests are run using Jest and Supertest. Make sure Jest is installed globally.
To run the tests:

    jest -i
