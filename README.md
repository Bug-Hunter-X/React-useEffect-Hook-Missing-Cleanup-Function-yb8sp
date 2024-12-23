# React useEffect Hook Missing Cleanup

This repository demonstrates a common error in React applications involving the `useEffect` hook:  the absence of a cleanup function.  The example shows how forgetting to return a cleanup function can lead to memory leaks or unexpected side effects.

## The Problem

The provided `bug.js` file showcases a `MyComponent` that uses `useEffect` to log a message when the component mounts. However, it's missing a crucial aspect: the return statement that defines the cleanup function.  Without a cleanup function, actions performed within the `useEffect` callback persist even after the component unmounts, potentially leading to memory leaks and unexpected behavior.

## The Solution

`bugSolution.js` provides the corrected code, demonstrating the importance of the cleanup function. By returning a function within the `useEffect` callback, we ensure that necessary cleanup is performed when the component unmounts. This prevents potential issues and keeps your application running smoothly.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the application. 
