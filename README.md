# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug causes an infinite rendering loop, leading to performance issues or crashes.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders. However, if the dependencies array is omitted or incorrectly defined, the effect will run on every render, potentially creating an infinite loop.

## How to Reproduce
Clone this repository and run `npm install` to install the necessary dependencies. Then, run `npm start` to start the development server. You will observe the console logging the count value repeatedly, and the browser tab may freeze.

## Solution
The solution involves correctly specifying the dependencies array for `useEffect`. The dependencies array ensures that the effect only runs when one of the listed values changes. This prevents the infinite loop.

## Lessons Learned
Always specify the dependency array in your `useEffect` hooks. This helps you avoid unexpected behavior and performance issues.
