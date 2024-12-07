# React Native Uninitialized State Variable Access

This repository demonstrates a common error in React Native: accessing a state variable before it has been initialized.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

## Problem

Accessing a state variable before the `useState` hook has fully initialized it results in a runtime error, as the state variable is initially `undefined`. This usually happens due to the asynchronous nature of rendering.

## Solution

The solution involves ensuring the state variable is properly initialized before being used. This can be achieved using conditional rendering or by initializing the state with a default value that can be used before the async operation completes.

## How to run

1. Clone the repository
2. `npm install`
3. `npx react-native run-android` (or `npx react-native run-ios`)