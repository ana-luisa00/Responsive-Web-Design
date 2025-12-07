# What are Div Elements and When Should You Use Them?
The `div` element is used as a container to group other elements.
```
<div>
  <p>Example paragraph element.</p>
  <p>Another paragraph</p>
</div>
```

You will mainly use the div element when you want to group HTML elements that will share a set of CSS styles.

Even though the div element is commonly used in real world codebases, you should be careful not to overuse it. There are times when another element would be more appropriate. For example, if you wanted to divide up your content into sections, then the section element would be more appropriate than a div element.
```
<section>
  <h2>Mammals</h2>
  <p>
    Mammals are warm-blooded animals with fur or hair. Most give birth to live
    young.
  </p>
  <ul>
    <li>Lion</li>
    <li>Elephant</li>
    <li>Dolphin</li>
  </ul>
</section>
<section>
  <h2>A h2 heading</h2>
  <p>A paragraph</p>
</section>
```

The section element has semantic meaning over the div element which is not semantic. Semantics are the meaning of words or phrases in a language. In HTML, which is a language, elements have their own semantic meaning too. So, this means if you use a section element, the browser will pick up its semantic meaning and understand to treat this as a section - on desktops, mobiles, you name it.

# What Are IDs and Classes, and When Should You Use Them?
## id
The id attribute adds a unique identifier to an HTML element.
```
<h1 id="title">Movie Review Page</h1>
<h2 id="subtitle">A h2 heading</h2>
```

You can reference the id name of title within your JavaScript or CSS. Here's a CSS example referencing the id of title to change the text color to red.
```
#title {
  color: red;
}
```

The hash symbol (#) in front of title, tells the computer you want to target an id with that value. id names should not be used more than once, and they should always be unique. Another thing to note about id values, is that they cannot have spaces in them. id attribute values should only contain letters, digits, underscores, and dashes.

## class
In contrast to the id attribute, the class attribute value does not need to be unique and can contain spaces.
```
<div class="box"></div>
```

If you wanted to add multiple class names to an element, you can do so by separating the names by a space.
```
<div class="box red-box"></div>
```
```
.box {
  width: 100px;
  height: 100px;
}

.red-box {
  background-color: red;
}
```

## Summary
So, to recap, when should you use an id versus a class? Classes are best used when you want to apply a set of styles to many elements. If you want to target a specific element, it is best to use id because those values need to be unique.