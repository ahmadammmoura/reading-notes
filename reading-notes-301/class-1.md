# What Is React?

### React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

### React has a few different kinds of components, but we’ll start with React.Component subclasses:

![V2](https://hackernoon.com/hn-images/1*HSisLuifMO6KbLfPOKtLow.jpeg)


# The smallest React example looks like this:

``react
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
``

### It displays a heading saying “Hello, world!” on the page.



# Why JSX?

### React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

### Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

### React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

### With that out of the way, let’s get started!

# Components and Props

### Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components.