# useState Hook

![image](https://lh3.googleusercontent.com/proxy/T8gjXHKu2Fxj6YswUCaEpOYpZWJJ8Auf4srmsdeuLbPi9vJGEHCUmzYpjpKat0TyumY26KYoyG7qSSweCsR72DJWT0c54Fnl4DmstQvnRuLOe0dlRYJpSWA)

###### Normal react code would use a class component and use this.setState to manage the state.

###### Hooks is a way to write functional components but use state inside of them like you would a class component.

##### First, import the hook you want to use from React.

###### useState gives us back two parameters inside of an array. Use array destructuring to declare, in this order, state value, and the function that will modify that state value. You can name these two items whatever you want (you’re just declaring variables here), so make the names explicit. E.g., if you wanted to set the name to the logged in user, a simple example would be like the below, where the name is being modified by the function setName, and useEffect is setting it to ‘Mikkel’ (as the inital state).


## Review, Research, and Discussion

1. How does React differ from vanilla JS/HTML/CSS?
    1. The primary difference between React and vanilla scripts is that it sets rules about its implementation. While React isn't as freeform as the others, it's still pretty versatile.

1. What is the primary difference between class components and functional components?
    1. Functional components are functions rather than instance of the React.component class, as such their syntax and form is entirely different. Most if not all functionality is identical across the two designs.

## Vocabulary Terms

1. Functional components
    1. These are React components written as functions rather than classes.
    1. They have a host of hooks available to them to enable React functionality

1. Children / Child components
    1. Children components are contained within a parent component




### Preview and Preparation

[Making Sense of React hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

* Functional components improve performance
* Class components lead to spaghetti code at a certain point
* Functions are easier to read
* Prevent unnecessary nesting (more classes to solve class problems)

