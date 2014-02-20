*This repository is a mirror of the [component](http://component.io) module [javve/get-attribute](http://github.com/javve/get-attribute). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/javve-get-attribute`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
![web component logo](http://i49.tinypic.com/e7nj9v.png)

# getAttribute

A cross-browser implementation of getAttribute.

Source found here: [http://stackoverflow.com/a/3755343/361337](http://stackoverflow.com/a/3755343/361337)
written by [Vivin Paliath](http://stackoverflow.com/users/263004/vivin-paliath)

Uses default `getAttribute` if it's available.

## Component
Built to be used with the [Component package manager](https://github.com/component/component). Read more here:
* [Component at Github](https://github.com/component/component)
* [TJ Holowaychuk's introduction](http://tjholowaychuk.com/post/27984551477/components)

## Installation

    $ component install javve/get-attribute

## Example

```html
<div id="test" data-value="myValue"></div>
```

```js
var getAttribute = require('get-attribute');

var el = document.getElementById('test')
var dataValue = getAttribute(el, 'data-value');

alert(dataValue); // Alerts "myValue"
```

## API

### getAttribute(element, attribute)

Return the value for `attribute` at `element`.

## License

MIT
