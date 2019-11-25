---
title: How to create React Component 
date: "2019-11-25T17:05:32.169Z"
language: en
---

Components are an essential part of any React application. In this post, we'll be learning how to create a new component. Bething components as bite-size chunks of our application that we can reuse all over our site. Let's pretend we're making a simple blog and want to put a button below each post. We could write the code for this button in each area we want it, but this is a hassle if we show it in different locations and need to change it, for some reason. By creating a unique component for this, we can write the actual code once and just include it wherever we want.

## Creating a class component

In order to create a class component, we will have to name it. In the code below, we will name our class component "Example1". All of our code for the component will go where the comment is. 

`{}`

That was easy! Here, it should be noted that if this is a component in a file of it's own, it will have to be exported. There are two ways to do this. We can either include prefix "export default" before our class instantiation

`{}`

or we can simply put a line right at the end of the class that exports it.

`{}`

## Adding state to a class component

Another benefit to class components is state. State allows us to manage various data within our component. State is one of the big advantages of using React. In order to use state functionality, we need a class component. To get started with state, we need to add a constructor to our class component. You can read more about constructors in JavaScript, but for now it's enough to know that this is required to add state to our components. Very often we see "props" being passed in as an argument for the constructor, so we can use any props being passed into this component. The example code below illustrates this.

`{}`

## Render our JSX with the render method

After the constructor, we can add a render method which is in charge for returning our JSX. 

It should be noted that in React, the render method can only return one direct element. This means that all of the JSX we are writing to create that component must be wrapped in an outer element such as a <div>. The example below illustrates how this is built.

`{}`


## Custom Functions in our component 

Another cool benefit of class components is the ability to write functions for use in our components, with our business logic. It's pretty clear. We can write our functions between the constructor and render methods. We can pass any parameters, if is necessary, just like any JavaScript functions. There is one additional step to make this work, though. Inside the constructor, we need to bind the “this” keyword to our method so it can be used anywhere. 

To do this, just use the code below:

`{}`

## Using a component

First of all, if we have our component in separate file, we will have to import the component into the file where we want to use it. That's pretty simple, do it with this code: 

`{}`

Once the component is imported, we can add it to our JSX using the name we assigned to it in the import, in our case “Example6”. Follow the code pattern bellow to add your component into JSX.

`{}`

## Props

So what if we want to pass data into our component avoiding hard code anything into it? 

This is where props come in. Props are pieces of data that passed into the component instance with whatever name we like so we can access it easily, within that component.

Let's say we want to pass a string into our component. When we assign the prop, 

we need to come up with a name for the prop. This should be something enlightening about what it is. Since this is an example, just use “text” but in real world apps it should be more descriptive. We can do it like this:

`{}`

## Receiving props inside component

So far, we have props being passed into our component, now what? As I said before, when we create our component's constructor, we generally put props into the arguments. That's the way our component receives the props we pass into it. Once there, we can access them in our JSX by using “this.props.NameOfProp” as follows: 

`{}`

## Conclusion

Although these are just the basics, they will get you pretty close in terms of building things in React. Try messing around with things, passing some props into new components or adding state to a component to present data. These are the foundational building blocks of React. Happy coding :)