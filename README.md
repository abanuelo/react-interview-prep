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
12. Inner HTML, (left off at 1:46:00)