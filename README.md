# React Native Dimensions API: Handling undefined/null initial dimensions

This repository demonstrates a common issue encountered when using the `Dimensions` API in React Native: the initial dimensions being `undefined` or `null`. This can cause crashes or unexpected behavior if your components attempt to use these values before they are available.

The solution involves using the `useEffect` hook to asynchronously retrieve the dimensions and update component state accordingly. This ensures that the dimensions are always defined before being used.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install` to install dependencies.
3. Run the app using a React Native simulator or device.
4. Observe the initial render and subsequent updates to the screen dimensions.

## Solution

The `DimensionsBugSolution.js` file provides a working example of how to handle the asynchronous nature of the `Dimensions` API using the `useEffect` hook.  This ensures that components render correctly even before the dimensions are completely loaded.