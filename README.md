# HTML-CSS-TUTORIAL

## Tutorial

---

### [1-REACT-SCRIMBA](#)

---

+REACT INFO SITE

<details>
  <summary>1. Introduction with CDNs</summary>

REACT DOCS:

```Javascript
https://reactjs.org/docs/cdn-links.html
```

React and ReactDOM are available over a CDN:

DEVELOPMENT:

```Javascript
<script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
```

PRODUCTION:

```Javascript
<script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
```

BABEL:

```Javascript
<script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
```

Index.html:

```Javascript
<html>
    <head>
        <link rel="stylesheet" href="index.css">
        <script crossorigin src="https://unpkg.com/react@17/umd/react.development.js"></script>
        <script crossorigin src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"></script>
        <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    </head>
    <body>
        <div id="root"></div>
        <script src="index.js" type="text/babel"></script>
    </body>
</html>
```

Index.js:

```Javascript
ReactDOM.render(<h1>Hello, everyone!</h1>, document.getElementById("root"))
```

```Javascript
ReactDOM.render(
    <ul><li>Thing 1</li><li>Thing 2</li></ul>,
    document.getElementById("root")
)
```

Imperative expression:

```Javascript
const h1 = document.createElement("h1")
h1.textContent = "This is an imperative way to program"
h1.className = "header"
document.getElementById("root").append(h1)
```

Declarative expression:

```Javascript
ReactDOM.render(<h1 className="header">Hello, React!</h1>, document.getElementById("root"))
```

</details>

<details>
  <summary>2. Creating Custom JSX Functions in React</summary>

Index.js:

```Javascript
import React from "react"
import ReactDOM from "react-dom"

const page = (
    <div>
        <h1 className="header">This is JSX</h1>
        <p>This is a paragraph</p>
    </div>
)

ReactDOM.render(
    page,
    document.getElementById("root")
)
```

```Javascript
import React from "react"
import ReactDOM from "react-dom"

const navbar = (
    <nav>
        <h1>Bob's Bistro</h1>
        <ul>
            <li>Menu</li>
            <li>About</li>
            <li>Contact</li>
        </ul>
    </nav>
)

ReactDOM.render(navbar, document.getElementById("root"))
```

</details>

<details>
  <summary>3. Create Root for React 18</summary>

```Javascript
import React from "react"
import ReactDOM from "react-dom/client"

const navbar = (
    <nav>
        <h1>Bob's Bistro</h1>
        <ul>
            <li>Menu</li>
            <li>About</li>
            <li>Contact</li>
        </ul>
    </nav>
)

const root = ReactDOM.createRoot(document.getElementById("root"))
root.render(navbar)
```

```Javascript
import React from "react"
import ReactDOM from "react-dom/client"

const page = (
    <div>
        <h1>My awesome website in React</h1>
        <h3>Reasons I love React</h3>
        <ol>
            <li>It's composable</li>
            <li>It's declarative</li>
            <li>It's a hireable skill</li>
            <li>It's actively maintained by skilled people</li>
        </ol>
    </div>
)

const root = ReactDOM.createRoot(document.getElementById("root"))
root.render(page)
```

</details>
