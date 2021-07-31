## Component Based Architecture

* A component can be thought of as an element that represents a concrete independent piece of functionality or an interface that is used to build wider UIs, which is just like objects, allows us to hide implementation details and use a higher level interface to interact with that component, although components usually do not depend on the context they are used in on contrary to objects and some functions.

* The characteristics of a component can be sorted as follows:
Components are made to be reused over and over again while applicable, which allows us to save time and effort. Since components are reusable because they do not depend on the environment or the context they are being used in, they can be replaced by other components when needed which provides a lot of flexibility. Components can be be extended from other components to provide more functionality. Just like objects and even functions, to avoid repeating and wasting time understanding the details of implementation, components offer an interface through which we can use its functionality without the need of even looking into the details behind that component. Lastly, since almost all of components’ characteristics arise form each other, components are also independent, which means that the dependencies on other components and outer code can be brought to its minimum.

* The advantages of using the component based design can be sorted as follows:
Since components can be replaced with others, this provides ease of deployment, meaning that when there is a newer version of an existing code, the older one can be replaced easily without the need to modify the original code. From the characteristics of components, we can deduct that this architecture saves as time and effort which reflects on reducing cost in terms of maintenance and development.  Dealing with component based programs makes it easy to develop which also reflects on the ease of maintenance and evolution since they encapsulate and hide the details and expose interfaces to gain control of the functionality. This is a reliable paradigm  since every component is itself considered reliable which affects the overall reliability of the system. Since every component is independent on its own and can be used independently of any context of environment it affects the connectivity of components positively and affects the speed of development as well as  productivity. 

## What is Props and How to Use it in React

Props is short for “properties” which is a mean of passing data from a component to the other in a uni-directional flow, usually from the parent to the child, and this type of data is read-only which means that the child should not modify or overwrite this data.

