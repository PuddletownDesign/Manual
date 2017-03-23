# Responsive Design & Progressive Enhancement

## Responsive Design

Responsive design is making sure that the app/page responds to the users environment. We're specifically going to first be looking at screen size.


### Mobile First

Begin Developing for the smallest size

### Example CSS

```
// these are the basic styles that will apply to all elements through all screen sizes

h1 {
	color: blue;
}


```


## Progressive Enhancement

Progressive enhancement is about making sure that advanced interface features

### Browser degradation

Browsers (software) get older when newer versions get released. Newer versions often have newer features supported that you may want to use.

Progressive enhancement is about making sure that:

### Primative First

You set the oldest supported environments. Build for these environments first. Then add on features on top of them for more modern versions.

1.  If the newer features aren't supported to have a fallback option.

2.  If there is no fallback option that it won't degrade the usability.

3.  If no option is available opt for the simplest solution.
