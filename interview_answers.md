# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?
The API helps keep the state clean. Context provides a way to share values between components without having to prop drill, explicitly pass a propr through every level of the tree. 

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
Actions are pieces of data that contain the action type and data. These actions are dispatched to the reducer which then updates the state according to the type and payload associated with the action. Reducers are pure functions with no side-effects that take two arguments, state and action. They then return a new updated state object. A store is an immutable object tree in Redux. It is a state container which holds application's state. The only way to change the data in the UI is to dispatch an action that will change the state within the reducer. 

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?
Redux-thunk allows us to make the reducer flow asynchronous. The redux-thunk middleware intercepts the normal redux flow. The action-creator returned thunk then has access to the dispatch function allowing it to run an async funtion. 

4. What is your favorite state management system you've learned and this sprint? Please explain why!