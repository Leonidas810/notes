---
tags:
  - Express
---

# Overview
Middleware functions are functions that have access to the *requestObjects(req)*, the *response object(res)*, and the *"next"* function in the application's request-response cycle. The *"next"* function is a functions in the [[Express]] router which, when invoked, executes the middleware succeeding the current middleware.

Middleware functions can perform the following tasks:
- Execute any code
- Make changes to the request and the response objects.
- End the request-response cycle
- Call the next middleware in the stack

If the current middleware function does not end the request-response cycle, it must call *"next()"* to pass control to the next middleware function. Otherwise, the request will be left hanging.

The following figure shows the elements of a middleware function call:

![[Express_middleware.png]]
Starting with Express 5, middleware functions that return a promise will call *"next(value)"* when they reject or throw an error. next will be called with either the reject value or the thrown Error.