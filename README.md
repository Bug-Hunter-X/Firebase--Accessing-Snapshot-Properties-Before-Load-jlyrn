# Firebase Snapshot Property Access Before Load

This repository demonstrates a common error when working with Firebase and asynchronous operations: attempting to access properties of a document snapshot before the snapshot has fully loaded.  This leads to undefined values or errors.

## Bug Description

The bug occurs when asynchronous operations, such as fetching data from Firebase, aren't properly awaited.  Accessing snapshot properties before the promise resolves results in an error or undefined values.

## Solution

The solution involves ensuring that all asynchronous operations are properly handled using async/await or `.then()` to wait for the promise to resolve before accessing snapshot properties.

## Setup

1.  Clone this repository.
2.  Install Firebase:
   ```bash
   npm install firebase
   ```
3.  Configure your Firebase project and replace placeholders in `bug.js` and `bugSolution.js` with your project's configuration.
4.  Run the code samples.

