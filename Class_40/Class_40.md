
## Q1. What is React Context, and how does it help in managing state and data sharing in a React application?

React Context is a feature in React that enables efficient state management and data sharing within a React application. It allows you to create a centralized data store (*context*) at the top level of the component tree. This context can then be accessed by any component in the application without the need for prop drilling, where data is passed through multiple levels of components via props.

React Context simplifies data sharing by providing a `Context Provider` component that wraps the parent component tree and holds the shared state. Child components can consume this data using the `Context Consumer` component, accessing the context data directly. This approach reduces component coupling, makes the codebase cleaner and more maintainable, and avoids passing props down the component tree.

## Q2. Explain the `useContext` Hook and how it can be used to access data from a React Context within a functional component

The `useContext` hook is a feature introduced in React 16.8 that provides a simple way to access data from a React Context within a functional component. It allows you to consume data that has been provided by a `Context.Provider` component higher up in the component tree without the need to use a `Context.Consumer`.

The `useContext` hook takes the context object created by `React.createContext()` and returns the current context value, which was provided by the nearest matching `Context.Provider` in the component tree.

Here's the syntax of `useContext`:

```jsx
const contextValue = useContext(MyContext);
```

Where `MyContext` is the context object created by `React.createContext()`.

## Q3. Describe the purpose of Next.js, and provide an example from the Vercel Next.js Examples reading on how it can be used to build a scalable web application

Next.js is a React framework used to build server-rendered and statically generated web applications. It abstracts away complexities, enabling developers to focus on building application logic while handling optimizations like server-side rendering and dynamic routing. An example, like the "Blog" example from Vercel's Next.js Examples, demonstrates how Next.js simplifies creating scalable web apps with server-side rendering, dynamic routing for blog posts, and optimized performance through automatic code splitting.
