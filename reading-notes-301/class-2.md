# Lifecycle of Components

### Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.

### The three phases are: Mounting, Updating, and Unmounting.

![V2](https://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/ogimage.png)
# Mounting
### Mounting means putting elements into the DOM.

### React has four built-in methods that gets called, in this order, when mounting a component:

### constructor()
### getDerivedStateFromProps()
### render()
### componentDidMount()
### The render() method is required and will always be called, the others are optional and will be called if you define them.

# constructor

### The constructor() method is called before anything else, when the component is initiated, and it is the natural place to set up the initial state and other initial values.

### The constructor() method is called with the props, as arguments, and you should always start by calling the super(props) before anything else, this will initiate the parent's constructor method and allows the component to inherit methods from its parent (React.Component).

# getDerivedStateFromProps
### The getDerivedStateFromProps() method is called right before rendering the element(s) in the DOM.

### This is the natural place to set the state object based on the initial props.

### It takes state as an argument, and returns an object with changes to the state.

### The example below starts with the favorite color being "red", but the getDerivedStateFromProps() method updates the favorite color based on the favcol attribute:

