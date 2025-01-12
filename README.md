# Unexpected Re-renders in React useEffect Hook

This example demonstrates a common issue in React applications involving the `useEffect` hook.  Incorrect dependency management within `useEffect` can lead to unexpected behavior, such as infinite loops or unintended re-renders.

The `bug.js` file contains a component with an `useEffect` hook that has an incomplete dependency array.  This causes the effect to run after every render, potentially leading to performance problems or infinite loops.

The `bugSolution.js` file shows the corrected version with the correct dependency array, ensuring the effect only runs when the count changes.