# React useEffect Runs on Every Render

This repository demonstrates a common issue in React where the `useEffect` hook runs on every render, even when a dependency array is provided. This can lead to performance problems and unexpected side effects.

The `bug.js` file contains the problematic code. The `bugSolution.js` file shows how to fix this issue. 

## Problem
The `useEffect` hook in `bug.js` is intended to log the current count only when the count changes. However, due to a missing or incorrect dependency array, it runs on every render.