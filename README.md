# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook and missing dependency arrays.  The bug causes an infinite loop, leading to application crashes or unexpected behavior.

## The Bug

The `bug.js` file contains a component that uses `useEffect` to increment a counter. However, the `setCount` function is called within the `useEffect` without specifying a dependency array. This causes the effect to run continuously, resulting in an infinite loop. 

## The Solution

The `bugSolution.js` file provides the corrected code. By adding the `count` state variable to the dependency array, the effect only runs when the `count` value changes.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` (or `yarn install`).
4. Run `npm start` (or `yarn start`).
5. Observe the infinite loop (or lack thereof, after the fix).

This example illustrates a crucial aspect of using the `useEffect` hook correctly in React applications.  Always carefully consider the dependency array to prevent unintended consequences.