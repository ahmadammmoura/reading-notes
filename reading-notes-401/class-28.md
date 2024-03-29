# Component Lifecycle / useEffect() Hook


## Review, Research, and Discussion

1. Why do we *not* need more .html pages in a multi-page React app?
    1. Instead of rendering multiple pages, a single page app re-renders the contents of a single page dynamically. The client gets all the pages contents, and moving to other 'routes' tells the page which resources to use.

1. If we wanted a component to show up on every page, where should we put it
    1. To render a component on every page put it inside of `<Router>` but not behind a `<Route>`.

1. What does routing do with the components that were rendered when a new route is requested
    1. The previous components unmount, and the new ones mount to the page... idk how that works though.

1. What does props.children contain
    1. It's the head between the ears, the text in between the tags. The text or components that are inside of the component itself is attached to props.children [(source)](https://reactjs.org/docs/glossary.html#propschildren).

    ```JS
    <Hello>Children live here</Hello>
    ```

1. How do `useState()` and `this.useState()` differ?
    1. useState() is a react hook that produces a stateful value and a setter function.
    1. this.state refers to the state that was constructed when a class component was instantiated

## Vocabulary Terms

1. State Hook
    1. The state hook is one of the basic hooks that come with React out of the box. It lets us create stateful functional components.

1. Mounting and Un-Mounting
    1. Mounting is the process of adding nodes to the DOM, and un-Mounting is the process of removing them.

## Further Reading

[Effect Hook – React docs](https://reactjs.org/docs/hooks-effect.html)

[React Router – docs](https://reactrouter.com/web/example/basic)