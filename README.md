# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js servers: unresponsiveness due to long-running operations blocking the event loop.  The `server.js` file contains a simple HTTP server that simulates a long-running task, causing the server to hang.

The solution, provided in `serverSolution.js`, utilizes asynchronous operations (using `setTimeout` as an example; typically worker threads or other non-blocking methods should be employed) to prevent the event loop from being blocked.