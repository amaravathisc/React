# React

hooks
------------
Hooks are a new addition in React 16.8. 
They let you use state and other React features without writing a class. Hooks are backwards-compatible.
always use Hooks at the top level of your React function, before any early returns. 
By following this rule, you ensure that Hooks are called in the same order each time a component renders. 
That's what allows React to correctly preserve the state of Hooks between multiple useState and useEffect calls.

useEffect will control the rerendering STAtements, in useEffect we use two arguments first one anonymous function, we add some statements that can be 
executed, and second arguments we give the dependency

useEffect(()=>{})----------> it executes every render, every refreshing page it will executes
useEffect(()=>{}, [])-----> [] empty subscript, it executes only first render
useEffect(()=>{},[dependency])-------->first it will execute the statement,next time it will depend on dependency

useCallBack: memorized version of the callback that only changes if one of the input has changed, it prevents situation(unneccessory renderings), it will not allowed to recrete

await:it returnsthe promise, it will returns value, it will fetch data from api

What are props in React JS?
Props are arguments passed into React components. Props are passed to components via HTML attributes. props stands for properties.

Declaring function:

function app(){
return(
<React.fragment>
</React.fragment>
)
}
in this app functional component what it return , it returns the <React.fragment>

why do we use <React.fragment> in return statement?
because its replacement of <div>
<React.fragment> it contains the components, we need to call the segments

how we r going to create custome hook
