### 7. React
#### State and Lifecycle Hooks


---

#### What is state?

* The data that defines the condition of some object or system.
* The television is off. The coffee is hot. These are states.
* Difference between a value and a variable - the number 42 does not have a state since you can't change it.
* A clock is a good example


---

#### Component state

* Every component can have its own local state.
* Only class components have the state functionality.
* State is something you set up by yourself, not like props.
* Every time the state is updated, the render method will run.


---

####  Set the initial state in the constructor
```JavaScript
constructor(props) {
  super(props); // Always pass props to base constructor
  this.state = {name: 'John Doe};
}
```


---

####  Set the initial state in the constructor
```JavaScript
constructor(props) {
  super(props); // Always pass props to base constructor
  this.state = {
    name: 'John Doe',
    date: new Date()
  };
}
```


---

####  State is an Object
```JavaScript
constructor(props) {
  super(props);
  this.state = {date: new Date()};
}

```
```
<h2>It is {this.state.date.toLocaleTimeString()}.</h2> //JSX
```


---

####  Updating state
#### # Wrong and does NOT trigger re-render and update

```JavaScript
this.state.comment = 'Hello';
```
#### # Correct - will trigger re-render and update

```JavaScript
this.setState({comment: 'Hello'});
```


---

####  When you call setState(), React merges the object you provide into the current state.

```JavaScript
this.state = {
  posts: [],
  comments: []
};

this.setState({posts: ['hello', 'john']});
this.setState({comments: ['drinking java', 'cool']});
```

These are called independently


---

####  Second argument is a callback that runs after state is updated

```JavaScript
this.state = {
  posts: [],
};

this.setState(
  {posts: ['hello', 'john']},
  () => {console.log('state is updated')
);
```


---

####  Setting a nested state

```JavaScript
this.setState({
    key: {
    key: value
  }
});
```


---

#### Top-down / Unidirectional data flow

* Components have now idea if some other state is passed down to them. They will always get it as props.
* The parent component does not know if the child is a class or a function.
* The state is local or encapsulated. It is not accessible to any component other than the one that owns and sets it.
* State can only affect components “below" them in the tree.


---

#### Top-down / Unidirectional data flow
<img style="width: 700px" src="/new-structure/media/react-images/react-7/dataflow.png" alt="lifecycle methods">


---

#### Lifting up state
<img style="width: 700px" src="/new-structure/media/react-images/react-7/liftingstate.png" alt="lifecycle methods">


---

#### Lifecycle Hooks (methods)

* **componentDidMount** - is invoked when the components output rendered to the DOM for the first time (mounting).
* **componentDidUpdate** - is invoked immediately after updating occurs. This method is not called for the initial render.
* **componentWillUnmount** - is invoked when the DOM produced by the Component is removed (unmounting).


---

#### <a href="https://reactjs.org/docs/react-component.html#mounting">Lifecycle Methods</a>


---

<img src="/new-structure/media/react-images/react-7/lifecycles.png" alt="lifecycle methods">