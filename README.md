# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js where an unexpected exception in an HTTP server isn't handled gracefully, causing the server to crash.

## The Bug

The `bug.js` file contains a simple HTTP server. However, if you request the `/error` route, it throws an uncaught `Error`, causing the server to terminate abruptly.

## The Solution

The `bugSolution.js` file provides a solution by using a `try...catch` block to handle the potential error within the request handler.  This prevents the server from crashing and allows for more robust error logging and handling.