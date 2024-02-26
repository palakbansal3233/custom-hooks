# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

Initialise State:

- Create a state to hold the throttled value using useState()

Track last execution time:

- useRef to keep a track of the last time the function was executed

UseEffect for throttling:

- Setup a timer (using setTimeout) to handle the logic
- Inside Timer:
- Check time elapsed since the last execution
- If the elapsed time is greater than or equal to the specified delay, update the throttled value and the last execution time
- Calculate the remaining time for next execution ( if any)
- Return a cleaup function to clear the timer
- return the throttled value from the hook
