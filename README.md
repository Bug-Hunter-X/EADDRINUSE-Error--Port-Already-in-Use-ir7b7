# Node.js EADDRINUSE Error

This repository demonstrates a common error encountered when running Node.js servers: the `EADDRINUSE` error. This occurs when the server attempts to bind to a port that is already in use by another process.

## Bug

The `bug.js` file contains a simple HTTP server that listens on port 8080. If port 8080 is already in use (e.g., by another server or application), the server will fail to start and throw an `EADDRINUSE` error.

## Solution

The `bugSolution.js` file demonstrates how to handle this error gracefully by checking if the port is available before attempting to bind to it.  It uses a try...catch block to catch the error and provides a more informative error message.