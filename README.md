# react-interview-prep

Practice most frequently asked React concepts and coding challenges and questions

Resouces used to study:
- https://www.youtube.com/watch?v=XBTJDpT2XaI&ab_channel=freeCodeCamp.org

1. Map and Filter
    - map and filter can be used to edit items being passed in as arrays
2. State Management 
    - useState for functional components
    - old school class components as well with a constructor
3. Props
    - variable and functions can be passed as props to child components.
    - if you want the child prop to have the parent execute a function prop we call () => setName("value")
4. Inline Conditional Expressions
    - reminder to use <></> fragement and ternary operator
5. Event Handling
    - For event handling we can work with input to trigger an onChange to update and grab event target values
6. Keys in React
    - .map() has a second parameter for index
7. Forms in React
    - learned about `<form>` and `<input>` fields where you can control what gets passed in as parameters to not pass entire event object
    - `let data = {[name]: value}` AND `setFormData({ ...formData, ...data })` dynamics updates object for form data
    - buttons inside <form> can have type "reset" and "submit", add event.preventDefault() to avoid refresh
8. Dynamic Inputs
    - use the spread operator ... to get all previous elements
    - use `splice(index,1)` to remove an element at a given index
9. CSS Styling
    - You have external, inline, and internal styling that you can use
10. Uncontrolled vs Controlled Components in React
    - Uncontrolled components do not refresh but instead use reacts createRef hook to set the values and updates them as needed
    - Controlled components are your traditonal onChange that will refresh your component each time
11. VirtualDom
    - DOM structuted save in vode and the new updated nodes get updated as needed, 
    - reconciliation with virtual dom and dom
12. Inner HTML
    - Learned about `dangerouslySetInnerHTML={{__html: quill}}`
    - quill library for HTML based renders
    - JSX vs Inner HTML and when to use both
13. React Fragments
    - `<></>` if you want to add a Fragment
14. Stateless vs Stateful Components
    - the presence of useState makes a component stateful
15. Rest APIs
    - Use of the axios library, using POST, PUT, GET, PUT
16. Debouncing React
    - Debouncing = Run only certain functions a limited number of times then always getting triggered on changes to optimize broswer performance 
    - So we know about `useEffect`, in the dependency array when values change it will trigger the useEffect
    - You can add `setTimeout` and `clearTimeout` in order to run certain queries to optimize browser performance
17. ContextAPI 
    - `useContext` hook in React to pass things down to child componets and definiing it
    - `createContext` hook to create the context and pass it down
    - `<name of context>.Provider value={{}}` will populate the context for you from the parent component
18. Class vs ClassNames
    - `class=""` is how you do this in HTML, but you are using two class keywords for class React components
    - `className` is the preferred since it won't have that error displaying
19. Higher Order Components
    - You can add an extra return in a functional component as follows to make a boiler plate div generator
    ```
    const HOC = (title, Component) => {
        return function HOC(){
            return (<></>)
        }
    }
    ```
20. Lazy Loading
    - `React.lazy(() => import('./Lorem'))` to prevent loading a giant component with lots of file info
    - `Suspense fallback={}` will show another screen when something is loading into React component nifty!
21. Helper functions in React
    - best practice to have a folder with helper functions and having the wrappers that handle resolving promises in their own functions
22. Recursion in React
    - You can reference the component within itself in the return of the DOM structure
23. Array of Functions in React
    - To create an array of functions to execute in react you can create a generic function type and use map to run them and store the results to a list
24. Custom Hooks
    - A custom hook involves add all useEffect and useState to another file as a function where it just resolves data
    - You can use that hook inside another component to get data
25. Promises and Async/Await in React
    - create a promise as `new Promise((resolve, reject) => {})` and have the calls to this function
    - async/await cannot catch errors thus why we need `try{}catch{}` block to catch the errors for us
26. Code Splitting in React
    - so Webpack compiles all react code into a single bundle.js, this can be inefficient
    - to improve you dynamically import content by calling `import(<path>).then((module) => {})` which creates a `.chunk.js` additional file to not have it entirely be within the `bundle.js` file
27. Search Filter in React
    - Read the code for the filter it just combines all the elements very smoothly
    - `includes` is only for Objects so you have to convert strings to Objects like `Object.values(str).join('').includes`
28. Caching an API Response
    - `useQuery` and the `react-query` library to the rescue to be able to cache data from calls from APIs
    - `const {data, isLoading} = useQuery("data", ()=>{fetch().then()})`
