# React Router Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other routes if not placed correctly within the `<Routes>` component.

The problem arises when the catch-all route is placed before other more specific routes.  This causes the catch-all route to match all paths, overriding other routes that should be rendered for specific paths. The solution is simple: place the catch-all route as the last route defined within the `<Routes>` component.