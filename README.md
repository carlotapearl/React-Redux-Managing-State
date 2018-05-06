# React-Redux-Managing-State
The Iron Yard, React Redux Part 1: Paired Programming Activity (September 2017)

## App Description  
In this project, you will refactor three components (`films`, `starships`, `view`) in order to manage their state via Redux. You will author a simple action, for `Starships` and `Films`, that will produce an alert with specific data for each. You will also author an action to the the state for the `Details` page.
To achieve this, you will need to implement:
  * Reducers
  * Actions
  * Dispatchers
  * Store
We have already refactored the People component and added two actions. One that displays an alert (with the character's homeworld) when the user clicks on a button. The other (commented out), is used to set state in the Details page.

## Instructions  
### General  
The following refactoring and functionality still need to be implemented:
1. Refactor the Starships and Films components so that their state is managed with Redux.
2. Refactor Filmsdata.js and Starships.js to export as a function. This is needed in order to properly set up their respective reducers.
3. Add two actions (and action types), one for each component. These actions needs to be hooked to a button (inside each of the containers's 'list' nested component), titled 'actions', and when clicked an alert should display the following; for Films show 'director', for Starships show 'model'.
4. Once you have these actions successfully calling the alert, the next step is to add a reducer to set state.
5. Name the reducer stateExample. This reducer will take all your actions and will return a string with a message (i.e, "Just triggered SHOW_MODEL actionType and set state!"). Then, in the rootReducer, you will pass in stateExample so that it becomes available in state.
6. There is a fourth action, DETAILS. It has been set up for you and along with a function, setDetails. Study how this action and function are used in the Details container to set state and use its props to render the data. Uncomment this action and function once you are done refactoring the View component and all your other actions and reducers are working.
7. Refactor the Details component (in View.js), paying attention to how the data is accessed in componentWillMount. Here you will use the 'setDetails' action to set the state.

## Files  
We have created all the necessary files for you. You will need to add the appropriate Redux and React functions and files in containers, actions, actionsTypes, and reducers.
index.js: remember to change the paths for Films and Starships. Currently, the paths for each is pointing to the components folder, instead of the container folder.
There are detailed instructions in each file. Read them carefully!

## Suggestions  
Study how People was refactored in order to implement Redux (component, container, action, action type, reducer, etc) and use this as a guide, while following the workflow chart below. Don't just copy each function, but think of them critically.
Focus on refactoring Films and Starships, first. Then, refactor View.js
When authoring all the necessary Redux functions, do not just copy all of the refactoring we have done for you already, but take a moment to think of the Redux workflow and how it applies to the project. There are a lot of moving pieces and understanding where and how each one fits is key to understanding Redux.

![Redux workflow](https://github.com/carlotapearl/React-Redux-Managing-State/blob/master/redux-workflow.jpg)

## Getting started  
1. Download the zip file, and place where you keep projects
2. Change directories into the project
3. Install the dependencies - npm install
4. Fire up the server - npm start
5. Open console.

## Your role as a student
Articulate their ideas as best you can. Try to facilitate effective collaboration with your paired student. Be willing to debate strategies for how best to approach your challenge, but don’t allow endless debate to keep you from making progress. Keep your eye on the clock and try to work yourself through the challenge at a reasonable pace. You and your partner should share the responsibility for authoring ideas and code. Finish your challenge and make certain that you call talk someone through the logic and strategies implemented by your group.
