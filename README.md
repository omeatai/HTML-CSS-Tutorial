# HTML-CSS-TUTORIAL


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