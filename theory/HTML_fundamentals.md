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

# What Are HTML Entities, and What Are Some Common Examples?
An HTML entity, or character reference, is a set of characters used to represent a reserved character in HTML. 

Let's say you wanted to display the text `This is an <img/>` element on the screen. This  it won't display the desired result. Even if you added src and alt attributes to the example, it would show an image in the middle of the paragraph. Not the desired result

When the HTML parser sees the less than (<) symbol followed by an HTML tag name, it interprets that as an HTML element. To fix this issue, you can use HTML entities.
```
<p>This is an &lt;img /&gt; element</p>
```
These types of character references are known as named character references. Named references start with an ampersand sign (&) and end with a semicolon (;). By using a named character reference, the HTML parser will not confuse this with an actual HTML element.

Another type of character reference would be the decimal numeric reference. This character reference starts with an ampersand sign and hash symbol (#), followed by one or more decimal digits, followed by a semicolon.
```
&#60; <!-- less than -->
&#169; <!-- copyright symbol -->
&#174; <!-- trademark symbol -->
```

The last type of character reference would be the hexadecimal numeric reference. This character reference starts with an ampersand sign, hash symbol, and the letter x. Then it is followed by one or more ASCII hex digits and ends with a semicolon.
```
&#x3C; <!-- less than -->
&#x20AC; <!-- euro symbol -->
&#x03A9; <!-- Greek capital letter Omega symbol -->
```

# What Is the Role of the Script Element in HTML, and How Can It Be Used to Link to External JavaScript Files?
The script element is used to embed executable code. Most developers will use this to execute JavaScript code. JavaScript is used to add interactivity to your web pages. Common examples of using JavaScript include interactive games, image sliders, and dynamic forms that validate user input in real-time.
```
<body>
  <script>
    alert("Welcome to freeCodeCamp");
  </script>
</body>
```

While you can technically write all of your JavaScript code inside the script tags, it is considered best practice to link to an external JavaScript file instead.
```
<script src="path-to-javascript-file.js"></script>
```
The src attribute is used here to specify the location for that external JavaScript file. src stands for "source". 

The reason why it is not encouraged to place all of your JavaScript inside the HTML document is because of separation of concerns. Separation of concerns is a design principle where you separate your programs into distinct sections and have each section address a separate concern. In this case, we want to separate our JavaScript code from our HTML code.