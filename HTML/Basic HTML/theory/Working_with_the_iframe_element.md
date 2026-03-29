# What are replaced elements, and what are some examples?
## Replaced element
An element whose content is determined by and external resource rather than by CSS itself. You can control the psition, or layout of an element.
*Example:* images, iframe, video elements

### Example of a replaced element: image
The element is replaced with the image. We can control things such as position, but we cannot modify the image itself at the CSS level.
```
<img src="example-img-url" alt="Descriptive text goes here">
```

## The iframe element
Embeds an external site on your web page
### Examples
Embedding a video
```
<iframe width="400" height="200" src="https://www.youtube.com/embed/u43gJJrVa1I?si=BoDW_puFsy8OEr_Z" title="Professional Cloud Architect Certification Course – Pass the Exam! (YouTube video)" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
```

Embedding a map
```
<iframe
  title="Map of the Royal Observatory, Greenwich, London"
  width="300"
  height="200"
  src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&amp;layer=mapnik">
</iframe>
```

## Other replaced elements
The video element and the embed element are two other examples of replaced elements. Moreover, some elements behave as replaced elements under specific circumstances. For example, the input element:
```
<input type="image" alt="Descriptive text goes here" src="example-img-url">
```
When the type attribute is set to image, input behaves as a replaced element. Other types such as text or email are no replaced elements.

# How do you embed videos onto your page using the iframe element?
## The iframe element, in depth
iframe stands for inline frame. This inline element is used to embed other HTML content directly within the HTML page. The content can be a video, a map, another HTML element of even other web pages.
```
<iframe
  width="400"
  height="400"
  src="https://www.youtube.com/embed/PkZNo7MFNFg?si=-UBVIUNM3csdeiWF"
  title="Learn JavaScript - Full Course for Beginners (YouTube video)"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen
></iframe>
```
- src: specified the URL of the page to embed
- width: width of the iframe
- height: height of the iframe
- allowfullscreen: allos to display the iframe in full screen mode
- title: important to specify for accessibility
- allow: list of things the iframe can or can't do, can be separated by semicolons or spaced, both can be used together
    - clipboard-write: allow the embedded page to write items to your clibboard
    - accelereometer: use moiton sensors so it can detect things like device tilt and rotation
    - autoplay: let the video start playing automatically
    - encrypted-media: use encrypted media extensions to protect the video
    - gyroscope: grant access to device's motion and oritentation sensors
    - web-share: allow sharing the iframe content through the device's native share dialogs
- srcdoc: used instead of src when we want to embed direct HTML withing the iframe
- referrerpolicy: determines how much detail you share when your page connects to another page
    - strict-origin-when-cross-origin: shares the full address on the same site, only the site name on other sites, and nothing on insecure sites