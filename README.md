# Static site template

Files to build a static site with CoffeeScript, Jade, Markdown and
Stylus.


## Files

After changing any of the files listed below, you should run
`npm run build-all` to compile the CSS, HTML and JS files.


### _base.jade

Base template that all Jade templates build from.


### index.jade

Final template to build the page for the current folder.


### script.coffee.md

CoffeeScript that is only run on the current page.

If there are functions that are shared between multiple pages, then they
should be in a file that is included in the parent `_base.jade`.


### style.styl

Same as `script.coffee.md`, this contains styles that are only used on
the current page.


### *.md

All `*.md` files are included in the appropriate place in `index.jade`.

It is easier to write large blocks of text in Markdown that it is in
Jade, but Jade offers more functionality, so it is used as a wrapper.
