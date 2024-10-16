# Notes
## GitHub
### Useful Commands
git add "file name"\
git commit -am "update"\
git pull\
git push
## HTML
### Notes for HTML deliverable
name the home page index.html. this is what the web will search for first
The <meta> part used so the user can control the zoom of the website
##### Body
body is the stuff that is showing up\
###### Header
nav is the navigation element\
li is the list item\
use href to access local url's that live in the same directory
hr is a line\
###### main
form is a container for input types\
div is a division\
p is a paragrapgh\
table has a table\
thead is the table head\
###### Footer
## CSS
Adds styles, fonts, sizing and many other styling options to html/
rules are added to elements of html. These rules are applied in cascading order/
3 ways to style: main why is having a link to a css file that has the styling rules
### Rules
#### selector
who the rule applys to in the html. like a paragraph tag "<p>", this would be an element/
##### ID
one thing that has a specific id
##### Class
a group of things in a class
##### list
multiple elements like body,section
##### descendents
sections that are in bodys is the example. this would be written as->   body section
#### declaration
the colon
#### Property
what aspect of the selector is being changed
#### value
what value of the property applied to the selector
### animation
name it, give it a duration, then define key frames using from->to and it will go from the begining to the end in the defined duration. you can define things during the from to by using percent like at 95% do this
### media queries
changing images and things depending on the size of the browser. use @media
### float
staying in a certain place with text
#### padding
amount of room in border i think
first number is left and right, 2nd number is bottom and top
#### margin
spacing between the floating thing and text
### grid
### flex
allows elements to be flexible when the window sizes is changed. This is done on the children of the element. 100vh means it takes up 100% of the viewfinder. a 0 after flex means that element wont flex and will remain the same size. 1 means it will flex and will take up 1 of the total pieces. For example if you had 1 and 3 then 1 would take up 1 fourth and 3 would take up 3 fourths. flex direction can be row or column. section:nth-child(1) would refer to the first section from top to bottom in the given parent.
### frameworks
things people have alreay made that you can use and put into ur css code
### styling
add link to css file styling in html code
## Java Script
for behavior/computation. Java manipulates the DOM/
browsers have an iterpreter usually called v8 that interprets java/
there are Node.js servers on our website that are waiting for code/
We add Java the same ways we added CSS/
use %c to forat using css within Java/
objects in Java are like maps but they are not iterable, use curly braces/
arrays are square braces/
### arrays
| Function | Meaning                                                   | Example                       |
| -------- | --------------------------------------------------------- | ----------------------------- |
| push     | Add an item to the end of the array                       | `a.push(4)`                   |
| pop      | Remove an item from the end of the array                  | `x = a.pop()`                 |
| slice    | Return a sub-array                                        | `a.slice(1,-1)`               |
| sort     | Run a function to sort an array in place                  | `a.sort((a,b) => b-a)`        |
| values   | Creates an iterator for use with a `for of` loop          | `for (i of a.values()) {...}` |
| find     | Find the first item satisfied by a test function          | `a.find(i => i < 2)`          |
| forEach  | Run a function on each array item                         | `a.forEach(console.log)`      |
| reduce   | Run a function to reduce each array item to a single item | `a.reduce((a, c) => a + c)`   |
| map      | Run a function to map an array to a new array             | `a.map(i => i+i)`             |
| filter   | Run a function to remove items                            | `a.filter(i => i%2)`          |
| every    | Run a function to test if all items match                 | `a.every(i => i < 3)`         |
| some     | Run a function to test if any items match                 | `a.some(i => i < 1)`          |

example:

const a = [1, 2, 3];

console.log(a.map((i) => i + i));
// OUTPUT: [2,4,6]
console.log(a.reduce((v1, v2) => v1 + v2));
// OUTPUT: 6
console.log(a.sort((v1, v2) => v2 - v1));
// OUTPUT: [3,2,1]

a.push(4);
console.log(a.length);
// OUTPUT: 4
### DOM
The Document Object Model (DOM) is an object representation of the HTML elements that the browser uses to render the display. The browser also exposes the DOM to external code so that you can write programs that dynamically manipulate the HTML.

The browser provides access to the DOM through a global variable name `document` that points to the root element of the DOM. If you open the browser's debugger console window and type the variable name `document` you will see the DOM for the document the browser is currently rendering.

```html
> document

<html lang="en">
  <body>
    <p>text1 <span>text2</span></p>
    <p>text3</p>
  </body>
</html>
```

```css
p {
  color: red;
}
```

For everything in an HTML document there is a node in the DOM. This includes elements, attributes, text, comments, and whitespace. All of these nodes form a big tree, with the document node at the top.
## Midterm Review Notes
Write the HTML needed to create a link, such that when the user clicks the words "my favorite store" they go to https://www.amazon.com:
`<a href="https://www.amazon.com">my favorite store</a>`

Write the HTML needed to create an image tag, where the image is stored at "/images/picture.png":
`<img src="/images/picture.png" />`

What is the HTML tag for an ordered list?
`<ol>`

What is the HTML tag for a second-level heading?
`<h2>`

What HTML tag do you use to make text italic?
`<em> or <i>`

