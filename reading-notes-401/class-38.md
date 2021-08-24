# Read: Class 38 - Redux - Asynchronous Actions

### Review, Research, and Discussion

**1. How granular should your reducers be?**

As granular as you can make them. This improves runtime and makes debugging easier (literally struggling with this today because I didn't do this lol)

**2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched?**

I'd say Pro because you sometimes want to share state changes across multiple reducers

**3. Name a strategy for preventing the above?**

Make sure your reducer names are explicit. The more vague they are the more confusing your code is to read. 

**Term** | **Definition**
-----|-----
store | An immutable object tree. State container which holds the application's state. [tutorialspoint](https://www.tutorialspoint.com/redux/redux_store.htm)
combined reducers | helper function that turns an object whose values are different reducing functions into a single reducing function you can pass to createStore [redux](https://redux.js.org/api/combinereducers)


### Preview
- [async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)
- [thunk middleware](https://github.com/reduxjs/redux-thunk)
- [redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)

1. Which 3 things had you heard about previously and now have better clarity on?

reducers, combined reducers

1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

Thunk middleware and redux thunk, combined reducers

1. What are you most excited about trying to implement or see how it works?

More Redux Practice

