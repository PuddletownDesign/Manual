# Atom text editor

*   Download atom here: <https://atom.io>
*   Atom flight manual: <http://flight-manual.atom.io>


## Initial Configuration

### Settings > Core

### Settings > Editior

1.  Set tabs to 4 spaces

### Settings > packages

**Disable all unneeded packages**

Packages that you're not using take extra time to load and make the editor slower.

1.  autoflow
2.  background tips
3.  Language C
4.  Language Clojure
5.  Language cSharp
6.  Language Go
7.  Language Java
8.  Language Less
9.  Language Make
10. Language Objective C
11. Language Perl
12. Language Ruby/Ruby on Rails
13. Language Toml
14. Language XML
15. Welcome
16. Wrap Guide
17. Status bar package

## Initial custom keybindings

```
'.editor':
  'alt-cmd-w': 'editor:toggle-soft-wrap'
  'alt-cmd-e': 'html-entitize:encode'
  'alt-cmd-d': 'html-entitize:decode'
  'cmd-~': 'wrap-in-tag:wrap'
```

## Useful packages

*   No Title Bar - `apm install no-title-bar`
*   Wrap in tag - `apm install atom-wrap-in-tag`
*   Color Picker - `apm install color-picker`
*   Pigments - `apm install pigments`
*   Git Plus - `apm install git-plus`
*   File Icons - `apm install file-icons`
*   Beautify - `apm install atom-beautify`
*   Emmet - `apm install emmet`
*   Emmet Snippets Compatibility - `apm install emmet-snippets-compatibility`
*   Docblockr - `apm install docblockr`
*   Highlight Selected - `apm install highlight-selected`
*   HTML Entitize - `apm install html-entitize`
*   Linter - `apm install linter`
*   Linter HTML - `apm install linter-htmlhint`
*   Linter Markdown - `apm install linter-markdown`

Here's all of them in one command

```
$ apm install no-title-bar atom-wrap-in-tag color-picker pigments emmet emmet-snippets-compatibility docblockr highlight-selected html-entitize linter linter-htmlhint linter-markdown linter-csslint linter-scss-lint
```


## Useful keyboard shortcuts

### Packages

`ctrl + shift + m` - Render markdown preview
`cmd + shift + c` - open color picker

### Wrapping multiple lines

*This still has some snags, make sure to do it only on the first column until it gets fixed*

1.  `cmd + shift + l` - selects multiple lines (on selected text), great for wrapping multiple lines at
2.  `cmd + ~` - wraps the lines in tags
3.  `ctrl + shift (up|down)` - click then select multiple lines at once. (*useful for indents*)

### Movement

*   `command + \` - Show/hide treeview
*   `ctrl + shift + L` - change syntax
*   `command + number` - Switch to that tab
*   `a`, `m`, `delete`, `shift + a` - when in treeview to *add, move, delete files, new folder*
*   `cmd + g` - Move to a specific line (and column 30:45)


### Searching

*   `cmd + t` or `cmd + p` - open fuzzy file finder. *Search the project for file name*
*   `cmd + f` - Search file for text
*   `cmd + shift + f` - search whole project
*   `cmd + b` - search only open files

### Bookmarking

*   `cmd + F2` - Bookmark line
*   `F2` - Jump to next Bookmark. *`+Shift` for previous bookmark*
*   `ctrl + f2` - see/ search all bookmarks in file
