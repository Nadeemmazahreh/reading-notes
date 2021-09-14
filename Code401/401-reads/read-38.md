## What is React context?
    React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

## When should you use React context?
    React context is great when you are passing data that can be used in any component in your application.

    These types of data include:
    -   Theme data (like dark or light mode)
    -   User data (the currently authenticated user)
    -   Location-specific data (like user language or locale)

## What problems does React context solve?
    React context helps us avoid the problem of props drilling.

    Props drilling is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.

## How do I use React context?
    Context is an API that is built into React, starting from React version 16. This means that we can create and use context directly by importing React in any React project.

    There are four steps to using React context:
    -   Create context using the createContext method.
    -   Take your created context and wrap the context provider around your component tree.
    -   Put any value you like on your context provider using the value prop.
    -   Read that value within any component by using the context consumer.

## Next.js 

    Next.js, the React Framework. Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the pit of success when building React applications. 
    
    Next.js aims to have best-in-class developer experience and many built-in features, such as:
    -   An intuitive page-based routing system (with support for dynamic routes)
    -   Pre-rendering, both static generation (SSG) and server-side rendering (SSR) are supported on a per-page basis
    -   Automatic code splitting for faster page loads
    -   Client-side routing with optimized prefetching
    -   Built-in CSS and Sass support, and support for any CSS-in-JS library
    -   Development environment with Fast Refresh support
    -   API routes to build API endpoints with Serverless Functions
    -   Fully extendable
    -   Next.js is used in tens of thousands of production-facing websites and web applications, including many of the world's largest brands.