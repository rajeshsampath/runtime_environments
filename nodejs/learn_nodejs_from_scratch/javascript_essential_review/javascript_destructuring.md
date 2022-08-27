# JavaScript Destructuring
#### Learn about destructuring in modern JavaScript.

By the end of this lesson, we’ll be able to destructure objects, arrays, and function parameters.

# Destructuring

When we have to access numerous properties from an object, such as state or props in a React component, we can use destructuring assignment.

This avoids assigning the properties to a variable one by one, resulting in cleaner syntax.

We can destructure objects, arrays, and even function parameters.

# Destructuring objects

The destructuring syntax allows data to be easily extracted from arrays or objects into separate variables.

Take a look at the code below:

>   const person = {
> 
>       name: "Hou Chia",
> 
>       title: "software engineer",
> 
>       city: "Brooklyn,NY",
> 
>       age: 32,
> 
>   };
> 
>   console.log(person);


If we wanted to extract the values from the person object into variables that we can use in our program, we might write something like this:

>   const name = person.name;
> 
>   const title = person.title;
> 
>   const city = person.city;
> 
>   const age = person.age;
>    
>   console.log(name);

With destructuring, we can accomplish the same thing in one line of code:

>   const { name, title, city, age } = person;
>   
>   console.log(name, title, city, age);


# Destructuring arrays

We can also destructure arrays as follows:

>   const letters = ["a", "b", "c"];
> 
>   const [firstLetter, secondLetter, thirdLetter] = letters;
> 
>   console.log(firstLetter) // a

We can also assign default values using =:

>   let [a = 4, b = 3] = [2];
> 
>   console.log(a); // 2
> 
>   console.log(b); // 3


# Destructuring parameters

We can also use destructuring to simplify the arguments passed to a function.

If a function takes more than one parameter, we can pass in an object that contains possible key-values and destructure the object.

The function **introduce()** below accepts four arguments:

>   const introduce = (name, title, city, age) => {
> 
>       console.log(`Hello, my name is ${name}, and I'm a ${title}. I live in ${city}, and I'm ${age} years old.`);
> 
>   };
> 
>   introduce("Hou", "software engineer", "Brooklyn, NY", 32);

When calling the introduce() function, the order in which the arguments are passed to the introduce() function matters here.

If the order of any two arguments were to be accidentally switched, then the function would output a nonsensical message.

With destructuring, we can pass an object that contains all the relevant data for the person, like this:

>   const person = {
> 
>     name: "Hou Chia",
> 
>     title: "software engineer",
> 
>     city: "Brooklyn,NY",
> 
>     age: 32,
> 
>   };
> 
>   const introduce = ({ name, title, city, age }) => {
> 
>     return `Hello, my name is ${name}, and I'm a ${title}. I live in ${city}, and I'm ${age} years old.`;
>   
>   };
> 
>   console.log(introduce(person));