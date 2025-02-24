# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common error in React 19 involving the `useEffect` hook.  Incorrectly specifying dependencies can lead to infinite render loops. This example showcases the problem and its solution.

## Bug
The `bug.js` file contains a component with an `useEffect` hook that's missing a key dependency, causing an infinite loop.  The console will show repeated render messages.

## Solution
The `bugSolution.js` file corrects the issue by adding the `count` state variable to the dependency array of the `useEffect` hook.  This ensures the effect only runs when the `count` changes, preventing the infinite loop.