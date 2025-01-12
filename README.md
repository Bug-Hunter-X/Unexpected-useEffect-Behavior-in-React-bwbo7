# Unexpected useEffect Behavior in React

This repository demonstrates a common issue with the `useEffect` hook in React where it runs after every render, leading to performance problems and unexpected behavior. The solution shows how to use dependency arrays to control when the effect runs.

## Problem

In the `bug.js` file, the `useEffect` hook logs a message to the console after every render, regardless of whether the component's state has changed. This can be inefficient and lead to unexpected side effects.

## Solution

The `bugSolution.js` file shows the correct usage of `useEffect` with a dependency array. The effect now only runs when the `count` state variable changes, improving performance and preventing unnecessary re-renders.