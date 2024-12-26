# React Router v6 Catch-all Route Issue

This repository demonstrates a subtle bug in React Router v6 related to the catch-all route (`/*`) when used in conjunction with nested routes. The catch-all route unexpectedly intercepts routes that should be handled by nested route components.

## Problem Description

The issue occurs when a catch-all route (`/*`) is defined alongside nested routes.  The catch-all route incorrectly captures all navigation attempts, including those meant for the nested routes.

## Solution

The solution involves re-ordering the routes. By placing the catch-all route at the very end, after all other routes, React Router will correctly match the more specific routes first.
