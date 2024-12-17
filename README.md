# React useEffect setInterval Memory Leak
This repository demonstrates a common React bug involving the `setInterval` function inside a `useEffect` hook without proper cleanup.  The bug leads to a memory leak because the interval continues running indefinitely even after the component unmounts.

The `bug.js` file shows the problematic code.  The `bugSolution.js` file provides the corrected code, including a cleanup function to stop the interval when the component unmounts.