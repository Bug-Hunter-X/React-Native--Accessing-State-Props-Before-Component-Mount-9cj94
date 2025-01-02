# React Native: Accessing State/Props Before Component Mount

This repository demonstrates a common error in React Native: attempting to access component state or props before the component has fully mounted.  This often manifests with unexpected behavior or errors, especially when dealing with asynchronous operations.

## The Problem

The `bug.js` file showcases a component that fetches data after mounting.  It attempts to access and display the fetched data before it has been fully set in the component's state, leading to undefined behavior.

## The Solution

The `bugSolution.js` file provides a corrected version. It utilizes the `useEffect` hook (for functional components) to fetch the data and update the state only after the component has successfully mounted.  Conditional rendering is also implemented to prevent display errors until the data is available.

## How to Run

1. Clone this repository.
2. Navigate to the project directory: `cd react-native-mount-error`
3. Run the project in a React Native environment (e.g., using Expo CLI).