What HTML tag do you use to make text bold?
`<strong> or <b>`

An HTML document should always be surrounded by an `<html>` tag?
true

What is the CSS property that changes the font size of an element?
`font-size`

What is the CSS property that you can use to make text bold?
font-weight

What is the CSS property that changes the amount of spacing within an element?
padding

What is the CSS property that changes the amount of spacing between elements?
margin

How would you set the style of an element to use centered text instead of left justified? Include complete punctuation:
text-align: center;

How would you set the style of an element to float to the right? Include complete punctuation:
float: right;

How would you set the width of an element to be 100%? Include complete punctuation:
width: 100%;

How would you specify that a set of CSS properties applies to the following div: `<div id="content">`?
#content

How would you specify that a set of CSS properties applies to the following div: `<div class="special">`?
.special

What pseudo-selector would you add to an element to show a style when the mouse is over an element? Include the necessary punctuation.
:hover

Which HTML Tag would you use to create a numbered list?
`<ol><li></li></ol>`

How would you use CSS tochangeall the div elements to have a background color of blue?
`div{
background-color: lightblue;
}`

What is the correct HTML for creating a text hyperlink?
`<a href="https://www.w3schools.com/html/">How to make a link</a>`

How would you display an image with a hyperlink in HTML?
`<a href="default.asp"><img src="smiley.gif"></a>`

What does the height attribute of a div element represent in pixels?
Length in pixels

How would you use CSS to change the font size for the p element with an id of "header"?
#header{
font-size: 250%
}

How would you use JavaScript to select all the p elements with an id of "header" and change their text color to red?
document.getElemetByID("header").style.color = "red";

What would you use in jQuery to select all p elements on the page?
`$("p")`

Create a new element and append it to the ul element:
`$("#btn2").click(function(){`
`$("ol").append("<li>Appended item</li>");`

jQuery code snippet will select `<li class='source'> </li>` element and change the text to 'AP':
`$(".source").text("AP");`

code snippet will select all p elements and remove them?
`$("p").remove();`

Which jQuery code snippet will create a new h1 element with the text 'Breaking news' and prepend it to `<div class='article'>...</div>` element?
`$(".article").append("<h1>Cool</h1>");`

Which jQuery code snippet will select the ul element and add the class "attribution"?
`$("ul").addClass("intro");`

Which jQuery code snippet will select the `<p class="description">..</p>` and remove the class "description":
`$("p").removeClass("description");`

Which jQuery code will create a new li element with the class author and append it to?
`$("ol").append("<li class='intro'>Appended item</li>");`

Which jQuery code snippet will select the a element and change the text to "Read more"?
`$(".source").text("Read More");`
`$("#test").text("Read More");`

Which jQuery code snippet will select the next sibling of the `<p class="description>.. </p> element`?
`$(p.description).next()`

Which jQuery code snippet will select the previous sibling of the ul element and change its text to "Breaking news"?
`$("ul.ENTER_ID_HERE").prev().text("Breaking News");`

What is Exactly is Mixed Content?
HTTPS connection where the we page's source code is pulling in other resources with insecure HTTP protocol. The browser will display a warning sayign that hte page has both HTTPS and HTTP content

What is Cross-origin resource sharing (CORS)?
Mechanism that alllows restricted resources (ex: fonts, images, stylesheets, scripts, videos) to be requested from another domain outside the domain from which the first resrouce was served. Allows more freedom and functionality than purely same-origin requests, but is more secure than simply allowing all cross-origin requests

What does the compiler do in the Angular JS runtime system?
Parses and processes the new markup from the template. AngularJS's HTML compiler allows the developer to teach the browser new HTML syntax. The compiler allows you to attach behavior to any HTML element or attribute and even create new HTML elements or attributes with custom behavior. AngularJS calls these behavior extensions directives. compiler updates/stores the value from input ng- model directives. Replaces {{ x }} with teh evaluated value of the markup

What is two-way data binding?
Whenever the input values change, the value of the expressions are automatically recalculated and the DOM is updated with their values. The automatic synchronization of data between the model and view components lets you treat the model as a single-source-of-truth because the view is a projection of the model at all times

What is dependency injection?
Software design that dealts with how objects and functions get created and how they get a hold of their dependencies. The AngularJS injector subsystem is in charge of creating components, resolving their dependencies, and providing them to other components as requested. You can use it when definining components or when providing run and config blocks for a module

How does scope interact with the controller and view in an Angular application?
Anguar JS provides a scope for the variables accessible to expressions. Controllers expose variables and functionality to expressions and directives. Controlllers are responsible for the element with the directive, and all of the element's children. Angular instantiates teh controller and saves it in teh variable specified in the current scope. The binding is live.

Example of for loop in Javascript:
`var i;`
`for (i = 0; i < cars.length; i++) {text += cars[i] + "<br>";}`

Example of while loop in javascript:
`var i = 0;`
`while (i < 10) {text += "<br>The number is " + i; i++;}`

MouseEvents:\
onClick();\
onMouseOut(); //when the user mouses over, or out of, an HTML object\
onmousedown(), onmouseup(); //part of mouse-click\
dblclick()\
hover()\
mouseenter(); //when mouse enters an element

