# Unhandled Error in Asynchronous Express.js Route Handler

This repository demonstrates a common error in Node.js applications using Express.js: an unhandled error within an asynchronous route handler. The error occurs because an exception is thrown inside a `setTimeout` callback, leading to a process crash without appropriate error handling or logging.

The `bug.js` file contains the flawed code. The `bugSolution.js` file provides a corrected version that demonstrates proper error handling.

## How to Reproduce

1. Clone this repository.
2. Run `npm install express` to install the required dependency.
3. Run `node bug.js` to see the unhandled error and application crash.
4. Run `node bugSolution.js` to observe the improved error handling and a graceful response.