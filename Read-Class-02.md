## React lifecycle

1. Based on the diagram, it shows that the 'render' does happen before 'componentDidMount'.
2. The first thing that happens in a lifecycle of React is the mounting phase, which takes place when an instance of a component is created and gets inserted into the DOM, it starts by calling the constructor of the component class.
3.  constructor -> render -> React Updates -> componentDidMount -> componentWillUnmount.
4. What componentDidMount does is that it allows us to execute the React code when the component is already placed in the DOM.

## Reaact State vs Props

1. Props can be passed things that are used mostly to initialize state or the initial shape of a component, and this type of data might differ depending on the properties od the component itself and what it needs to get rendered.
2. The difference between props and state is that props is usualy the things that you pass to the component while state is actually a representation for the internal state of the component, meaning that it is something inside of the component while props is handeled outside. Props must be updated outside the component while the state is handelled internally.
3. When you change the state of a component or a part of the applicaton, it is going to re-render that part of the application.
4. Examples on things that can be stored in state are counters, and form fields' values and so on.

