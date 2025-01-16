# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of error handling for invalid input.  Specifically, the `/users/:id` route attempts to parse the `id` parameter as an integer without checking for potential errors.  If the `id` parameter is not a valid integer, this could lead to unexpected behavior or crashes.

The `bug.js` file contains the buggy code. The `bugSolution.js` file demonstrates a corrected version with proper error handling.

## Bug
The original code lacks proper error handling for invalid user IDs.  This can result in exceptions if the ID is not an integer or cannot be parsed as such.