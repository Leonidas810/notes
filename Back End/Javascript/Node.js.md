
[Node.js official web ](https://nodejs.org/en/learn/getting-started/introduction-to-nodejs)
Node.js is an open-source and cross-platform JavaScript runtime environment. It is popular too for almost any kind of project!.

Node.js runs the V8 JavaScript engine, the core of Google Chrome, outside of the browser. This allows Node.js to be very performant.

A Node.js app runs in a single process, without creating a new thread for every request. Node.js provides a set of asynchronous I/O primitives in its standard library that prevent JavaScript code from blocking. In addition, libraries in Node.js are generally written using non-blocking paradigm. Accordingly, blocking behavior is the exception rather that the norm in Node.js

When Node.js performs an I/O operation, like reading from the network, accessing a database or the filesystem, instead of blocking the thread and wasting CPU cycles waiting, Node.js will resume the operations when the response come back.

This allows Node.js to handle thousands of concurrent connections with a single server without introducing the burden of managing thread concurreny, which could be a significant source of bugs.