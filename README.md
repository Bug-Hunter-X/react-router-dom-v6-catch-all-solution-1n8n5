# React Router DOM v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`*`) in React Router DOM v6.  The catch-all route, intended to handle any unmatched paths, may not function correctly due to route definition order or path specificity conflicts.

## Problem
The `App.js` file contains a basic React Router setup with a catch-all route for handling 404 errors. However, this catch-all route may not be triggered as expected, especially if the URL doesn't match any other defined routes.

## Solution
The solution involves careful route ordering and path specificity.  The catch-all route (`*`) should always be placed as the last route in the `Routes` component to ensure it's only used for paths not matched by other routes. 