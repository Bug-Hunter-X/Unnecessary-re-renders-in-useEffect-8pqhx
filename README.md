# Unnecessary Re-renders in React useEffect

This example demonstrates an issue where a React `useEffect` hook runs after every render, even when there's no actual change in state or props. This leads to unnecessary re-renders and potentially performance issues.

The `useEffect` hook with no dependency array (`[]`) runs after every render, resulting in the console log being printed multiple times.

The solution demonstrates how to use a dependency array to specify when the effect should run.