# React Native useEffect Cleanup Function Error

This repository demonstrates a common error in React Native applications involving the `useEffect` hook's cleanup function.  The error occurs when the cleanup function attempts to access or modify the component's state after the component has been unmounted, leading to a warning about potential memory leaks. 

The `bug.js` file contains the problematic code, while `bugSolution.js` provides a corrected version.

## Problem

The `useEffect` hook's cleanup function in `bug.js` attempts to access the `count` state variable after the component is unmounted.  React prevents this, throwing a warning to alert the developer to the potential memory leak and a no-op.