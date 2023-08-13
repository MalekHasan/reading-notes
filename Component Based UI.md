# Component Based UI

## React Quick Start


**Read the React Quick Start quide, to refresh your memory on React.**

1. What are the building blocks of a React app?
 ***The components.***

2. What is the difference between an HTML element and a React component?
***React component names must always start with a capital letter, while HTML tags must be lowercase.***

3. What is JSX and why do we use it?
 ***It's a markup syntax extension to Javascript so the code will look like HTML but it's JS,most React projects use JSX for its convenience.JSX is stricter than HTML.***
4. Describe the process of embedding JavaScript expressions in JSX.
***JSX is stricter than HTML. You have to close tags like <br />. Your component also can’t return multiple JSX tags. You have to wrap them into a shared parent, like a <div>...</div> or an empty <>...</> wrapper.***

5. Does React or JSX have any special features for iteration or conditional logic?
***Yes,You will rely on JavaScript features like for loop and the array map() function to render lists of components. Also ,You will rely on JavaScript features like conditional logic ( && || ? : !..etc), there is no special syntax for writing conditions. Instead, you’ll use the same techniques as you use when writing regular JavaScript code.***

6. How does React know to respond to a user’s inputs?
***You can respond to events by declaring event handler functions like(onClick) inside your components.React will call your event handler when the user clicks like on button.***

7. What word indicates that a React component manages data with a Hook?

***Functions starting with use are called Hooks.***

8. How can two react components share data?
***There is alot of way that react components can share data eact toghether using props, context API ,redux or etc...***

## Render and Commit

1. What are the three steps of refreshing a React UI?

- Triggering a render.
- Rendering the component.
- Committing to the DOM.

2. How do you trigger updates to a component after the initial render?
***Once the component has been initially rendered, you can trigger further renders by updating its state with the set function. Updating your component’s state automatically queues a render.***

3. Does React recreate DOM nodes on every rerender?

***React uses a virtual DOM (VDOM) to efficiently update the actual DOM. When a component re-renders, React creates a new virtual DOM representation of the component's UI. It then performs a diffing algorithm to compare the new virtual DOM with the previous one. This diffing process identifies the minimal set of changes needed to update the actual DOM, and only those specific changes are applied to the real DOM.***

4. After React has updated the DOM, what still needs to happen before the user sees the change?

***After rendering is done and React updated the DOM, the browser will repaint the screen. Although this process is known as “browser rendering”, we’ll refer to it as “painting” to avoid confusion throughout the docs.***

## Additional Questions

1. Note the naming conventions in the Airbnb React/JSX Style Guide. What pattern(s) do you see?
***Use PascalCase for React components and camelCase for their instances.***