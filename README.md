# React Router v6 Nested Routes Re-rendering Issue

This repository demonstrates a common issue encountered when working with nested routes in React Router v6.  The parent component re-renders unnecessarily when navigating to a child route, potentially leading to performance problems or unexpected state changes.

The `bug.js` file shows the problematic code.  The `bugSolution.js` file provides a solution to mitigate this issue.

## Problem

The issue stems from the way React Router v6 handles route changes.  In the original example, navigating to a child route causes the parent component to remount, leading to unnecessary re-renders and potential state loss.

## Solution

The solution involves using techniques to prevent unnecessary re-renders of the parent component.   This might involve memoization, use of `useMemo` hook,  or changes to the state management strategy to make the parent component state more resilient to child route changes.