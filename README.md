# Quiz #2

## Instructions

1. Fork this repo
2. Clone your fork
3. Fill in your answers by writing in the appropriate area, or placing an 'x' in
the square brackets (for multiple-choice questions).
4. Add/Commit/Push your changes to Github.
5. Open a pull request.

## CSS

### Question #1

Describe the purpose of a clearfix in CSS, and give an example of how to do it.

Your Answer:
```
clearfix is used to allow the parent container to naturally fit to the elements within that are floated. Without clearfix, the parent container will collapse if/when elements within are floated.

To implement clearfix, we do the following:

Give the parent container a classname "clearfix" in the html file.
In the style.css file,

.clearfix:before,
.clearfix:after {
  content: " ";
  display: block;
}

.clearfix:after {
  clear: both;
}

After this you can float the elements within the container and it won't collapse.
```

### Question #2

What does the following selector do?  `ul.dropdown > li`?

Select 1:
```
Note: 'ul.dropdown > li' as a selector shows me error. But '.dropdown > li' works. It selects all li's that are directly inside ul's with class dropdown.

[x] Selects all li's which are directly inside a ul of class dropdown (children)
[] Selects all li's which are anywhere inside a ul of class dropdown (any descendant)
[] Selects all ul's of class dropdown, as well as the children elements that are li's
[] Selects all ul's of class dropdown, only if their children are exclusively li's
```

## Scope/Context/Closures

### Question #3

Describe the rules of scope in JavaScript.

Your Answer:
To know the scope a variable in JS is to know where a variable can be referenced or used. A variable has a local scope when it is defined inside a function with the keyword 'var', and it is global in scope if it is define outside a function or anywhere without the keyword 'var'. Scope is important because it allows us to know where a particular variable can be used or referenced.```

```


### Question #4

Define an object and store it in a variable `pizza`. The object should have 2
properties: a temperature (set to 70), and a method called `bake`. When called,
this method should set the pizza's temperature to be 300. Note: you may not use
the variable pizza inside your method.

Your Answer:
```js

var pizza = {
temperature: 70,
bake: function (){
  this.temperature = 300;
};
}

Or

var pizza = {
temperature: 70,
bake: function () {
  pizza.temperature = 300;
};
}

```

## Callbacks

### Question #5

**Define a function called `doSomething`. It should take one argument, called
`thingToDo`. When called, thing to do should invoke the function given as an
argument. Finally, demonstrate calling `doSomething` with a function.**

Your Answer:
```js
The language is quite confusing; I've a hard time understanding the main concept. As for my understanding goes, argument(s) for a function goes inside (); and then included inside the function like we've been doing with examples like: function doSomething( num1, num2) {
num1*num2;
}

//But in this particular question, I'd assume it goes as follows

function doSomething (thingToDo) {
thingToDo;
}

But this will return argument unchanged.
Can you please help walk me through this?
```

### Question #6

**What is the difference between synchronous and asynchronous program execution?**

Select all that apply:
```
[] Synchronous code runs at an even pace, asynchronous code runs with uneven pacing.
[] Synchronous code runs all at the same time, asynchronous code runs completely randomly
[x] Synchronous code runs in order (as appears in the source), asynchronous code may run at a later time.
```

## Git

### Question #7

Which of the following represents a correct workflow for submitting a PR on a non-master branch?
(ignore the lack of commit messages)

Select 1:
```
[x] fork on github; git clone <fork_url>; git checkout -b <charlie_solution>; git add <files>; git commit; git push; create pull request
[] fork on github; git clone <ga_dc_url>; git checkout -b <charlie_solution>; git add <files>; git commit; git push; create pull request
[] git clone <ga_dc_url>; git branch <charlie_solution>; git add <files>; git commit; git push; create pull request
[] fork on github; git clone <fork_url>; git checkout -b <charlie_solution>; git add <files>; git commit; git pull; create pull request
```

## jQuery

### Question #8

Which of the following statements will work, assuming jQuery is loaded?

Select all that apply:
```
[x] `$(".post").css("background", "peachpuff")`
[] `$(".post").innerHTML`
[] `$(".post").html()`
[] `document.getElementsByClassName("post")[0].innerHTML`
[] `document.getElementsByClassName("post").innerHTML`
```

### Question #9

Using jQuery, add an event listener for clicks on the button with the id
'greeting'. When the event happens, the code should append a paragraph to the
body, that says "hello".

Your Answer:
```js
// After creating a button in HTML with class name greeting, in script.jss file, the code is as follows:

$('.greeting').on("click", function () {
  $('body').append ("<p> hello </p>");
})

```

## Software Development Processes

### Question #10

Create a repo for project 1. (You don't need to fork, just create a brand new repo).

Create a readme.md in that repo. In the readme, write out five (5) user stories for your first project. Be sure to include a
role, goal, and reason for each.

Finally, link to your repo on github in the space below.

Your Answer:
```
git@github.com:matiamin/mati_Project1.git
```
