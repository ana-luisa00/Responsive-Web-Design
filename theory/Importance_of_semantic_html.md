# Importance of semantic HTML
## Why Should You Care About Semantic HTML?
The semantic meaning of an element refers to what special information that element conveys. The semantic meaning of a `p` element, for example, is a paragraph of text:
```
<p>
  Let me tell you about my fantastic holiday in Paris.
  I saw the impressive Eiffel Tower up close!
</p>
```
Most elements have semantic meaning. The `div` element is one of the very few that does not.

Why is it important:
- using proper semantic HTML will ensure the best experience for users with assistive technology like screen readers
- semantic HTML can improve your search rankings. This is referred to as search engine optimization, or SEO.
-  using correct semantic elements can improve your development experience

## Why is it Important to Have Good Structural Hierarchy?
Using the right hierarchy is important for accessibility. Assistive technologies, like screen readers, rely on the structure of a web page to determine how to parse and announce that web page to the user. Using an `h3` element after an `h1` might cause a screen reader user to believe they have accidentally skipped over important content, due to the lack of an `h2` element.

Proper structure is also important for SEO. Search engines use automation to parse the content of your web page and determine when and where it should show up in results. If your structure is malformed, search engines may not be able to rank you very well in the relevant search results.

Finally, depending on how incorrect your structure is, your HTML may not even be technically valid. When this happens, the web browser has to effectively guess what you meant to do. And what it guesses might not even be what you want at all.

## What Is the Difference Between Presentational and Semantic HTML?
Presentational HTML focuses on the appearance and style of the content. In the early days of HTML, developers would use elements like the `center`, `big`, and `font` elements. But in modern web development you shouldn't use these types of elements, because of their limitations and negative impact on accessibility and maintainability.

Many presentational HTML elements are deprecated, which means that they are outdated and no longer recommended. There are better ways to get the same results. However, it is helpful to know that they exist, so we'll take a look at some examples

### `font` element
The `font` element is a deprecated element used to set the font size and color of the text. 
```
<font size="5" color="blue">This text is blue and large.</font>
```
While this element still works, you should not use it because the font size and color should always be set in CSS, not in HTML.

### `center` element
The `center` element is another deprecated element that is used to center the content horizontally within its container.
```
<center>
  This text is centered.
  <p>HTML is awesome.</p>
</center>

<p>Another example text.</p>
```

### `big` element
This is another deprecated presentational HTML element that makes the enclosed text one level bigger than its surrounding text.
```
<p>
  This text has a normal font size.
  <big>This text is larger.</big>
  Some other text.
</p>
```
Remember that font size should always be set with CSS, so you should not use this element in modern HTML.

### What to use instead of presentational HTML?
Semantic HTML is now the recommended practice. It describes the content of the elements, so it's much easier to read, understand, and maintain.

Search engines can easily understand your website when you use semantic HTML. It's also helpful for accessibility purposes, because screen readers need semantic information to describe what's on the web page.

The semantic elements clearly show their purpose within the HTML structure. There are many different semantic HTML elements. You will definitely find one that fits the needs of your project.