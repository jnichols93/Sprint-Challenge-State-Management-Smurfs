1. What problem does the context API help solve?

Prop drilling is a common pattern of passing props all the way from a root element to its children whenever its needed, if there's 15 child node elements all of them will have to pass props. Almost like youre at whole foods, your name is Karen and you have 15 children on one leash, well you want to tell little braxton to get the gluten free sphagetti sauce from the bottom shelf, because you have bad knees due to the sheer presence of 15 children but hes off picking his nose and staring off into the distance, and you cant just yoink him into action with a firm pull of the leash without sending all 14 other children airborne(in this scenario you also lift alot), now imagine having individual  custom leahes for each child, although its additional set up, you can now rest assured your child will be flying into the sauce at landspeed record levels.  SO BASICALLY context API this chain can be escaped and we can pass props straight to the desired child.

1. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
1. What is the difference between Application state and Component state? When would be a good time to use one over the other?

Actions are verbs or things you cand do duh. For real though, basically events triggered by the UI, they're telling reducers exactly what has to be done and are passing some of the necessary information. Reducers accept that object info and type of an action, and are returning the new state to the entire application. 

Store allows UI elements to grab pieces of global data all over the app. Store is known as a single piece of truth because it passes the global state everywhere where individual components then are allowed to choose which pieces of state they need to grab.

1. Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?
It allows Redux to run asynchronously, meaning not having to wait for an API call to do something else in the application. It changes the calling of an action because now we're nesting themm together like asyncFunc => data => dispatch => {}

1. What is your favorite state management system you've learned and this sprint? Please explain why!
I like Redux Thunk because it makes calling APIs easier, I cant wait to spend some time this weekend broadening my understanding a little bit more!