# What Is the Role of the Meta Description, and How Does It Affect SEO?
SEO, or Search Engine Optimization, is a practice that optimizes web pages so they become more visible and rank higher on search engines. One way to improve your site's SEO, is to provide a short description for the web page using the meta element
```
<meta
  name="description"
  content="Discover expert tips and techniques for gardening in small spaces, choosing the right plants, and maintaining a thriving garden."
/>
```
By setting the name attribute to description, it ensures that browsers, search engines, and other web tools correctly interpret this metadata. The content attribute is where you will place your description. It is recommended that you keep your descriptions short and concise. This is because search engines will often truncate the description based on the results page layout.

Even though meta descriptions won't directly affect a site's ranking on search engine, having a strong description could result in more traffic to your website.

# What Is the Role of Open Graph Tags, and How Do They Affect SEO?
The open graph protocol enables you to control how your website's content appears across various social media platforms, such as Facebook, LinkedIn, and many more. By setting these open graph properties, you can entice users to want to click and engage with your content. You can set these properties through a collection of meta elements inside your HTML head section.

The first important OG property to include would be the title. 
```
<meta content="freeCodeCamp.org" property="og:title" />
```
For the property attribute, you will need to specify that it is og:title. The content attribute is where you will write the title you want displayed for social media sites.

The next important OG property would be the type
```
<meta property="og:type" content="website" />
```
The type property is used to represent the type of content being shared on social media. Examples of this content include articles, websites, videos, or music.

The third important OG property would be the image.
```
<meta
  content="https://cdn.freecodecamp.org/platform/universal/fcc_meta_1920X1080-indigo.png"
  property="og:image"
/>
```
All of these images should be high quality with good dimensions and ratios. Most social media platforms will include criteria for image requirements to help you ensure that your content displays well on their site.

The fourth important OG property would be the url.
```
<meta property="og:url" content="https://www.freecodecamp.org" />
```

There are many more OG properties that you can set, like description, audio, video and locale. However, the open graph url, image, type, and title are the most important ones to include.

So how do these open graph properties affect Search Engine Optimization? When your content is shared on social media, well-crafted OG properties can enhance the appearance for your content in users' feeds. This can lead to higher click-through rates which could signal to search engines that your content is relevant and engaging.