*This repository is a mirror of the [component](http://component.io) module [auchenberg/slotcount.js](http://github.com/auchenberg/slotcount.js). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/auchenberg-slotcount.js`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
## slotCount.js

### [Demo](http://auchenberg.github.com/slotCount.js)

Simple slot machine-like counter, inspired by Google Plus.

No dependencies. AMD and CJS compatible.

Works in modern browsers. Chrome, Firefox, Safari 6+, IE10+.

## Installation

#### Manually

Adding to your HTML file:

    <script src="/path_to_http_invoke/slotcount.js"></script>

#### with [Bower](http://bower.io)

    bower install slotcount

#### with [Component](https://github.com/component/component)

    component install auchenberg/slotcount.js

## Usage

```javascript
var counter = new slotCount(container, initialCount);

counter.set(newCount);
counter.dispose();
```

## Examples

### Random number every 2000ms

```javascript
var counter = new slotCount(document.querySelector('.counter-box'), 10);

setInterval(function() {
  var random = Math.floor(Math.random() * 50);
  counter.set(random);
}, 2000);
```

## Test

You can test the component implementation of slotCount.js with Mocha in your browser.

Make sure you run ```component build``` and then point your browser locally to ```test/index.html```.

## Credits
slotCount.js is a project by [Kenneth Auchenberg](http://kenneth.io)

## License

    The MIT License (MIT)
