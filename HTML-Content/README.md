# HTML Content Formatting

## Atom keyboard shortcuts

-   `command + ~` wraps selected text in html tag (default p)
-   `command + shift + l` selects multiple lines to edit multiple lines
-   `command + option + w` toggles line wrapping
-   `command + option + e` encodes selected special html characters
-   `command + option + d` decodes selected special html characters

## List of tags

The goal of tags is not to make text look a certain way. It's to give the text a greater meaning.

-   `<h1>` - header 1; `h2` `h3` etc
-   `<p>` - paragraph
-   `<br>` - line break, _no closing tag_ make a single line break
-   `<em>` - emphasized text _italics_
-   `<strong>` - stronger than emphasized... it's bold
-   `<pre>` - pre-formatted non-wrapping text
-   `<code>` - computer code
-   `<ul>` - unordered list _list of items with no particular order_
-   `<ol>` - ordered list _for instance a series of steps_
-   `<li>` - a list item _inside of a ul or li tag_
-   `<img src="" alt="">` - _no closing tag_ (attributes - src is the url of the image, alt is alternative text describing the image)
-   `<a href="">` - anchor _aka hyperlink_ (attributes - href is the url)
-   `<abbr title="">` - abbreviation (attributes - title are the expanded words)
-   `<blockquote>` - A passage of quoted text. _text inside is usually wrapped in a p, use `cite` to credit the author_
-   `<cite>` - cite an author in a blockquote. _always inside a blockquote, usually inside a p tag_

## Notes about special characters

-   Characters used in HTML tags must be replaced with special characters. Mainly the greater than and less than symbols.

### Best practice when opening a new text document to make into HTML:

1.  select all text `command + a`
2.  encode all of the characters  `command + option + e`
