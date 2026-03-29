# When Should You Use the Emphasis Element Over the Idiomatic Text Element?
The idiomatic text element, `i`, was originally used for presentational purposes to display the text in italics. But now, it is frequently used for highlighting alternative voice or mood, idiomatic terms from another language, technical terms, and thoughts.
```
<p>There is a certain <i lang="fr">je ne sais quoi</i> in the air.</p>
```
The lang attribute inside the open `<i>` tag is used to specify the language of the content. The `i` element does not indicate if the text is important or not, it only shows that it's somehow different from the surrounding text.

If you do need to emphasize the importance of the text, you can use a similar semantic element called the emphasis element, `em`. This is usually recommended if you need to provide more context. You should use this element for parts of the text that require a special emphasis compared to surrounding text. It's usually limited to only a few words, because it can alter the meaning of the sentence.
```
<p>
  Never give up on <em>your</em> dreams.
</p>
```

It's important to know that these elements should not be used for presentational purposes only. If you need to display the text in italics, but the text doesn't have a special purpose, style, or meaning in the paragraph, you should use CSS instead.

# When Should You Use the Strong Element Over the Bring Attention To Element?
The "bring attention to" element, `b`, is commonly used to highlight keywords in summaries, or product names in reviews. Usually, browsers display this text in boldface.
```
<p>
  We tested several products, including the <b>SuperSound 3000</b> for audio
  quality, the <b>QuickCharge Pro</b> for fast charging, and the
  <b>EcoClean Vacuum</b> for cleaning. The first two performed well, but the
  <b>EcoClean Vacuum</b> did not meet expectations.
</p>
```

If you need to emphasize the importance of the text, you should use the `strong` element instead of the `b` element.

`strong` is a semantic HTML element that emphasizes text that is crucial, or urgent.
```
<p>
  <strong>Warning:</strong> This product may cause allergic reactions.
</p>
```

Visually both are very similar, because they are both rendered as bold by default. But their meanings are quite different. While the "bring attention to" element only draws attention to the text, without indicating the higher level of importance, the `strong` element does more than that. It conveys a sense of importance, or urgency. This is their main difference.

# What Are Description Lists, and When Should You Use Them?
Description lists are perfect for presenting terms and definitions in an organized and easy-to-read format, like in a glossary, or real dictionary, where you can find words with their corresponding definitions.
```
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
  <!-- <dt>JS</dt>
  <dd>JavaScript</dd> -->
</dl>
```
You will need three HTML elements to define a description list. First, the description list element, `dl`, which is the container for the entire list. You can see it wraps around all the other elements of the description list.

Then, one description term element, `dt`, for each term.

And finally, after each term you will find a description details element, `dd`, for the description, or details associated with that term.

In the browser, you would see each term followed by its corresponding description. By default, the descriptions are slightly more indented towards the right to distinguish them visually.

But description lists are not limited to only terms and definitions. They are much more versatile than that.
```
<dl>
  <dt>Flour</dt>
  <dd>2 cups</dd>
  <dt>Sugar</dt>
  <dd>1/2 cup</dd>
  <!-- <dt>Vegetable Oil</dt>
  <dd>2 tablespoons</dd> -->
</dl>
```

Other use cases for description lists include product specifications, frequently asked questions, contact information, and metadata. Essentially, when you have two related pieces of information in a key-value pair format, where one acts as a label, the key, and the other acts as additional related information, the value, you can use a description list.