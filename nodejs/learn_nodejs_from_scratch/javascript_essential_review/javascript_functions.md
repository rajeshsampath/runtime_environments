# JavaScript Functions
#### Learn about functions in JavaScript.

By the end of this lesson, we’ll be able to do the following:
>   - Use the ES6 arrow function syntax.
>   - Create default function parameters.

# ES6 functions: arrow functions

-   Arrow functions were introduced in ES6.

>   Let’s take a look at this example, which uses an ES5 function expression syntax:
>       var printName = function (firstName, lastName) {
> 
>             return `${firstName}${lastName}`;
> 
>       };
> 
>       output = printName("educative.","io");
> 
>       console.log(output);

-   To convert the printName() function to use the ES6 arrow syntax, we’ll have to follow two steps:
    -   Drop the function keyword.
    -   Add a fat arrow between the parentheses and opening curly brace.

>   -   The resulting function will look like this:
>       const printName = (firstName, lastName) => {
> 
>           return `${firstName}${lastName}`;
> 
>       };
> 
>       output = printName("educative.","io");
> 
>       console.log(output);

-   If our function immediately returns a value, the curly braces that wrap the function body and return statements aren’t needed. The value is implicitly returned.
    -   Here’s the shorthand we can use:
>   const printName = (firstName, lastName) => `${firstName}${lastName}`;
> 
>   output = printName("educative.","io");
> 
>   console.log(output);