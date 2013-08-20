# Carousel

Turn HTML pages into keyboard-navigable slideshows. Designed to be used with [browserify](http://browserify.org/).

## Installation

```
npm install carousel --save
```

## Usage

Create a simple script to use Carousel:

```js
// pre-browserify.js
var Carousel = require('carousel');
new Carousel('#slides');
```

Use browserify to bundle it up for the browser:

```sh
npm install browserify -g
browserify pre-browserify.js -o post-browserify.js
```

Then drop the browserified script into your HTML page and you're good to go.

```html
<script src="post-browserify.js"></script>

<ol id="slides">
  <li>a slide</li>
  <li>another slide</li>
  <li>keep on slidin'</li>
<ol>
```

## Demo

Visit [buildpack-adventure-2.herokuapp.com](http://buildpack-adventure-2.herokuapp.com) for a
working example of Carousel in action, then check out its [source on github](https://github.com/zeke/buildpack-adventure-2#readme).

## Hacking

```
npm install grunt-cli -g
npm install
grunt
```