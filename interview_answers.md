# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?

    Context API allows you to share values between components without having to pass props through every level of a tree, making it easier to give components a local preference or UI theme.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

    Actions are objects with information that are sent to the reducer, that identify which slice of state to change and the changes needed for the update. Using an action allows our reducer to be a pure function. Reducers are pure functions, that change the current slice of state. They do so by making a copy and then replacing the previous state with that copy. The store is an object where all of the global state is held. It is never mutated. The store is known as the single source of truth since that is the only place with state that can be passed to where ever the data is needed.  

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?

    Redux-thunk allows us to make API calls in our action-creators by changing them to be asynchronous.  

4. What is your favorite state management system you've learned and this sprint? Please explain why!

    My favorite state management system I've learned this week is redux. Even though it has many pieces split up all over the place, it makes it easy debug by just following the flow of the code. Also having the ability to just add in props with out having to pass them everywhere is much easier to implement.
