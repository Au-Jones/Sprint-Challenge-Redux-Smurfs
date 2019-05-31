1.  Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?

map,reduce,filter do not produce side-effects. we use map to create a new object.

1.  Describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

actions- functions that pass along data from your app to the store and are the source of information for the store

reducers- specify how the state changes in response to the actions. they capture info and put it in the state.

store- all of your state lives here in redux. holds the entire state tree and allows us to send state where ever its needed.

1.  What is the difference between Application state and Component state? When would be a good time to use one over the other?

ApplicationState- lives in the store and is global.
good time to use this would be when data needs accessed from multiple places in the app.

ComponentsState- lives in the component and is local.
good time to use this would be when short term data needs changed such as the characters present in the text as the user types.


1.  What is middleware?

a function that that returns a function that returns a function

1.  Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

Thunk is a middleware that allows yo uto call action creators that return a function instea of an action object.
    it changes our action-creators by letting the function recieve the stores dispatch method, which then uses the dispatch synchronous actions in the function once the asynchronous ops have completed.

1.  Which `react-redux` method links up our `components` with our `redux store`?

connect()()

