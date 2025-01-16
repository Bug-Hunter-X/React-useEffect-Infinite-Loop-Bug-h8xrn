# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook: an infinite loop caused by missing dependencies.  The bug occurs when an effect that modifies state is missing that state variable from its dependency array. 

## Bug Description

The `bug.js` file shows an infinite loop because the `useEffect` hook has a dependency array that is empty (`[]`). This leads to the console logging continuously and the browser may hang.