# html-demo-element
inserts [prism JS syntax colored](https://prismjs.com/) HTML in demo-element before actual dom

## Sample
The code
```html
<html-demo-element title="Error case">
    <slotted-element src="https://badUrl.heck">
        <p slot="loading" hidden>Loading... ⏳ </p>
        <p slot="error" hidden>Something went wrong. 😭 </p>
    </slotted-element>
</html-demo-element>

<script type="module" src="https://unpkg.com/html-demo-element@1.0.0/html-demo-element.js"></script>
<script type="module" src="https://unpkg.com/slotted-element@1.0.0/slotted-element.js"></script>
```

renders following content:
![screenshot](screenshot.png?raw=true "Title")

# Use
Include the script BEFORE inner content is modified. I.e. immediately after HTML and before scripts with components.

# Live demo
https://unpkg.com/slotted-element@1.0.0/demo/index.html
