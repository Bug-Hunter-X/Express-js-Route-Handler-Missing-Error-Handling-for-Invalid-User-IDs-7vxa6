# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers:  failure to handle invalid input, specifically non-numeric user IDs in this case.  The provided `bug.js` file showcases the problematic code, while `bugSolution.js` offers a corrected version with robust error handling.

## Problem

The original code attempts to find a user based on a provided ID. However, it lacks error handling for scenarios where the `userId` parameter is not a valid integer. This can lead to exceptions, unexpected behavior, or application crashes.

## Solution

The corrected code in `bugSolution.js` includes explicit checks to ensure the `userId` is a number before attempting to parse and use it.  If it's not a number, an appropriate error response is returned to the client.