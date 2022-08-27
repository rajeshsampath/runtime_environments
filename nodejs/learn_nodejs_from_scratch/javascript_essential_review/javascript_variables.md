# JavaScript Variables:
##### Learn about the different types of variables available in JavaScript

By end of this reading, we'll be able to understand the difference between ***var***, ***let***, ***const*** and how to use them correctly.

In javascript, variables can be declared with ***var***, ***let***, ***const***.

> **Note:** The ***let*** and ***const*** keywords were introduced in ES6 and are they preferred variables declaration methods for our study.

# Variable Update:

The ***var*** variables can be updated and redeclare with in its scope.

Let's take a look at the code below. ***What will be logged to the console? and Why?***
>   `var color = "red";`
> 
>   `var color = "yellow";`
> 
>   `console.log(color);`
> 
>   **Output: yellow**

The value ***yellow*** is logged because ***var*** variables can be updated and redeclare within its scope.

While ***let*** variables can be updated, but they can't be redeclare.

Now, let's take a look at the code below. ***What will be logged to the console? and Why?***
>   `let color = "red";`
> 
>   `let color = "yellow";`
> 
>   `console.log(color); // SyntaxError: Identifier 'color' has already been declared`
> 
> 
>   `let greeting = "hello";`
> 
>   `greeting = "hi";`
> 
>   `console.log(greeting); // 'hi' is logged, since `let` variables can be updated`

The const variables can neither be updated nor redeclared

> const color = "red";
> 
> color = "yellow";
> 
> console.log(color); // TypeError: Assignment to constant variable.


Setting a **const** data item to an object is interesting.

Once we’ve assigned an object to *const*, we can’t reassign the *const* data item to a different object, but we can update the *methods* and *properties* on the object.

>   const computer = {
> 
>   type: "Macintosh",
> 
>   os: "Catalina",
> 
> };
> 
> computer.type = "Microsoft";
> 
> computer.os = "Windows 10";
> 
> console.log(computer); // { type: 'Microsoft', os: 'Windos 10' }
> 
> computer = {
> 
>   type: "Chromebook",
> 
>   os: "Chrome OS",
> 
> };
> 
> console.log(computer); // TypeError: Assignment to constant variable.

The ***var*** variables are global or function scoped.

The ***let & const*** variables are block scoped.

# Variable hoisting

Hoisting describes the default JavaScript behavior of moving variable declarations to the top of their scope. 

The *var, let, and const* variables are all hoisted, albeit a little differently.

During hoisting, *var* variables are initialized to *undefined*.

So trying to access a variable declared with *var* before the declaration returns *undefined*.

Trying to do the same with *let or const* will return a *ReferenceError* because they aren’t *initialized* during *hoisting*.

