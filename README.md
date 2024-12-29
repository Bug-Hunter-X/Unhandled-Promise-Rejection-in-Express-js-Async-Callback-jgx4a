# Unhandled Promise Rejection in Express.js Async Callback

This repository demonstrates a common error in Node.js applications using Express.js: unhandled promise rejections.  The bug occurs when an exception is thrown within an asynchronous callback, causing the application to crash without proper error handling.

## Bug Description

The `bug.js` file contains an Express.js server with a route that simulates an asynchronous operation.  Sometimes the operation throws an error, resulting in an unhandled promise rejection.

## Solution

The `bugSolution.js` file shows how to fix this using a `try...catch` block within the asynchronous callback to handle the potential error, preventing the unhandled rejection and providing more graceful error handling.