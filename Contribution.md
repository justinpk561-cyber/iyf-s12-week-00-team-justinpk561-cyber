# Team Members

 | Name | GitHub | Role | Contributions |
|------|--------|------|---------------|
| username(Lead)|  [username](github link ) | Team Lead | edit|
| Quantums-meruit |[Quantums-meruit](Https://github.com/Quantums-meruit/) | member | DOM |
|username|[username](link) | member| edit |
| gakuruclaire39-cmd | [ gakuruclaire39-cmd](Https://github.com/gakuruclaire39-cmd/)|member| HTML|


# Our Teams Knowledge Base
Welcome, this is our teams repository where we share projects, issues
and conflicts in order to help each other solve and learn simultaneously

## Justin's Section
<!-- my paragraph -->

## Calvin's Section

I am an **undergraduate student studying Real Estate** at *Kenyatta University*, while simultaneously expanding my technical capabilities in web development and programming. 

## Core Focus & Skills
* **Web Development:** HTML5, CSS, JavaScript and github.
* **Real Estate student:** Interested in real estate analytics, property management systems, and building digital tools for the property market.
* **Tools & Workflow:** VS Code, Command Line / Shell, and collaborative GitHub workflows.

> *"Continuous learning and version control are key to building solid, scalable software."*

---


## Grace's Section
I am learning **programming** to explore new ways of thinking, explore how technology works and create information using codes.


## Claire's Section
 
I am learning HTML to build structured web pages. I love creating forms, links, and layouts.

**Skills:** HTML5, Semantic Tags, Forms

### HTML

**HTML** (HyperText Markup Language) is the standard language for creating web pages.

### Why Students Should Learn It
- It is the backbone of all websites.
- Easy to learn for beginners.
- Works with CSS and JavaScript to make sites beautiful and interactive.
- Every web developer must know it.

### Basic Example
```html
<!DOCTYPE html>
<html>
<head>
  <title>My First Page</title>
</head>
<body>
  <h1>Hello World!</h1>
  <p>This is a paragraph.</p>
</body>
</html>
```

### Useful Links
- [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/)
- [HTML Living Standard](https://html.spec.whatwg.org/)
- [Learn HTML - web.dev](https://web.dev/learn/html)
- [HTML Validator](https://validator.w3.org/)

 
## Magdalene's section 

## fidel's section

## Joseph 
### [`Document Object Model`](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)

The  DOM connects web pages to script or programming languages by representing the structure of a document 
DOM represents a document with a logical tree, where by each branch of tree ends in a node , and each node contains objects. DOM methods allow programmatic access to the tree. With them, you can change the document's structure, style, or content.

### Concepts and Usage

A web page is a document that can be either displayed in the browser window or as a `HTML` source. In both cases, the `DOM` allows it to be manipulated. As an object-oriented representation of the web page, it can be modified using a scripting language  like `Javascript`.

For Example:
```
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);
```


### [Dom Tree](https://www.w3schools.com/js/js_htmldom.asp)
When a web page loads, the browser creates a tree-like representation of the HTML document.

Each part of the document are nodes in the tree:


|Node |Description|
|----------|--------------|
|`<html>`|Element Node|
|`<head> `| Element Node|
|`<body>`| Element node|
| `<a>` | Element Node|
| `href` | Attribute node|
| `<h1>` | Element Node |
| `My Header`| Text node |



DOM connects web pages to script or programming languages by representing the structure of a document with logical tree where by each branch of the tree ends in a node and each node contains objects.

Example :

``` HTML
<body>
    <h1>Hello</h1>
    <p>Welcome</p>
</body>

```

The browser represents it roughly as :

```
document
└── body
    ├── h1
    └── p
```

1. **Document Object**
`document ` represents the webpage 

``` JavaScript
`document`
```

DOM manipulation usually starts from `document `

Example:
``` javascript 
document.querySelector("h1");
```

means: 

> find an `<h1>` element in the webpage .


2. `*Selecting Elements *`

 `QuerySelector()`

``` javascript
const heading = document.querySelector(".title");
```

`querySelector()` finds the first element matching the selector

it uses CSS selector syntax.

``` javascript
**ID** 

document.queryselector("#title")


**Class** 

document.queryselector(".title")

**Tag**

document.queryselector("h1")

```

NB: 
>the selector tells js what to search for .
>The returned value is the actual DOM element 


Example 

``` javascript
const heading = document.queryselector(".title")

```


> ``` plain text
> ".title" -->  selector
> heading -> actual element
> heading.textContent -> text inside the element
> ```


3. `querySelector()` vs `querySelectorAll()`

`querySelector()`

- it returns the first matching element.


``` js
const message = document.querySelector(".message");
```


if you have :

```html
<p class="message">One</p>
<p class="message">Two</p>
```

only the first `<p>` is returned 

`querySelectorAll()`

returning all matching elements 

```js
const messages = document.querySelectorAll(".message");
```

This gives a Nodelist containing all matching elements.

4.`NodeList indexing`

In JavaScript indexing begins at [0]

Example:

```js
const topics = document.querySelectorAll(".topic");

console.log(topics[0]);
console.log(topics[1]);
console.log(topics[2]);
```

hence:

``` Plain text
topics[0] → first element
topics[1] → second element
topics[2] → third element
```

>NB:
>index 0 = first element 

thus:

```js 
topics[1].textContent
```

gets the second element's text.


5.`textContent

`textContent` allows one to read or change text inside an element.

Reading

```js 
const heading = document.querySelector("h1");

console.log(heading.textContent);
```

if:

```html
 <h1> Hello</h1>
```

the result is:

```plain text 
Hello
```

**Changing **

```js
heading.textContent = "Welcome!"
```

The text on the webpages changes.

NB ⭐


``` Plain text
heading
       ↓
actual element

heading.textContent
       ↓
text inside the element
```

6.**forEach()**

When `querySelectorAll() ` gives you multiple elements, you can loop through them with `forEach()`

```js
const fruits = document.querySelectorAll(".fruit");

fruits.forEach(function(fruit) {
    console.log(fruit.textContent);
});
```

if there are three fruits, the callback runs three times.

**important distiction**

``` plain text
fruits
  ↓
entire collection

fruit
  ↓
one element at a time
```

the parameter name doesn't have to be `fruit`

All the below are valid:

```js
	fruits.forEach(function(fruit) {
});
```

``` js

fruits.forEach(function(item) {
});
```


```js

fruits.forEach(function(element) {
});
```


the name is your choice 

**NB ⭐**

`forEach()` **doesn't select elements**.

`querySelectorAll()` selects them.

`forEach()` **iterates through the selected elements**.

7. **Reading Attributes**

DOM elements can have HTML atrributes.

Example:

```html
<a href="https://example.com">Visit</a>
```


attributes are read using the below:

``` js

element.getattribute("href")
```

Example:

``` js
const link = document.querySelector("a");

console.log(link.getAttribute("href"));
```

output:

``` plain text

https://example.com
```

`getAttribute()`
>read an attribute.


8. `Changing Attributes`
Dom allows changing attributes with:

```js

element.setAttribute("attribute", "value")
```

Example:

```js
link.SetAttribute("href", "https://example.com")
```


**NB ⭐**

Remember:

```plain text

getAttribute() → read
setAttribute() → change/set
```

9.`classList`

classList lets JavaScript manipulate `CSS` classes.

> [for more of Dom manipulation read the `article` ](https://javascript.info/document)





