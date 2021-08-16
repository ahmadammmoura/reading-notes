
## Review, Research, and Discussion

##### What are some good use cases for using the Context API for global state?

##### Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

##### How can you best test context?


##### It recommends testers to choose their testing techniques, test deliverables, test documentation and test objectives by looking into the details of a specific situation.



### Term

* context => React Context is a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree.


* useContext() => The useContext accepts the value provided by React. createContext and then re-render the component whenever its value changes but you can still optimize its performance by using memorization.


* static context => A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object. ... But static contexts(methods and blocks) doesn't have any instance they belong to the class.


#### Preparation Materials

[context-api](https://reactjs.org/docs/context.html)
[hooks-and-context-example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
[react-context-links](https://github.com/diegohaz/awesome-react-context)