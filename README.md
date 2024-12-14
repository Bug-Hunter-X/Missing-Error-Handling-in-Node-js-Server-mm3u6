# Missing Error Handling in Node.js Server

This repository demonstrates a common error in Node.js server development: missing error handling.  The example shows a basic HTTP server that lacks proper error handling for potential issues during server creation and port listening.  The solution demonstrates how to add comprehensive error handling to prevent unexpected crashes and provide informative error messages.

## Bug

The `server.js` file contains a simple HTTP server without any error handling. If there's an issue (e.g., port already in use), the server will crash without providing useful debugging information.

## Solution

The `serverSolution.js` file shows how to properly handle potential errors using `server.on('error', ...)` event listeners.  This allows the server to gracefully handle errors and log them for debugging.