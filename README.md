# ListEasy
## Description
In this project you'll help a task management app made a to-do list interactive using the .submit event to `.appendTo()` new items and `.click` event to `.remove()` items.

## Objective
__ListEasy__ is making a task management app. [Here's what it looks like]("https://s3.amazonaws.com/codecademy-content/projects/2/listeasy/index.html"). A user can add a new item, star items, and remove items.

## Tasks
### 1.
Look at __index.html__:

In `<div class="main">`, there is a `<div class="list">` element containing each list item.

Each list item is made up of a checkbox, a `.glyphicon-star`, the list item text, and a `.glyphicon-remove`.

Under the `.list` div, there is a form element. The form element contains a `<input id="todo">` element for the text box to enter new list items.

Look at __script.js__:

There is a function named `template()` that takes list item text as input and returns HTML for the list item as output. This HTML can then be added to .list div.

In the `main()` function, there is a submit event handler attached to form. When a user types an item into the text box and submits the form, the code inside the submit event handler will run.

### 2.
In __script.js__ inside the submit event handler:

a. Get the value typed into the `<input id="todo">` element, and save it into a variable named `text`.

b. Pass `text` as input into the `template()` function, and save the output into a variable named `html`.

c. Append `html` to the `<div class="list">` element.

d. After appending `html` to the list, clear out the value value of `<input id="todo">`.

### 3.
Under the `submit` event handler, attach a `click` event handler to the `.glyphicon-star` element. When clicked, `toggle` the class active.

So far, we've used the `.click()` method to attach click event handlers to HTML elements. The `.click()` method works for HTML elements that are already on the page. Here we're using the form to dynamically add new HTML elements to the page. The `.click()` method won't work on dynamically added HTML elements. Instead, we need to use the `.on()` method.

### 4.
Under the click event handler, attach another click event handler to the `.glyphicon-remove` element. 
