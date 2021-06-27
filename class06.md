
# JavaScript Object Literal


A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

Object Literal Syntax
Object literals are defined using the following syntax rules:

A colon separates property name[1] from value.
A comma separates each name-value pair from the next.
A comma after the last name-value pair is optional.[2]
If any of the syntax rules are broken, such as a missing comma or colon or curly brace, a JavaScript error will be triggered. Browser error messages are helpful in pointing out the general location of object literal syntax errors, but they will not necessarily be completely accurate in pointing out the nature of the error.

Why and How We Use Object Literals
Several JavaScripts from dyn-web use object literals for setup purposes. Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.

There is one drawback: if you are unfamiliar with the syntax, it can be very easy to introduce errors which cause the code to stop working.

example about it 

![objectsliteral](https://miro.medium.com/max/2880/1*96Uu1IPFGKxqspDd9GUoMA.png)









# DOCUMENT OBJECT MODEL

This example brings together a selection of
the techniques you have seen throughout the
chapter to update the contents of the list.
It has three main aims:
1: Add a new item to the start and end of the list
Adding an item to the start of a list requires the use of a different method
than adding an element to the end of the list.
2: Set a cl ass attribute on all items
This involves looping through each of the <l i >elements and updating
the value of the c 1 ass attribute to coo 1.
3: Add the number of list items to the heading
This involves four steps:


1. Reading the content of the heading
2. Counting the number of <:l i >elements in the page
3. Adding the number of items to the content of the heading
4 . Updating the heading with this new content
DOCUMENT

![object](https://appdividend.com/wp-content/uploads/2019/03/Javascript-Objects-Tutorial-Example-Working-With-Objects-in-JS.png)



