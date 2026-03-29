# Comments
Commenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with `<!--`, contains any number of lines of text, and ends with `-->`.
```
<!-- TODO: Remove h1 -->
```

# HTML5
HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

## main element
The main element is used to represent the main content of the body of an HTML document. Content inside the main element should be unique to the document and should not be repeated in other parts of the document.
```
<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>
```

## section element
The section element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document. It is a semantic element that helps with SEO and accessibility.
```
<section>
  <h2>Section Title</h2>
  <p>Section content...</p>
</section>
```

## figure element
The figure element represents self-contained content and will allow you to associate an image with a caption.
```
<figure>
  <img src="image.jpg" alt="A description of the image">
  <figcaption>A cute cat</figcaption>
</figure>
```
A figure caption (figcaption) element is used to add a caption to describe the image contained within the figure element.

## footer element
The footer element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more
```
<footer></footer>
```

## head element
The head element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page.
```
<head></head>
```
### title element
The title element determines what browsers show in the title bar or tab for the page.
```
<head>
    <title>CatPhotoApp</title>
</head>
```

### meta elements
You can set browser behavior by adding meta elements in the head.
```
<meta attribute="value">
```


## html element
The html element is the root element of an HTML page and wraps all content on the page. You can also specify the language of your page by adding the lang attribute to the html element.
```
<html lang="en"></html>
```

## Declaration
All pages should begin with `<!DOCTYPE html>`. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.

`<!DOCTYPE html>` tells browsers that the document is an HTML5 document which is the latest version of HTML.

# Nesting
Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.
```
<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>
```

# Images
You can add images to your website by using the img element. img elements have an opening tag without a closing tag. An element without a closing tag is known as a *void* element.
```
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_secondary.svg">
```
The src attribute in an img element specifies the image's URL (where the image is located).
```
<img src="cat.jpg" alt="A cat">
```
All img elements should have an alt attribute. The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.

# Anchor 
You can link to another page with the anchor (a) element
```
<a href="https://www.freecodecamp.org"></a>
```

A link's text must be placed between the opening and closing tags of an anchor (a) element.
```
<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>
```

To open links in a new tab, you can use the target attribute. The target attribute specifies where to open the linked document. `target="_blank"` opens the linked document in a new tab or window.
```
<a href="https://www.freecodecamp.org" target="_blank">freeCodeCamp</a>
```

Other types of content can also be turned into a link by wrapping it in anchor tags.
```
<a href="example-link">
  <img src="image-link.jpg" alt="A photo of a cat.">
</a>
```

# Lists
## Unordered lists
To create an unordered list of items, you can use the ul element.
```
<ul></ul>
```

## Ordered lists
The code for an ordered list (ol) is similar to an unordered list, but list items in an ordered list are numbered when displayed.
```
<ol></ol>
```

## List elements
The li element is used to create a list item in an ordered or unordered list.
```
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

# Italics
To place emphasis on a specific word or phrase, you can use the em element.
```
Cats <em>love</em> lasagna.
```

# Bold
The strong element is used to indicate that some text is of strong importance or urgent.
```
Cats <strong>hate</strong> other cats.
```