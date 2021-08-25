## Read: Class 39 - Redux - Additional Topics

### Review, Research, and Discussion

**1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?**

Best practice is to fire an asynchronous function so you can get your data before the page renders. You would bring in something like useEffect which will fire a fetch function on page load

**2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?** 

You export your action creator 

**Term** | **Definition**
-----|-----
middleware | Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware. (Red Hat)[https://www.redhat.com/en/topics/middleware/what-is-middleware]
thunk | a dull, heavy sound, such as that made by an object falling to the ground...just kidding it's the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests. [EvanHahn](https://github.com/reduxjs/redux-thunk)


### Preview
- [Redux Toolkit (RTK)](https://redux-toolkit.js.org/)
- [Tutorial](https://redux-toolkit.js.org/tutorials/overview)
- [MobX](https://mobx.js.org/getting-started.html)
- [HookState](https://hookstate.js.org/)


1. Which 3 things had you heard about previously and now have better clarity on?

Thunk, middleware, dispatches/actions

1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

I still need more practice with redux, it is starting to click though after yesterdays lab. 

1. What are you most excited about trying to implement or see how it works?

redux

