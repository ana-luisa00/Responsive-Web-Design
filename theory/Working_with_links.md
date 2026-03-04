# What are the different target attribute types, and how do they work?
```
<a href="https://freecodecamp.org" target="_blank">Visit freeCodeCamp</a>
```
- target: where to open the URL for the anchor element
    - _self: default value, opens the link in the current browsing context (current tab or window)
    - _blank: opens the link in a new browsing context (new tab or window)
    - _parent: opens the link in the parent of the current context. For example, an iframe with a website would open a link in the current website tab or window
    - _top: open the link in the top-most browsing context, like the parent of the parent
    - _unfencedTop: used for the experimental FencedFrame API

# What is the difference between absolute and relative paths
## Paths
A string that specifies the location of a file or directory in a file system. Paths let developers link to resources like images, stylesheets, scripts and other web pages.
### Absolute path
Complete link to a resource, starting from the root directory and including every other directory concluding with the filename and extension. The root directory refers to the top level directory or folder in a hierarchy. If linking to a resource on your local machine, use an absolute path.
```
<p>
  Read more on the
  <a
    href="/Users/user/Desktop/fCC/script-code/absolute-vs-relative-paths/pages/about.html"
    >About Page</a
    >
</p>
```
### Absolute URL
Complete address used to access a resource. Include the protocol (http, https, file) and the domain name if the resource is on the web.
*Web resource*
```
<a href="https://design-style-guide.freecodecamp.org/img/fcc_secondary_small.svg">
  View fCC Logo
</a>
```
*Local file*
```
file:///Users/user/Desktop/fCC/script-code/absolute-vs-relative-paths/pages/about.html
```
### Relative path
Specifies the location of a file relative to the directory of the current file. It does not include the protocol or the domain name, making it shorter and more flexible for internal links within the same website.
```
<p>
  Read more on the
  <a href="about.html">About Page</a>
</p>
```
## How and when to use relative vs absolute paths
*Absolute paths*
- when you want to reference a resource from a fixed location, such as from the root of your site or a known directory on your local machine

*Absolute URL*
- when linking to a resource hosted on an external website

*Relative paths*
- when linking to resources within the same website
- if you want to keep your code cleaner and easier to maintain during development
- during local testing to ensure links work without an internet connection

# What Is the Difference Between Slashes, a Single Dot, and Double Dot in Path Syntax?
## /\ - the slash
Path separator used to indicate a break in the text between folder or file names
## . - single dot
Points to the current directory. Usually seen to ensure that the path is recognised as a relative pat
## .. - fouble dots
Points to the parent directory. Used to access files outside of the current working directory

# What Are the Different Link States, and Why Are They Important?
```
<body>
    <a href="https://freecodecamp.org" target="_blank">Visit freeCodeCamp</a>
</body>
```
```
a:visited {
  color: brown;
}
```
- :link : default state, represents a link that the user has not visited, clicked or interacted with yet
- :visited : when a user has already visited the page being linked to. By default, it turns purple, but this can be changed with CSS
- :hover : when a user is hovering their cursor over the link
- :focus : applies when we focus on the link
- :active : applies to links that are being activated by the user

There is a specific order in which you need to write your CSS to style links: link, visited, hover, focus, active.