## How would you break a mock into a component heirarchy?
    Using single responsibility principle

## What is the single responsibility principle and how does it apply to components?
    is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part.

## What does it mean to build a ‘static’ version of your application?
    build components that reuse other components and pass data using props.

## Once you have a static application, what do you need to add?
    The state, to identify which component mutates

## What are the three questions you can ask to determine if something is state?
    1- Is it passed in from a parent via props? If so, it probably isn’t state.
    2- Does it remain unchanged over time? If so, it probably isn’t state.
    3- Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?
    - Identify every component that renders something based on that state.
    - Find a common owner component (a single component above all the components that need the state in the hierarchy).
    - Either the common owner or another component higher up in the hierarchy should own the state.
    - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
