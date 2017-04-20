# Atom text editor

-   Download atom here: <https://atom.io>
-   Atom flight manual: <http://flight-manual.atom.io>

## Initial Configuration

### Settings > Core

### Settings > Editior

1.  Set tabs to 4 spaces

### Settings > packages

**Disable all unneeded packages**

Packages that you're not using take extra time to load and make the editor slower.

        $ apm disable autoflow metrics exception-reporting background-tips language-c language-clojure language-csharp language-go language-java language-less language-make language-php language-objective-c language-perl language-python language-ruby language-ruby-on-rails language-toml language-xml status-bar welcome wrap-guide

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

## Useful packages

    $ apm install atom-beautify atom-wrap-in-tag autocomplete-bash-builtins autocomplete-paths busy-signal color-picker docblockr emmet emmet-snippets-compatibility file-icons git-plus goto-definition gulp-snippets highlight-selected html-entitize intentions javascript-snippets linter linter-htmlhint linter-jshint linter-markdown linter-scss-lint linter-ui-default no-title-bar pigments turbo-javascript

-   No Title Bar - `apm install no-title-bar`
-   Wrap in tag - `apm install atom-wrap-in-tag`
-   Color Picker - `apm install color-picker`
-   Pigments - `apm install pigments`
-   Git Plus - `apm install git-plus`
-   File Icons - `apm install file-icons`
-   Beautify - `apm install atom-beautify`
-   Emmet - `apm install emmet`
-   Emmet Snippets Compatibility - `apm install emmet-snippets-compatibility`
-   Docblockr - `apm install docblockr`
-   Highlight Selected - `apm install highlight-selected`
-   HTML Entitize - `apm install html-entitize`
-   Linter - `apm install linter`
-   Linter HTML - `apm install linter-htmlhint`
-   Linter Markdown - `apm install linter-markdown`

## Backing up and restoring configurations

### Backing up

#### Backup package list

    $ apm list --installed --bare > packages.list

#### Back up files in the .atom directory

    .gitignore
    config.cson
    init.coffee
    keymap.cson
    linter-config.json
    package-deps-state.json
    packages.list
    snippets.cson
    styles.less

### Restore from back up

Pull your changes back into the linked atom directory. Then install Atom.

    $ brew cask install atom

## Initial custom keybindings

    '.editor':
      'alt-cmd-w': 'editor:toggle-soft-wrap'
      'alt-cmd-e': 'html-entitize:encode'
      'alt-cmd-d': 'html-entitize:decode'
      'ctrl-1': 'wrap-in-tag:wrap'

## Modifying and customizing atom packages

1.  Create a fork of the package on your repo
2.  go to the `.atom/packages/` directory and run `git clone <package name>` to clone the fork into that folder.
3.  If it's a core package, rename the package in all places in the script
4.  if it's not a core package, disable or uninstall the old one.

## Useful keyboard shortcuts

-   `command + option + w` toggles line wrapping
-   `command + option + e` encodes selected special html characters
-   `command + option + d` decodes selected special html characters

### Packages

`ctrl + shift + m` - Render markdown preview
`cmd + shift + c` - open color picker

### Wrapping two or more lines at once

_This still has some snags, make sure to do it on the first column until it gets fixed_

-   `cmd + shift + l` - selects multiple lines (on selected text), great for wrapping multiple lines at once
-   `ctrl - 1` - wraps the lines in tags
-   `ctrl + shift (up|down)` - click then select multiple lines at once. (_useful for indents_)

### Movement

-   `command + \` - Show/hide treeview
-   `ctrl + shift + L` - change syntax
-   `command + number` - Switch to that tab
-   `a`, `m`, `delete`, `shift + a` - when in treeview to _add, move, delete files, new folder_
-   `cmd + g` - Move to a specific line (and column 30:45)
-   `opt+ up|down` _on a number_ - increments a number higher|lower
-   `opt+command [|]` - folds or unfolds code indentation

### Panes

-   `cmd + k` then `Cmd+Up/Down/Left/Right` - splits a new pane in that direction

### Searching

-   `cmd + t` or `cmd + p` - open fuzzy file finder. _Search the project for file name_
-   `cmd + f` - Search file for text
-   `cmd + shift + f` - search whole project
-   `cmd + b` - search open files

### Bookmarking

-   `cmd + F2` - Bookmark line
-   `F2` - Jump to next Bookmark. _`+Shift` for previous bookmark_
-   `ctrl + f2` - see/ search all bookmarks in file

### Github

-   `Alt+G` `O` - Open file on GitHub
-   `Alt+G` `B` - Open Blame view of file on GitHub
-   `Alt+G` `H` - Open History view of file on GitHub
-   `Alt+G` `C` - Copy the URL of the current file on GitHub to the clipboard
-   `Alt+G` `R` - Branch compare on GitHub
