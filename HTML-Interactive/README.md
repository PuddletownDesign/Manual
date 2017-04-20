# HTML Interactive elements

_also data tables too..._

I suggest reading through this whole article.

<http://learn.shayhowe.com/html-css/getting-to-know-html/>

All of the docs on that site are pretty cool. I recommend following along with various tutorials on building layouts from scratch. If they use any preexisting CSS of JS files I would skip them. Stick with hand written HTML and CSS for now. Trust me.

At this point you need to be getting your tools sharpened. You want to have memorized sets of keyboard shortcuts for writing out and formatting HTML quickly and easily. The index.html file I initially sent you (2-basic-html) would take me roughly 20 seconds.

## Snippets and emmet

Make sure to begin experimenting with emmet at this phase. also start learning to build out snippets for any thing you repeatedly make.

## Forms and Tables best practices

1.  on forms, the label `for` has to have a matching input `id` this ties the two together. The most obvious effect is clicking the label selects the form.
2.  can't put any other markup like h2 or p within the table (unless it's in a cell)
3.  the sloppy looking `br` tags I use on forms are to insure that even without css they are still usable. `input` and `label` elements are inline and will wrap.
4.  tables work as follows. You have a row `tr` and a cell `td` within the row. That structure at the very least must maintain intact.
5.  tables have optional headers `thead` and footers `tfoot` that can be added. The main data goes into the body `tbody`
6.  note the adjustments to the `colspan` and `rowspan` attributes on two of the tables. Just understand that the count of all cells needs to add up to the same in all rows.
7.  Lastly the forms we'll be using more once we get into javascript and then especially into server side stuff. For now it's just important to know how to build them properly and get them to validate.

## Specifications

-   Must have proper doctype and validate (don't worry about warnings)
-   have proper meta tags (with description tags)

## HTML5 Tags you need to know at this point

See reference here:

<http://html5doctor.com/element-index/>

Semantics can be vague and difficult to understand sometimes, cross reference that site with others to understand better while you mke documentation.

When reading through read about them in the groups I've outlined below. It will make a lot more sense.

### Document tags

-   head
    -   meta
    -   link
    -   script
-   body

### layout and document structure

-   article
-   main
-   section
-   aside
-   header
-   footer

### Block level

-   h1-h6
-   p
-   ul
    -   li
    -   ol
    -   blockquote
    -   cite

### inline

-   a
-   abbr
-   em
-   strong
-   img

### Preformatted text and code

-   code
    -   pre

### Misc Formatting

-   br
-   hr

### Non-semantic elements used for positioning (css/js)

-   div
-   span

### Tables

-   table
    -   thead
        -   tr
            -   td
    -   tfoot

### Forms / Interaction

-   form
-   input
    -   text, checkbox, radio
-   textarea
-   select
    -   option
-   button
