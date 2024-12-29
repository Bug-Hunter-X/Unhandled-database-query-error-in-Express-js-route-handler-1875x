# Unhandled Database Query Error in Express.js Route Handler

This repository demonstrates a common error in Express.js applications where a database query failure in a route handler is not properly handled, leading to server crashes or unexpected 500 errors.  The example uses a simplified database interaction, but the principle applies to more complex scenarios.

## Bug Description
The provided `bug.js` file contains an Express.js route handler that fetches user data based on a provided ID. If the database query fails to find a user with the matching ID, the code lacks proper error handling, potentially resulting in an unhandled exception and server failure.  The solution demonstrates proper error handling to prevent this scenario.

## Solution
The `bugSolution.js` file provides a corrected version with appropriate error handling using try...catch blocks to gracefully handle database errors and return appropriate HTTP status codes to the client.