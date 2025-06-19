## Pre requisite Java Script for learning React

### Arrow Functions
It is common in Javascript to create a function like so:
'''
function myFunction() {
    ... do something
}
'''

While this is perfectly valid in ReactJS it is more common to see arrow functions which are created with this syntax:
'''
const myFunction = () => {
    ... do something
}

This is due to the fact that by using const, it prevents the function from being overwritten in the code, because it's a constant now.

Arrow functions also prevent hoisting, which is when you are able to use a function before it's defined. This is better in my opinion
because it forces developer to pre-define their function which means they should have an idea of what their code is going to do before
it runs. Hoisting opens the door to eractic behaviour and bugs that could be very difficult to debug.

In summary make sure to use Arrow Functions when creating ReactJS applications as they enforce stricter coding practices and structure, resutling in 
more clarity, predictabiliy, and immutability.

### Anonymous Functions
Anonymous functions are almost the exact same as they are in Python with just slighlty different syntax.

() => { console.log("Hello World")};

This above would be an example of an anonymous function.

You might recognize this because it's very similar to how we create arrow functions. If we look at the code below:

const myFunction = () => {
    ... do something
}

What's really going on is that we are creating a constant called myFunction and we are assigning it the value of an anonymous function. 
This really just enforces the idea that in JavaScript, functions are treated just like other values such as ints, strings, and floats.


#### Why use anonymous functions?

The biggest benefit to using anonymous functions is that you are able to use them in-line which comes in handy when you need to pass in a function
with very simple logic. This prevents you from having to define and create a whole function which although is more explicit, it can be annoying for traceability as the reader of your code now needs to look for your function definition to understand your logic. On another note, they simply reduce
lines of code significantly.


