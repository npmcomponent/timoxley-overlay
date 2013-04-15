# Overlay

  Overlays for individual DOM elements.

## Installation

    $ component install timoxley/overlay

## Example

```js

var domify = require('component-domify')
var overlay = require('overlay')
var overlayEl = domify('<div class="overlay"><i class="icon icon-pencil"></i></div>')[0]

var elementSelector = ElementSelector({
  selector: "#container *"
}).on('highlight', function(el) {
  overlay(el, overlayEl).show() // create overlay
}).on('dehighlight', function(el) {
  overlay(el).hide() // hide overlay
})
```

[Demo](http://timoxley.github.com/overlay/examples/overlay/)

## License

  MIT
