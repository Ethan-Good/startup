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
Write the HTML needed to create a link, such that when the user clicks the words "my favorite store" they go to https://www.amazon.com: '<a href="https://www.amazon.com">my favorite store</a>'