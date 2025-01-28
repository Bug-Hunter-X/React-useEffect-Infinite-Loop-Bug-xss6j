# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by modifying the state variable within the dependency array. The `bug.js` file contains the buggy code, while `bugSolution.js` provides a corrected version.

## Bug Description
The `useEffect` hook attempts to reset the `count` state to 0 when it exceeds 5. However, this action triggers a re-render, causing the `useEffect` hook to run again, leading to an infinite loop.

## Solution
The corrected version prevents the infinite loop by using functional updates and carefully managing state changes.