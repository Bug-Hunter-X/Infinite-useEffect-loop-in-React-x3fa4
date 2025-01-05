# React Infinite useEffect Loop Bug

This repository demonstrates a common React bug involving an infinite loop in the `useEffect` hook. The issue arises from improperly specifying the dependencies array in `useEffect`, leading to the effect running continuously and impacting performance.

## Bug Description

The `useEffect` hook is designed to perform side effects after every render. However, if the dependencies array is missing or incorrectly specified, it can lead to an infinite loop.

## Solution

The solution is to accurately specify the dependencies array. In this case, the `count` variable should be included in the dependency array to ensure the effect only runs when `count` changes.

## How to reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`. 
4. Observe the console output. 
5. Observe the browser performance by pressing click me button repeatedly.

## How to fix

1. Modify the code accordingly in bugSolution.js file