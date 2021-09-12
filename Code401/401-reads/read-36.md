## React example
    ```
    ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
  );
   ```

## Introducing JSX
    JSX produces React “elements”.

    example:
```
const element = <h1>Hello, world!</h1>;
 ```

## Rendering an Element into the DOM

```
<div id="root"></div>
```

## Function and Class Components

    The simplest way to define a component is to write a JavaScript function:

```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

## Next.js
    To build a complete web application with React from scratch, there are many important details you need to consider:

    Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
    You need to do production optimizations such as code splitting.
    You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
    You might have to write some server-side code to connect your React app to your data store.

## Tailwind css example
```
    <div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-md flex items-center space-x-4">
        <div class="flex-shrink-0">
            <img class="h-12 w-12" src="/img/logo.svg" alt="ChitChat Logo">
        </div>
    <div>
        <div class="text-xl font-medium text-black">ChitChat</div>
            <p class="text-gray-500">You have a new message!</p>
        </div>
    </div>
```
