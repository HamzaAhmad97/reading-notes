# Thinking in React

1. To break a mock into a component heirarchy, we can start by drawing boxes around components and their subcomponents, this is similar to what we used to do when building or drawing a wireframe for a website, then as we do when we think about a problem that might need a special function or object, to be responsible for doing a specific task or set of tasks, in order to be able to decide what pieces of our webiste need to be a stand alone component.

2. The **single responsibility principle** is a principle used to help choosing which parts of an applicaton deserve to be a component, this is done by thinking about the functionality a component might be able to provide. And if you think about it, when you do that correctly, this will reflect on the UI itself, and you will notice that this also helps make the UI more consistant depending on the data and information the component handle.

3. To build a static version of an app is similar to saying that we want to only see the UI and the data model, but the webiste will have no interactivity, so the components will only have the render() method at this stage, and passing data is only done using props.

4. Once you have the static version of your app you will then need to add things that will handle the state, that is, to add interactivity.

5. To determine if something is state we might ask these three questions:

* *Is it passed in from a parent via props? If so, it probably isn’t state.*
* *Does it remain unchanged over time? If so, it probably isn’t state.*
* *Can you compute it based on any other state or props in your component? If so, it isn’t state.*

Source: [reactjs.com](https://reactjs.org/docs/thinking-in-react.html).

6. To figure out where state will live, we can start by checking which components render based on its state, then you might need to check a common container or component that is above all components to add state to it, this component might need the state. This common component or another one at a higher level should own the state, and in case you do not find such component that can hold the state, create a separate one to hold the state.

