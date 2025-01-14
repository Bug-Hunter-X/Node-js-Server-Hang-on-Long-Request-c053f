# Node.js Server Hang on Long Request

This repository demonstrates a common issue in Node.js where a server can hang if it's processing a request that takes a long time to complete.  This is because Node.js uses a single-threaded event loop, and a long-running operation blocks the event loop from processing other requests.

The `server.js` file shows the buggy code which contains a long-running synchronous operation that blocks the event loop.  The `serverSolution.js` demonstrates how to fix it using asynchronous operations and proper event loop handling.