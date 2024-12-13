# Node.js Express Server Timeout

This repository demonstrates a common issue in Node.js Express servers where a delayed response leads to timeout errors.  The server includes a `setTimeout` function that delays the response for 5 seconds, simulating a long-running task.

## Bug

The `bug.js` file contains the code for an Express server that delays its response.  This delay can cause clients to timeout before receiving the response.

## Solution

The `bugSolution.js` file offers a solution to this problem by ensuring the response is sent immediately.  This can be done by removing the `setTimeout` or by using techniques to manage long-running tasks asynchronously. 

## How to Reproduce the Bug

1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Send a request to `http://localhost:3000`. Observe the delay of 5 seconds before receiving the response.

## How to Solve the Bug

1. Replace the `bug.js` file with the `bugSolution.js` file.
2. Run `node bugSolution.js`. Observe the immediate response. 