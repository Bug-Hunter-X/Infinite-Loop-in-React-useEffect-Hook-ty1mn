# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by improper use of the `useEffect` hook.  The `bug.js` file contains the buggy code, while `bugSolution.js` provides the corrected version.

The bug arises from the `useEffect` hook's dependency array.  By including `count` in the dependency array, the effect is triggered whenever `count` changes. The effect then updates `count`, creating an endless loop of updates.

The solution involves strategically managing dependencies to break this cycle.  Learn more by examining the corrected code in `bugSolution.js`.