# What Role Does HTML Play on the Web?
HTML, which stands for Hypertext Markup Language, is a markup language for creating web pages. When you visit a website and see content like paragraphs, headings, links, images, and videos; that's HTML.

HTML represents the content and structure of a webpage through the use of elements. Most elements will have an opening tag and a closing tag. Sometimes those tags are referred to as start and end tags. In between those two tags, you will have the content. This content can be text or other HTML elements.
```<p>I am a paragraph element.</p>```

Both opening and closing tags start with a left angle bracket (<), and end with a right angle bracket (>), with the tag name placed between these angle brackets. While HTML tag names are case-insensitive, it is a widely accepted convention and best practice to write them in lowercase.

What distinguishes an opening tag from a closing tag is the forward slash (/) placed immediately after the left angle bracket in a closing tag. Some HTML elements do not have a closing tag. These are known as void elements.
Here is an example of an image element which is a void element:
```<img>```
Notice that this image element does not have the closing tag and it does not have any content. Void elements cannot have any content and only have a start tag.

Sometimes you will see void elements that use a / before the > like this:
```<img />```
While many code formatters like Prettier, will choose to include the / in void elements, the HTML spec states that the presence of the / "does not mark the start tag as self-closing but instead is unnecessary and has no effect of any kind".

If you wanted to display an image, you will need to include a couple of attributes inside your image element. An attribute is a special value used to adjust the behavior for an HTML element.
```<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg" />```
The src attribute is used to specify the location for that image. 

For image elements, it's good practice to include another attribute called the alt attribute. The alt attribute is used to provide short, descriptive text for the images.
```<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Two tabby kittens sleeping together on a couch." />```

So, you might be wondering if HTML by itself is enough to build a website. Well, the answer is: it depends. If you're building a small practice project that only displays text and images, HTML alone might be sufficient. However, if you're creating a modern professional website, you will need to have HTML, CSS, and JavaScript.

HTML is for the content and structure. CSS is for styling. JavaScript is for adding interactivity to your web pages. A good analogy for this is to compare HTML, CSS, and JavaScript with a complete building.

HTML represents the blocks, concrete, and irons that make up the walls. It's the foundation that makes the building strong. CSS represents the interior and exterior design that makes the house look beautiful. JavaScript represents the electrical and water system that ensures uninterrupted access to water and electricity.

# What are attribute, and how do they work?
An attribute is a value placed inside the opening tag of an HTML element. Attributes provide additional information about the element or specify how the element should behave. Here is the basic syntax for an attribute:
```<element attribute="value"></element>```

The attribute name is followed by an equal sign (=) and a value in quotes. The value can be a string or a number, depending on the attribute.

```<a href="https://www.freecodecamp.org" target="_blank">Visit freeCodeCamp</a>```
This first example uses the href and target attributes. The href attribute specifies the URL of a link and the target attribute specifies where to open the link. Without the href attribute, the link would not work because there would be no destination URL. So you must include this href attribute to make the link functional.
The target="_blank" enables the link to open in a new browser tab.

```<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Two tabby kittens sleeping together on a couch." />```
Other common attributes are the src, and alt, or alternative, attribute - which is used to specify the source of an image and provide alternative descriptive text for the image, respectively.

Similar to the href attribute, the src attribute is required because it specifies the image file to be displayed. The alt attribute is not required, but it is recommended for accessibility purposes. 
Accessibility means making sure that everyone, including those with disabilities, can use and understand things like websites, apps, and physical spaces.

```<input type="checkbox" checked />```
Some attributes are a little unique with their syntax like the checked attribute. Here we have an input element with the type attribute set to checkbox. Inputs are used to collect data from users, and the type attribute specifies the type of input.

The checked attribute is used to specify that the checkbox should be checked by default. The checked attribute does not require a value. If it is present, the checkbox will be checked by default. If the attribute is not present, the checkbox will be unchecked. This is known as a boolean attribute.

There are several common boolean attributes you will encounter in HTML, such as disabled, readonly, and required. These attributes are used to specify the state of an element, such as whether it is disabled, read-only, or required.

Here is an example of a text input element that is disabled by default
```<input type="text" disabled>```