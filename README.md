# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6. The catch-all route seems to always be triggered, even when other routes should match.

## Problem

The provided `App.js` shows a simple React Router setup.  The expectation is that the `/` and `/about` routes should work correctly. The `/*` route is intended to handle 404s (Not Found). However, it consistently intercepts all requests, regardless of the path.

## Solution

The solution, `AppSolution.js`, demonstrates how to resolve this issue by placing the catch-all route as the last route.  This ensures that other routes are checked first before the catch-all route is considered. 

## Setup

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `npm install` to install the required dependencies.
4. Run `npm start` to start the development server.