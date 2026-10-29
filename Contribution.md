# Team Members

 | Name | GitHub | Role | Contributions |
|------|--------|------|---------------|
| justinpk561-cyber(Lead)|  [justinpk561-cyber](https://github.com/justinpk561-cyber) | Team Lead | HTTPS|
| Quantums-meruit |[Quantums-meruit](Https://github.com/Quantums-meruit/) | member | DOM |
|username|[username](link) | member| edit |
| gakuruclaire39-cmd | [ gakuruclaire39-cmd](Https://github.com/gakuruclaire39-cmd/)|member| HTML|


# Our Teams Knowledge Base
Welcome, this is our teams repository where we share projects, issues
and projects in order to help each other solve and learn simultaneously

## Justin's Section

### HTTPS

**HTTPS (Hypertext Transfer Protocol Secure)** is a secure version of HTTP used to transfer data between a web browser and a website. It helps protect information exchanged online from being intercepted or altered.

### Why Students Should Use It

- It encrypts data exchanged between a browser and a website.

- It helps protect sensitive information, such as passwords and personal details.
- It verifies a website's identity using a digital certificate.
- It helps prevent attackers from reading or modifying data while it is being transmitted.

### How to Get Started
1. Visit websites using `https://` in their web addresses.
2. Check for the security indicator in your browser's address bar.
3. When developing a website, configure HTTPS using a valid TLS certificate.
4. Avoid entering sensitive information on websites that show security warnings.

### Useful Links
- [HTTPS Explained - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Glossary/HTTPS)
- [Let's Encrypt - Free TLS Certificates](https://letsencrypt.org/)

## Calvin's Section

I am an undergraduate student at *Kenyatta University, while simultaneously expanding my technical capabilities in web development and programming. 

### JavaScript
JavaScript is a high-level, interpreted programming language that adds interactivity, dynamic behavior, and logic to web pages. It runs directly in the browser and forms the core of modern interactive web applications.

### Why Students Should Use It
* It enables dynamic client-side web interactivity and real-time user interface updates.
* It is an essential pillar of web development alongside HTML and CSS.
* It supports modern ES6+ features, asynchronous operations, and API data fetching.
* It expands into full-stack development through environments like Node.js.

### How to Get Started
* Write and test scripts directly inside your browser's Developer Console.
* Embed JavaScript into HTML using `<script>` tags or link external `.js` files.
* Practice coding fundamentals using code editors like VS Code paired with Live Server.
* Build interactive mini-projects like calculators, dynamic forms, and to-do lists.

### Useful Links
* [MDN Web Docs - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [JavaScript.info - The Modern JavaScript Tutorial](https://javascript.info/)


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

## Joseph's section

### [Document Object Model (DOM)](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)

The DOM allows JavaScript to interact with web pages by representing the document as a tree of objects called nodes. It allows us to change the structure, content, and style of a webpage.

### Concepts and Usage

A webpage can be viewed in the browser or as HTML source code. The DOM allows JavaScript to access and modify the webpage.

Example:

```js
const paragraphs = document.querySelectorAll("p");
alert(paragraphs[0].nodeName);
```

This selects all paragraph elements and displays the name of the first one.

### [DOM Tree](https://www.w3schools.com/js/js_htmldom.asp)

When a webpage loads, the browser creates a tree-like representation of its HTML elements.

| Node | Description |
|---|---|
| `<html>` | Element node |
| `<head>` | Element node |
| `<body>` | Element node |
| `<a>` | Element node |
| `href` | Attribute |
| `<h1>` | Element node |
| `My Header` | Text node |

Example:

```html
<body>
    <h1>Hello</h1>
    <p>Welcome</p>
</body>
```

The DOM tree can be represented roughly as:

```text
document
└── body
    ├── h1
    └── p
```

### 1. Document Object

The `document` object represents the webpage and is usually where DOM manipulation begins.

```js
document.querySelector("h1");
```

This selects the first `<h1>` element on the page.

### 2. Selecting Elements

`querySelector()` selects the first element that matches a CSS selector.

```js
document.querySelector("#title");  // ID
document.querySelector(".title");  // Class
document.querySelector("h1");      // Tag
```

**NB:** The selector tells JavaScript what to search for, and the returned value is the actual DOM element.

### 3. `querySelector()` vs `querySelectorAll()`

- `querySelector()` returns the first matching element.
- `querySelectorAll()` returns all matching elements in a NodeList.

```js
const message = document.querySelector(".message");
const messages = document.querySelectorAll(".message");
```

If several elements have the class `message`, the first variable holds only the first match, while the second holds all matches.

### 4. NodeList Indexing

JavaScript indexing starts at `0`, so the first element is at index `0`.

```js
const topics = document.querySelectorAll(".topic");

console.log(topics[0]); // First element
console.log(topics[1]); // Second element
console.log(topics[2]); // Third element
```

**NB:** `topics[1].textContent` accesses the text of the second element.

### 5. `textContent`

`textContent` allows us to read or change the text inside an element.

**Reading text:**

```js
const heading = document.querySelector("h1");
console.log(heading.textContent);
```

**Changing text:**

```js
heading.textContent = "Welcome!";
```

This changes the heading's text on the webpage.

**NB:**

- `heading` refers to the element.
- `heading.textContent` refers to the text inside it.

### 6. `forEach()`

When `querySelectorAll()` returns multiple elements, `forEach()` can loop through them one at a time.

```js
const fruits = document.querySelectorAll(".fruit");

fruits.forEach(function(fruit) {
    console.log(fruit.textContent);
});
```

If there are three matching elements, the callback runs three times.

The parameter name is your choice. For example, `fruit`, `item`, or `element` can all be used.

**NB:** `querySelectorAll()` selects the elements, while `forEach()` iterates through them.

### 7. Reading Attributes

HTML elements can have attributes, such as `href` on a link.

```html
<a href="https://example.com">Visit</a>
```

Use `getAttribute()` to read an attribute's value.

```js
const link = document.querySelector("a");
console.log(link.getAttribute("href"));
```

Output:

```text
https://example.com
```

### 8. Changing Attributes

Use `setAttribute()` to set or change an attribute's value.

```js
link.setAttribute("href", "https://example.com");
```

**NB:**

- `getAttribute()` → reads an attribute.
- `setAttribute()` → sets or changes an attribute.

### 9. `classList`

`classList` allows JavaScript to add, remove, toggle, or check CSS classes on an element.

For more information about DOM manipulation, read the [JavaScript.info article](https://javascript.info/document).


