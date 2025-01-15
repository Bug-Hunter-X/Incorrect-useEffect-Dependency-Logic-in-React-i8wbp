# Incorrect useEffect Dependency Logic in React

This example demonstrates a common error in React's `useEffect` hook: incorrect dependency array logic. The original code has a condition (`if (count)`) inside the useEffect that is always true whenever `count` is greater than 0.  This leads to the log message printing more frequently than intended.

The solution demonstrates how to correctly utilize the dependency array to manage side effects and avoid this common pitfall.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm start` to start the development server.
4. Observe the console output as you click the "Increment" button. The console will print many times due to the incorrect `useEffect` dependency logic.