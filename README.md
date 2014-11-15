Flex Starter
============

**WORK IN PROGRESS**

Starter-theme and boilerplate for static site generation

[Demo of generated site](http://atelierbram.github.io/flex-starter/)

This repository is build on top of [build-boilerplate](https://github.com/atelierbram/build-boilerplate) which in turn is a fork of [static-site-boilerplate](https://github.com/bdadam/static-site-boilerplate) by Adam Beres-Deak, with some modifications:

- Sass instead of Less
- different Javascript workflow
- adapted Gruntfile.js file

## Extended boilerplate
When a boilerplate is further extended with, let’s say pre-processor modules (Sass), and the generation of `gh-pages`, then it may still be usefull, but the scope will be more limiting. And it’s not a boilerplate anymore, but more an opinionated starter-theme; so that is what this is. When one likes _parts_ of this thing, but _other parts_ not so much, then maybe have [build-boilerplate](https://github.com/atelierbram/build-boilerplate) and this thing side by side, pick and choose, assemble your own starter-theme: make your own Bootstrap.

## How to use this?
1. Clone this repository `git clone https://github.com/atelierbram/flex-starter`
1. Install node dependencies `npm install`
1. Simply run `grunt build` to see that everything works
1. from the commandline run: `grunt gh-pages` to build the remote gh-pages branch

## How to work with this?
You can run `grunt --dev` while developing. This starts a new web server on port 3000 (http://localhost:3000/).
After every change the affected files are regenerated.

## Available Grunt tasks
1. `grunt` - default task: build everything and then whatches for changes and regenerated the affected files
1. `grunt build` - builds everything
1. `grunt clean` - cleanup
1. `grunt assemble` - generates html with Assemble
1. `grunt sass` - generated css file(s) from Sass.scss files
1. `grunt concat` - concatenates JavaScript.js files
1. `grunt uglify` - minifies JavaScript.js files
1. `grunt cssmin` - minifies CSS.css files
1. `grunt hashres` - computes hash code for static resources (aka cachebusting)
1. `grunt connect` - starts web server and stops it automatically when all the other tasks finished
1. `grunt watch` - checks for file modifications and runs the appropriate tasks
1. `grunt gh-pages` - to push to your gh-pages branch hosted on GitHub or any other branch anywhere else

All tasks accept a `--dev` flag, which disables CPU intensive tasks like JS-optimization. This should only be used during development.


## What is included?
1. Static site generation with [Assemble](http://assemble.io/)
1. Generating and minifying a single CSS file with Sass
1. Concatanate and minify JavaScript
1. Generating hash (cache buster) for JS and CSS files
1. Automatic regeneration and Liverload during development
1. [grunt-gh-pages](https://github.com/tschaub/grunt-gh-pages) to push to your gh-pages branch hosted on GitHub or any other branch anywhere else

## Resources

- [static-site-boilerplate](https://github.com/bdadam/static-site-boilerplate) by Adam Beres-Deak
- [grunt-assemble-boilerplate](https://github.com/adregan/grunt-assemble-boilerplate)
- [Effeckt.css](https://github.com/h5bp/Effeckt.css)
- [article by Chis Coyier](http://24ways.org/2013/grunt-is-not-weird-and-hard/)


### License

Released under [MIT Licence](http://atelierbram.mit-license.org)
