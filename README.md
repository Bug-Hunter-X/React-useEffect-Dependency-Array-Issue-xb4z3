# React useEffect Dependency Array Issue

This repository demonstrates a common error in React's `useEffect` hook: forgetting to include dependencies in the dependency array. This leads to unnecessary re-renders and potential performance problems.

## Bug
The `bug.js` file shows a `MyComponent` that uses `useEffect` without correctly specifying the dependency array. This results in the effect running after every render, even when the count doesn't change, logging the message unnecessarily.

## Solution
The `bugSolution.js` file demonstrates the corrected version. By adding `count` to the dependency array, the effect only runs when the value of `count` changes.