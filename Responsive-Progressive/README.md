# Responsive Design & Progressive Enhancement

## Responsive Design

Responsive design is making sure that the app/page responds to the users environment. We're specifically going to first be looking at screen size.


### Mobile First

Begin Developing for the smallest size getting larger as you complete smaller sizes.

### Puddletown Bootstrap

We'll start with using my custom frontend framework.

```
$ git clone https://github.com/PuddletownDesign/puddletown-bootstrap
```

Rename the directory

```
$ mv puddletown-bootstrap new-name
```

Then move into the directory

```
$ cd puddletown-bootstrap
```

Since this is a template we will want our own project history, not the github project history. delete existing git information.

```
$ rm -rf .git
```

Then move into the src directory. **This is the directory you will be working out of**

```
cd src

a ./
```
Then install all dependencies

```
$ npm install && bower install
```

Then run gulp

```
$ gulp
```

When you preview your work, preview from the `build/` directory. `http://localhost:8080/build/`

## Progressive Enhancement

Progressive enhancement is about making sure that advanced interface features have fallbacks or do not fuck up the usability.

### Browser degradation

Browsers (software) get older when newer versions get released. Newer versions often have newer features supported that you may want to use.

Progressive enhancement is about making sure that:

1.  If the newer features aren't supported to have a fallback option.

2.  If there is no fallback option that it won't degrade the usability.

3.  If no option is available opt for the simplest solution.

### Primative First

You set the oldest supported environments. Build for these environments first. Then add on features on top of them for more modern versions.
