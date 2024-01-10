# React1
Q.1- What is React ?
Ans.- React is a flexible and efficient Javascript library for building user interfaces.
React lets you compose intersting and complex UIs from small isolated pieces of code called components.

For an instance :

function Message(props){
    return (
        <div className = "my-name">
            <h1>Hello my name is {props.name}</h1>
        </div>
    );
}

Here, `Message` is a React component. A component takes in parameters, called props(properties), and displays its return value.

Q.2- Who made React ?
Ans.- 'Jordan Walk' a Facebook engineer created React. It was first introduced in May 2013. He worked on the prototype and created
React to come up with a solution for managing Facebook ads.

Q.3- What is Babel ?
Ans.- Babel is a free and open-source Javascript transcompiler that is mainly to convert latest Javascript code into the one that 
the browser undestands. Babel is a popular toolchain for web developers. Main things Babel can do include transforming syntax, 
source code transformations.

Q.4- How does Babel convert html code in React into valid code ?
Ans.- The compilation of html through Babel happens in three main steps:
    1.Parsing - In this step, Babel parses the code into an Abstract syntax tree(AST), which represents the code structure.
    2.Transforming - In this step, the AST is passed through various transformations. The JSX transform plugin converts JSX into
      React.createElement calls.
    3.Generating - In this step, the transformed code is generated.

    For instance:

    // JSX Code
    const App = () => {
    return <div>Hello, JSX!</div>;
    };

    // After Babel Transformation
    const App = () => {
    return React.createElement('div', null, 'Hello, JSX!');
    };


Q.5- What is ReactDOM used for? Write an example ?
Ans.- ReactDOM acts as a bridge between React components and actual DOM elements that make up a webpage.

For an instance, the following code renders a <h1> element into a <div> element with id "root":

// using root template--

const element = <h1>Hello, world!</h1>;
ReactDOM.render(element, document.getElementById('root'));


Q.6- What are the packages that you need to import for react to work with ?
Ans.- Some of the useful libraries that we need to import in order to create React projects are-
    1. A Create-React-App.
    2. A Data Fetching library.
    3. A Dead-Simple state management library.
    4. A powerful component library.
    5. A Hook-Based Form library.

Q.7- How do you add react to a web application ?
Ans.- Simply, we can create a new project on VS code and select React.js
Other ways to create a React web application include using the tag on an HTML web page, Create-React-App, and Gatsby etc.

Q.8- What is React.createElement ?
Ans.- React.createElement() is a method in React that creates a new React element. It is used to create a virtual representation
 of a DOM element or a user-defined component. The method takes three arguements:
 1. Type- HTML tag names "div", "h1", "span" etc.
 2. Props- className, id, style etc.
 3. Children- The child elements of the element being created.


Q.9- What are the three properties that createElement accept ?
Ans.- Three properties that createElement accepts are-
 1. Type- HTML tag names "div", "h1", "span" etc.
 2. Props- className, id, style etc.
 3. Children- The child elements of the element being created.


 Q.10- What is the meaning of render and root ?
 Ans.- Render means "give-back, restore, return". In React render() is a function that displays the specified HTML code inside
  the specified HTML element.

  Root refers to the element that exists in the original HTML that all of the React contents go into. In React, the root component
   is the component at the top of the component tree, and is the first component to be rendered. 
