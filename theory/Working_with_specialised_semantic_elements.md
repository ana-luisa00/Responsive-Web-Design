# Mathematical equations and chemical formulas
## Superscript element
The superscript element is used to display a piece of text as a superscript. A superscript is a symbol or letter printed above the normal line of text.
```
<p>2<sup>2</sup> (2 squared) is 4.</p>
```
It is important to note that the superscript element should only be used for typographical reasons. If you want to style a piece of text with a raised baseline, then you should use CSS instead of the superscript element.

## Subscript element
To represent chemical equations inside HTML, you would use the subscript element. This element uses a subscript which displays a lowered baseline using smaller text.
```
<p>CO<sub>2</sub></p>
```
Common use cases for the subscript element include chemical formulas, footnotes, and variable subscripts.

# Computer Code
## Inline code element
The inline code element is used to represent short snippets of code inside text. Common use cases for the code element would be for technical articles and documentation pages.
```
<p>
  To set the text color to blue in CSS, use the following code:
  <code>color: blue;</code>
</p>
```
The browser will apply default styles for content inside of the code element. The default styling is a monospaced font. When it comes to including code examples inside your HTML document, you should use the code element for short inline examples.

## Preformatted text element
The preformatted text element is used to represent preformatted text.
```
<pre>
  <code>
    body {
      color: red;
    }
  </code>
</pre>
```
When using the pre element, you will need to be mindful of spacing because it will display exactly as written inside the HTML document.
If you need to display longer code snippets, then you will need to use the pre and code elements.