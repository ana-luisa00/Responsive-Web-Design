In real world code bases you would usually rely on icon libraries so you don't need to generate your svg elements from scratch

```
<svg viewBox="0 0 50 50">
</svg>
```
- viewbox: controls what part of the image is visible inside the svg
- the first two numbers set the starting position of the viewbox (top left corner is 0,0)
- the next two numbers define the width and height