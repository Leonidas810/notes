---
tags:
  - Express
---
Express is a lightweight web application framework, and is one of the most popular packages on [[NPM]]. Express makes it much easier to create a server and handle routing for your [[Node.js]] application, which handles things like directing people to the correct page when they visit a certain endpoint.

# 5.x API
[Express 5.0](https://expressjs.com/en/5x/api.html#express.json) requires [[Node.js]] **18** or higher

## express()
Creates and Express application.  The *"express()"* function is a top-level function by the express module.

```
const express = require('express')
const app = express()
```

### Methods

#### express.json("[options]")
This is a built-in middleware function in Express, It parse incoming requets with JSON payloads and is based on body-parser

Returns middleware that only parses JSON and only looks at the request where the *"Content-Type"*  header matches the type option. This parser accepts any Unicode encoding of the body and supports automatic inflation of gzip and deflate encoding

A new body object containing the parsed data is populated on the request object after the middleware (i.e req.body), or undefined if there was no body to parse, the *"Content-Type"* was no matched, or an error ocurred

### express.static(root,[options])

This is a built-in middleware function in Express. It serves static files and is based on server-static.

The root argument specifies the root directory from which to serve static assets. The function determines the file to serve by combining *"req.url"* with the provided root directory. When a file is not found, instead of sending a 404 response, it instead calls *"next()"* to move on the next middleware, allowing for stacking and fall-backs
## Application

The app Object convetionally denotes the Express application. Create it by calling the top-level *"express()"* function exported by the Express module:

```
const express = require('express')
const app = express()

app.get('/',(req,res)=>{
	res.send('hello world')
})

app.listen(3000)
```

The app object has methods for
- Routing HTTP requests
- Configuring middleware
- Rendering HTML views
- Registering a templates engine
