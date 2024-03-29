# Lifting State Up

### Often, several components need to reflect the same changing data. We recommend lifting the shared state up to their closest common ancestor. Let’s see how this works in action.

### In this section, we will create a temperature calculator that calculates whether the water would boil at a given temperature.

### We will start with a component called BoilingVerdict. It accepts the celsius temperature as a prop, and prints whether it is enough to boil the water:


# Lists and Keys

### First, let’s review how you transform lists in JavaScript.

### Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
This code logs [2, 4, 6, 8, 10] to the console.

### In React, transforming arrays into lists of elements is nearly identical.

# Rendering Multiple Components

### You can build collections of elements and include them in JSX using curly braces {}.

### Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems:

const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
We include the entire listItems array inside a <ul> element, and render it to the DOM:

ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
Try it on CodePen

### This code displays a bullet list of numbers between 1 and 5.

# Basic List Component
### Usually you would render lists inside a component.

### We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,
  document.getElementById('root')
);
When you run this code, you’ll be given a warning that a key should be provided for list items. A “key” is a special string attribute you need to include when creating lists of elements. We’ll discuss why it’s important in the next section.

Let’s assign a key to our list items inside numbers.map() and fix the missing key issue.

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li key={number.toString()}>
      {number}
    </li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,
  document.getElementById('root')
);