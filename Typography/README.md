
# Web Typography

Each different OS has a default set of fonts loaded into it. Fonts rendered in the browser attempt to read these fonts if they are present on the system.

![Typography](http://tinyimg.io/i/N9ez94m.jpg)

## Fonts in the browser

Declared fonts in CSS in groups like this:

```
font-family: Helvetica, Arial, "Lucida Grande", sans-serif;
```

Basically this is saying:

1.  Load `Helvetica`
2.  If `Helvetica` is not present/available load `Arial`
3.  If `Arial` is not present try `Lucida Grande`
4.  If none of them are available load the system default sans serif font

Three types of default fonts. `sans-serif`, `sans`, `mono`

Here's what each of these are:

<https://www.fonts.com/content/learning/fontology/level-1/type-anatomy/serif-vs-sans-for-text-in-print>

There's a safe/ default set of fonts that are generally found across OSs.

These you will use at least as fall backs.

## Common default font set combinations (Safe Fall backs)

### Sans
```
Helvetica, Arial, "Lucida Grande", sans-serif
"Helvetica Neue", Helvetica, Arial, sans-serif
Optima, Segoe, "Segoe UI", Candara, Calibri, Arial, sans-serif
Futura, "Trebuchet MS", Arial, sans-serif
"Gill Sans", "Gill Sans MT", Calibri, sans-serif
Tahoma, Geneva, Verdana, sans-serif
"Trebuchet MS", "Lucida Grande", "Lucida Sans Unicode", "Lucida Sans", Tahoma, sans-serif
Verdana, Geneva, sans-serif
"Lucida Grande", "Lucida Sans Unicode", "Lucida Sans", Geneva, Verdana, sans-serif
Geneva, Tahoma, Verdana, sans-serif
Segoe, "Segoe UI", "Helvetica Neue", Arial, sans-serif
Candara, Calibri, Segoe, "Segoe UI", Optima, Arial, sans-serif
Calibri, Candara, Segoe, "Segoe UI", Optima, Arial, sans-serif
"Franklin Gothic Medium", Arial, sans-serif
```

### Serif

```
Georgia, "Times New Roman", Times, serif
Garamond, Baskerville, "Baskerville Old Face", "Hoefler Text", "Times New Roman", serif
"Lucida Bright", Georgia, serif
Palatino, "Palatino Linotype", "Palatino LT STD", "Book Antiqua", Georgia, serif
Didot, "Didot LT STD", "Hoefler Text", Garamond, "Times New Roman", serif
Baskerville, "Baskerville old face", "Hoefler Text", Garamond, "Times New Roman", serif
"Hoefler Text", "Baskerville old face", Garamond, "Times New Roman", serif
"Bodoni MT", Didot, "Didot LT STD", "Hoefler Text", Garamond, "Times New Roman", serif
"Goudy Old Style", Garamond, "Big Caslon", "Times New Roman", serif
Constantia, Palatino, "Palatino Linotype", "Palatino LT STD", Georgia, serif
Cambria, Georgia, serif
"Book Antiqua", Palatino, "Palatino Linotype", "Palatino LT STD", Georgia, serif

```

# Monospace

```
"Andale Mono", Courier, monospace
```

## Adding these fonts into atom

*Add the following to your `snippets.cson` file*

```
## CSS Snippets

'.source.css':
  'Helvetica':
    'prefix': 'ffshelvetia'
    'body': 'Helvetica, Arial, "Lucida Grande", sans-serif'
  'Helvetica Neue':
    'prefix': 'ffsHelvetica-Neue'
    'body': '"Helvetica Neue", Helvetica, Arial, sans-serif'
  'Optima':
    'prefix': 'ffsOptima'
    'body': 'Optima, Segoe, "Segoe UI", Candara, Calibri, Arial, sans-serif'
  'Futura':
    'prefix': 'ffsFutura'
    'body': 'Futura, "Trebuchet MS", Arial, sans-serif'
  'Gill Sans':
    'prefix': 'ffsGillsans'
    'body': '"Gill Sans", "Gill Sans MT", Calibri, sans-serif'
  'Tahoma, Geneva, Verdana, sans-serif':
    'prefix': 'ffsTahoma'
    'body': 'Tahoma, Geneva, Verdana, sans-serif'
  'Trebuchet':
    'prefix': 'ffsTrebuchet'
    'body': '"Trebuchet MS", "Lucida Grande", "Lucida Sans Unicode", "Lucida Sans", Tahoma, sans-serif'
  'Verdana':
    'prefix': 'ffsVerdana'
    'body': 'Verdana, Geneva, sans-serif'
  'Lucida':
    'prefix': 'ffsLucida'
    'body': '"Lucida Grande", "Lucida Sans Unicode", "Lucida Sans", Geneva, Verdana, sans-serif'
  'Geneva':
    'prefix': 'ffsGeneva'
    'body': 'Geneva, Tahoma, Verdana, sans-serif'
  'Segoe':
    'prefix': 'ffsSegoe'
    'body': 'Segoe, "Segoe UI", "Helvetica Neue", Arial, sans-serif'
  'Candara':
    'prefix': 'ffsCandara'
    'body': 'Candara, Calibri, Segoe, "Segoe UI", Optima, Arial, sans-serif'
  'Calibri':
    'prefix': 'ffsCalibri'
    'body': 'Calibri, Candara, Segoe, "Segoe UI", Optima, Arial, sans-serif'
  'Franklin Gothic Medium':
    'prefix': 'ffsFranklin'
    'body': '"Franklin Gothic Medium", Arial, sans-serif'
  'Georgia':
    'prefix': 'ffsGeorgia'
    'body': 'Georgia, "Times New Roman", Times, serif'
  'Garamond':
    'prefix': 'ffsGaramond'
    'body': 'Garamond, Baskerville, "Baskerville Old Face", "Hoefler Text", "Times New Roman", serif'
  'Lucida Bright':
    'prefix': 'ffsLucidaBright'
    'body': '"Lucida Bright", Georgia, serif'
  'Palatino':
    'prefix': 'ffsPalatino'
    'body': 'Palatino, "Palatino Linotype", "Palatino LT STD", "Book Antiqua", Georgia, serif'
  'Didot':
    'prefix': 'ffsDidot'
    'body': 'Didot, "Didot LT STD", "Hoefler Text", Garamond, "Times New Roman", serif'
  'Baskerville':
    'prefix': 'ffsBaskerville'
    'body': 'Baskerville, "Baskerville old face", "Hoefler Text", Garamond, "Times New Roman", serif'
  'Hoefler':
    'prefix': 'ffsHoefler'
    'body': '"Hoefler Text", "Baskerville old face", Garamond, "Times New Roman", serif'
  'Bodoni':
    'prefix': 'ffsBodoni'
    'body': '"Bodoni MT", Didot, "Didot LT STD", "Hoefler Text", Garamond, "Times New Roman", serif'
  'Goudy':
    'prefix': 'ffsGoudy'
    'body': '"Goudy Old Style", Garamond, "Big Caslon", "Times New Roman", serif'
  'Constantia':
    'prefix': 'ffsConstantia'
    'body': 'Constantia, Palatino, "Palatino Linotype", "Palatino LT STD", Georgia, serif'
  'Cambria':
    'prefix': 'ffsCambria'
    'body': 'Cambria, Georgia, serif'
  'Book Antiqua':
    'prefix': 'ffsBookAntiqua'
    'body': '"Book Antiqua", Palatino, "Palatino Linotype", "Palatino LT STD", Georgia, serif'
  'Mono':
    'prefix': 'ffsMono'
    'body': '"Andale Mono", Courier, monospace'
```

## Loading custom fonts

**Users can decide to deactivate this option, people do for either privacy or quicker page loading times**. This is why you need a fallback.

### To load a custom font you use `@font-face`

```
@font-face {
	font-family: "Cooper";
	src: url("fonts/Cooper.ttf");
}
```

Once linked into the css file and called like this:

```
font-family: Cooper, Helvetica, Arial, "Lucida Grande", sans-serif;
```

Fonts also loaded from online hosts like Google Fonts. Bear in mind that if these services are offline the font won't load in your app. If you call it from a big host like google there's a small chance that it will  cached on the users machine.

## Google Fonts

The mega resource of free license fonts online.

<https://fonts.google.com>

### Making sense of google fonts and learning about pairings

*   <https://femmebot.github.io/google-type/>
*   <http://fontpair.co>


### Best practices with typography

Think of fonts generally in two ways.

1.  As a heading font. *You can take more liberties here*
2.  As a body text font. *If it's anything more than a headline, it has to be a tried and true body font, easily readable at small or medium sizes.*

**Web fonts are heavy in size. It's a bad idea to load more than 2 max onto a page. 1 is great. 0 remote fonts is best**

*(Generally) Never use more than 3 fonts total on a page. It's tacky*

## Helpful resources on learning typography

*   <https://blog.hubspot.com/marketing/typography-terms-introduction>
