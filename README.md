# React Router Wildcard Route Issue

This repository demonstrates a common issue in React Router v6 where a wildcard route (`*`) unexpectedly matches all paths, preventing other routes from functioning correctly.

## Problem
The `App.js` file shows how a wildcard route, intended to handle 404 errors, unintentionally captures all navigation, even if a more specific route exists.  This is because wildcard routes are always matched last, if not carefully placed.

## Solution
The `AppSolution.js` file presents the corrected code. The wildcard route is placed at the end, ensuring that it only matches if no other route is found.