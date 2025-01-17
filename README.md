# React Router Dom Catch-All Route Override

This repository demonstrates a common issue in React Router Dom v6 where a catch-all route (`/*`) unintentionally overrides other, more specific routes.  The problem is that `/*` is too broad and matches any path, preventing other routes from being matched.

## Problem

The provided `App.js` demonstrates this problem.  No matter which route you try to navigate to, you will always end up on the `NotFound` page, because the catch-all route will always match.  This is often a difficult-to-debug issue for React developers.