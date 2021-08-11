# Advanced State With Reducers

### How can we ensure that an effect hook runs only once?

To ensure that useEffect() hook is run only once, you can add a second parameter is square brackets and pass in props, state, or nothing. 

example: 

          import React, { useEffect } from 'react';

    function App() {
      useEffect(() => {
        // Run! Like go get some data from an API.
      }, []); <----------- the square brackets here ----------

### Can useState() update more than one state variable at the same time?
yes, because each set state will be different and will not collide with each other.

### Is useState() synchronous?
State is asynchronous. 

### term
### State Hook
State Hook is used to change React state in functional components. 
### Component Lifecycle
Components will be created or mounted onto the DOM, then updated, and then unmount from the DOM. 

Initialization ---> Mounting ---> Update ---> Unmount