# Next.js Blank Screen After Navigation with Long-Running Task

This repository demonstrates a bug in a Next.js application where navigating to a page with a long-running task (simulated here) can result in a blank screen or a frozen UI.  The issue stems from potential race conditions or improper asynchronous operation handling. The solution involves optimizing the loading state management and providing more robust feedback during the loading process.

## Bug
The `about.js` file contains a `useEffect` hook that simulates a 5-second delay.  During this delay, if the user navigates away from the page, the UI may freeze or display a blank screen.

## Solution
The `aboutSolution.js` file demonstrates a solution which includes adding a loading indicator and managing the loading state more efficiently, preventing the blank screen issue.