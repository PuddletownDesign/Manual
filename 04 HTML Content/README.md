# HTML Content Formatting

## Atom keyboard shortcuts

* `command + ~` wraps selected text in html tag (default p)
* `command + shift + l` selects multiple lines to edit multiple lines
* `command + option + w` toggles line wrapping
* `command + option + e` encodes selected special html characters
* `command + option + d` decodes selected special html characters


## List of tags

* `h1` - header 1; `h2` `h3` etc
* `p` - paragraph
* `br` - line break, *no closing tag* make a single line break
* `em` - emphasized text *italics*
* `strong` - stronger than emphasized... it's bold
* `pre` - pre-formatted non-wrapping text
* `code` - computer code
* `ul` - unordered list *list of items with no particular order*
* `ol` - ordered list *for instance a series of steps*
* `li` - a list item *inside of a ul or li tag*
* `img [src] [alt]` - *no closing tag* (attributes - src is the url of the image, alt is alternative text describing the image)
* `a [href]` - anchor *aka hyperlink* (attributes - href is the url)
* `abbr [title]` - abbreviation (attributes - title are the expanded words)
* `blockquote` - A passage of quoted text. *text inside is usually wrapped in a p, use `cite` to credit the author*
* `cite` - cite an author in a blockquote. *always inside a blockquote, usually inside a p tag*


## Notes about special characters

* Characters used in HTML tags must be replaced with special characters. Mainly the greater than and less than symbols.

### Best practice when opening a new text document to make into HTML:

1. select all text `command + a`
2. encode all of the characters  `command + option + e`
