# Unhandled Exception Crashing Node.js Server

This repository demonstrates a common error in Node.js applications: unhandled exceptions crashing the server.  The `bug.js` file shows a server that crashes when a specific URL is requested due to an uncaught `Error`. The `bugSolution.js` file provides a solution by incorporating a `try...catch` block to gracefully handle the exception and prevent the server from crashing.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `node bug.js`.
4. Access `http://localhost:3000/error` in your browser.  Observe the server crashing.
5. Run `node bugSolution.js`. Access the same URL. Observe that the server does not crash and provides an error message.

## Solution

The solution involves using a `try...catch` block to handle potential errors. This allows for more robust error handling, logging, and prevents the server from unexpectedly terminating.  Always handle potential errors to build resilient and stable applications.