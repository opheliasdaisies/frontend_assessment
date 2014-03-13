# Frontend Assessment Part 1

### HTML

- What does "semantic markup" mean?
  Semantic markup is when element names have meaning that indicate their purpose. For example, using a footer element instead of a div, or using the strong tag instead of b.
- What does a doctype do?
  A doctype specifies what markup language you are using so that the browser knows what rules to use.
- Explain what standards and standards bodies are and why they are important.
  Standards are a convention that is decided on for what browsers will support. They are important because without them, it would be difficult to know what elements would work on different browsers.
- What are CSS3 and HTML5? How are they different from previous standards? Why is this important?
  CSS3 and HTML5 are the latest standards for CSS and HTML. They are considered "living standards", which means they will change over time as new aspects are built. This is important because it is a large change from how standards worked in the past, and it means that changes and improvements will be able to be incorporated mroe quickly instead of having to wait for the next release of CSS or HTML.

### CSS

- What does a CSS reset do and why is it useful?
  A CSS removes the default styling that the browser would provide. This helps mitigate differences between how different browsers display various elements.
- What is the box model? Draw a picture and label the portions here.
  The box model is the order of the different components of a piece of content. It includes content, padding, border, and margin.
  
     -----------------------------------
    |              margin               |
    |   -----------border------------   |
    |  |   ----------------------    |  |
    |  |  |        padding       |   |  |
    |  |  |  -----------------   |   |  |
    |  |  | |     content     |  |   |  |
    |  |  |  -----------------   |   |  |
    |  |   ----------------------    |  |
    |   -----------------------------   |
     -----------------------------------

- What is the difference between a relative, fixed, absolute, and statically positioned element? Feel free to draw pictures to explain your answer.
  A relative element is positioned a specified number of pixels in relation to its default position. Its original place in the dom is preserved.
  A fixed element is positioned in relation to the window, and will not move as the page scrolls.
  An absolute element is positioned in relation to its closest positioned parent. If no parent is positioned it is positioned in relation to the window.
  A statically positioned element has its default positioning.
- What is SASS and why do people use it?
  Sass stands for syntactically awesome stylesheets. It is a CSS pre-processing language. It allows you to use features not included in CSS, like nesting, variables, and mixins, and will compile to CSS.
- Name one feature of SASS and explain why it is helpful.
  One feature of SASS is the use of variables. It is useful because if you decide to change the value for something that is repeated throughout your CSS file, you only need to change it in one place.

### JS

- Explain prototypal inheritance.
  Prototypal inheritance is when you create an object that inherits properties from another object. This is used in Javascript because true classes do not exist in Javascript. All objects in Javascript have a prototype, and this is what is used as a model when creating an instance of the object.
- What is a closure and how/why would you use one?
  A closure is a way to contain a specific varaible in the scope of a function. You use it by defining, but not calling, a function in another function, and returning that function. This will allow you to pass in an argument while setting the function equal to a variable, and then that argument will be "closed over" in the scope of the function when used by calling it via the variable. An example of when you would use it would be if you wanted to use a setTimeout function inside a loop, since setTimeout has a global scope.
- What is an anonymous function? Give a typical usecase for one.
  An anonymous function is a function that is not named. A typical usecase is if you want to pass a function as an argument.
- Describe the difference between 
  - `function Person(){}`  This is creating a new constructor for an object Person.
  - `var person = Person()`  This is setting the variable person equal to the object constructor Person.
  - `var person = new Person()`  This is setting the variable person equal to an instance of the Person object.
- Explain hoisting.
  Hoisting is Javascript's practice of instantiating all variables at the very top of the document. However, only the instantiating, and not the defining of variables, are hoisted.
- What is the difference between `===` and `==`?
  === checks to make sure that two items are equal in both value and type. == checks to make sure that two items are equal in value, but they can have different types and still be considered equal. For example, 2 === "2" would return false, but 2 == "2" would return true.
