
# Web Typography

Each different OS has a default set of fonts loaded into it. Fonts rendered in the browser attempt to read these fonts if they are present on the system.

## Fonts in the browser

Fonts in CSS are declared in groups like this:

```
font-family: Helvetica, Arial, "Lucida Grande", sans-serif;
```

Basically this is saying:

1.  Load `Helvetica`
2.  If `Helvetica` is not present/available load `Arial`
3.  If `Arial` is not present try `Lucida Grande`
4.  If none of them are available load the system default sans serif font

There are three types of default fonts. `sans-serif`, `sans`, `mono`

Here's what each of these are:

<https://www.fonts.com/content/learning/fontology/level-1/type-anatomy/serif-vs-sans-for-text-in-print>

There's a safe/ default set of fonts that are generally found across OSs.

These you will use at least as fall backs.

## Loading custom fonts

**Users can decide to deactivate this option, many people do for either privacy or quicker page loading times**. This is why you need a fallback.

### To load a custom font you use `@font-face`

```
@font-face {
	font-family: "Cooper";
	src: url("fonts/Cooper.ttf");
}
```

Once linked into the css file it would be called like this:

```
font-family: Cooper, Helvetica, Arial, "Lucida Grande", sans-serif;
```

Fonts can also be loaded from online hosts like Google Fonts. Bear in mind that if these services are offline the font won't load in your app. However if you call it from a big host like google there's a small change that it will already be cached on the users machine.

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
