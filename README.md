# React useEffect Hook Bug

This repository demonstrates a common bug related to the `useEffect` hook in React. The bug involves an incorrectly specified dependency array, leading to unexpected behavior and potential performance issues.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders. However, if the dependency array is not correctly specified, it can run more or less often than intended, resulting in unexpected results or performance problems. This example showcases a scenario where the dependency array is missing a needed state variable.

## Bug Reproduction
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs and the behavior of the counter.

## Bug Solution
The solution involves reviewing the dependencies of the `useEffect` call and correctly updating the dependency array to ensure the effect only runs when the state value changes.   This involves correctly updating the dependencies array in the useEffect call to include all values from the component state that the effect depends on.