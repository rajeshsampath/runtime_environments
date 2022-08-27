# Introduction to Node.js
#### Get an overview of Node.js

> ## We'll cover the following:
> - Node.js overview
>  - What is node.js
>  - Node.js uses the **V8** Javascript engine
>  - Node.js ***versus*** the browser

Welcome to this chapter, By end of this chapter, we'll achieve the following:
  - You'll be able to explain what Node.js and how it's different from browsers.
  - You'll Understand different between blocking and non-blocking patterns in node.js.
  - You'll know how to use the node.js Read-Evaluate-Print-Loop(REPL) environment.
  - You'll know how to use basic node.js debugging tools.


# Node.js overview

Node.js was first released in 2009 by a programmer named **Ryan Dhal**

# What is node.js?

Node.js enables javascript to run outside the browser.

It can be used to build server-side applications that efficiently handle high traffic volumes.

Node.js is portable, means it can be run on various operating systems(***Mac, Windows, Linux and several other systems***) 

# Node.js uses the **V8** javascript engine

A javascript engine is a program that compiles javascript to machine code that the operating system can Understand.

**V8** is the name of the javascript engine it powers the node.js, and it created by Google it is open-source since 2008.

It's written in **C++**


# Node.js ***vs*** The browser

- Before the advent of node.js, javascript could only run in the browser, and its primary was to create browser events interactions.
- Node.js allow us to write javascript in the server to perform common server tasks, such as accessing file system and connecting to databases.


> ### Browser:
>   - The browser has access to **document** and **window** objects.
>   - The **global** object references the **window**.
>   - The browser uses ECMAScripts modules(***import*** and ***export***).
> ### Node.js:
>   - Node.js has access to **http** and **fs** objects.
>   - The **global** object references Node.js specific modules.
>   - Node.js uses the CommonJS module system( ***require()*** and ***module.exports***).

