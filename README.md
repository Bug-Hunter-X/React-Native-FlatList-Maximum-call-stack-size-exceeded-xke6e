# React Native FlatList Maximum Call Stack Size Exceeded

This repository demonstrates a common error in React Native when using `FlatList` with large datasets: the "Maximum call stack size exceeded" error.  The provided solution optimizes rendering for improved performance.

## Bug
The bug occurs because `FlatList` attempts to render all items simultaneously, exceeding the call stack limit.  The `FlatListBug.js` file shows this problematic implementation.

## Solution
The solution, demonstrated in `FlatListSolution.js`, involves using techniques such as `keyExtractor`, `getItemLayout`, and potentially `windowSize` to optimize rendering and improve performance. These techniques enhance the way FlatList manages the rendering process and avoid exceeding the call stack limit.

## Reproduction
1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app on an emulator or device.
4. Observe the error with the initial implementation (FlatListBug.js).
5. Observe the improved performance and lack of errors with the solution (FlatListSolution.js).