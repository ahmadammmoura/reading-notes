## Read: Class 37 - Redux - Combined Reducers

### Review, Research, and Discussion

**1. Why choose Redux instead of the Context API for global state?**

Context API prompts a re-render on each update of the state and re-renders all components regardless. Redux however, only re-renders the updated components. [codehouse group](https://www.codehousegroup.com/insight-and-inspiration/tech-stream/using-redux-and-context-api)

**2. What is the purpose of a reducer?**

Evaluates an action and creates a new state object given the evaluated action

**3. What does an action contain?**

payload, type, and switch cases

**4. Why do we need to copy the state in a reducer?**

So the application doesn't lose the current state

**Term** | **Definition**
-----|-----
immutable state | State that cannot be modified
time travel in redux | The ability to look back at previous states to see what the state was at that moment in time
action creator | A function that returns an action object
reducer | A pure function that takes an action and the previous state of the application and returns the new state [PluralSight](https://www.pluralsight.com/guides/how-to-write-redux-reducer)
dispatch | Tells the app the state has been updated

### Preview
- [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)
- [Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)
- [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

1. Which 3 things had you heard about previously and now have better clarity on?

payload, actions, context API

1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

time traveling with redux, overall better understanding of reducers

1. What are you most excited about trying to implement or see how it works?

Excited to get more comfortable with the flow of redux
