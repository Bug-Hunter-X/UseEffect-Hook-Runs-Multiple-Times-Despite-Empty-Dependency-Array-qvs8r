# React useEffect Hook Runs Multiple Times Despite Empty Dependency Array

This repository demonstrates a common issue with the React `useEffect` hook where the effect runs multiple times despite specifying an empty dependency array.  The code in `bug.js` showcases the problem.  `bugSolution.js` provides a corrected version.

The problem arises from a misunderstanding of how React's reconciliation process interacts with effects.  Sometimes, even with an empty dependency array, updates or re-renders in other parts of the component tree can trigger the effect unnecessarily.

This example highlights the importance of correctly managing dependencies in `useEffect` to avoid unexpected behavior and performance issues.