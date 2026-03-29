# Block Inline Quotes
In HTML, quoted elements are used to distinguish quoted text from the surrounding content. This gives the quoted text a format that is easy to identify.

You should use the block quotation element for representing a section quoted from another source. It's mainly used for extended quotations. If the source of the quote has an address, you can cite it with the cite attribute. The value of this attribute should be a valid URL.

```
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  "Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?"
</blockquote>
```

The value of the cite attribute is the URL of the source. While this attribute doesn't change the presentation of the block quote, it's very helpful for giving screen readers and search engines more information about the quote.

```
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  <p>Build your projects. Show them to your friends. Build projects for your friends.</p>
  <p>Build your network. Help the people you meet along the way. What goes around comes around. You'll get what's coming to you.</p>   
  <p>It is not too late. Life is long.</p>
  <p>You will look back on this moment years from now and be glad you made a move.</p>
</blockquote>
```
All the paragraphs are contained within the same block quotation element, so they are part of the same quotation. 

If you want to attribute the source visually, you can add a citation element, `cite`, outside of the block quotation element. This is different from the `cite` attribute. The citation element is an HTML element that you can use to mark up the title of a referenced creative work like a book article, song, film, website, or research paper.
```
<div>
  <blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?
  </blockquote>
  <p>—Quincy Larson, <cite>How to Learn to Code and Get a Developer Job [Full Book].</cite></p>
</div>
```

You should use block quotes like these for long quotations from other sources. But sometimes you will only need to quote a few words within a larger paragraph.

That's exactly what the inline quotation element is for. It's for short inline quotations from other sources. Most modern browsers will add quotation marks around the inline quote automatically when you use this element.

```
<p>
  As Quincy Larson said,
  <q cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Momentum is everything.
  </q>
</p>
```

What's the difference between block quotes and inline quotes? You should use block quotes for extended quotations from other sources and inline quotes for short quotations from other sources that should be part of existing paragraphs.

# Abbreviations
An abbreviation is a shortened form of a word or phrase. 
## Acronyms
An acronym is a word formed from the initial letters of a phrase, with each letter representing the first letter of a word in that phrase.
## Initialisms
An initialism is formed from the initial letters of a phrase, with each letter representing the first letter of a word in that phrase.
## Acronyms vs Initialism
Both acronyms and initialisms are types of abbreviations. The distinction is acronyms are pronounced as words and initialisms are pronounced as individual letters.

## The abbreviation element
```
<p><abbr>HTML</abbr> is the foundation of the web.</p>
```
You should always explain the abbreviation's full meaning when you use them for the first time. Then you can use the abbreviation element to highlight them and provide more details.
The abbreviation element is providing helpful context behind the scenes, but users will still see the initialism as normal text.

```
<p><abbr title="HyperText Markup Language">HTML</abbr> is the foundation of the web.</p>
```
- title: human readable description of the abbreviation

Usually, the style of the abbreviation element will change when you add this attribute. The specific style will depend on the browser. Some browsers may display a dotted underline, while others may convert the contents to small caps. When the user hovers over the abbreviation, the full form is displayed as a tooltip.

# Addresses
```
<address>
  <h2>Company Name</h2>
  <p>
    1234 Elm Street<br />
    Springfield, IL 62701<br />
    United States
  </p>
  <p>Phone: <a href="tel:+15555555555">+1 (555) 555-5555</a></p>
  <p>Email: <a href="mailto:contact@company.com">contact@company.com</a></p>
</address>
```
The contact address element is used to represent contact information for a section on a web page. The address element is versatile and can be used for business pages, author pages, personal sites, and more.

# Times and dates
## Time
The `time` element is used to represent a specific moment in time.
```
<p>The reservations are for <time datetime="20:00">20:00 </time></p>
```

## Datetime
The datetime attribute is used to translate dates and times into a machine-readable format. The value for the datetime attribute must be either a valid year, valid month, valid time, local date, global date, or valid duration string.
```
<p>
  The graduation will be on <time datetime="2024-06-15T15:00">June 15</time>
</p>
```
The value for the datetime attribute is in the ISO 8601 format. ISO 8601 is an international standard to represent dates and times.
