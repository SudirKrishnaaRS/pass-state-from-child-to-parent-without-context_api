## How to pass the child state into parent component?

# Solution : 
Passing the state from a child component to a parent component can be done using a callback function. The parent component can pass a callback function as a prop to the child component, and the child component can call that function and pass its state as an argument when it changes.

Here is an example:

Refer Parent.js and Child.js files

In this example, the parent component uses the useState hook to manage a piece of state called childState. The parent component also defines a handleChildState function that updates the childState state when called. This function is passed as a prop onStateChange to the Child component.

The Child component receives the onStateChange prop and uses the useState hook to manage its own state, state. The Child component also defines a handleChange function that updates its state when the input value changes and a handleSubmit function that calls the onStateChange prop and passes its state as an argument when the form is submitted.