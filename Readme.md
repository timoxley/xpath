# xpath

XPath utilities extracted from [Firebug](http://code.google.com/p/fbug/source/browse/branches/firebug1.6/content/firebug/lib.js#1294).


## Installation

```js
$ component install timoxley/xpath
```

## Example

Given this html:
```html
<html>
<body>
  <div>
  </div>
  <div>
    <ul>
      <li></li>
      <li id="someItem"></li>
    </ul>
  </div>
</body>
</html>
```

Get the xpath of `#someItem`;
```js
var xpath = require('xpath')
xPath.getElementTreeXPath(document.getElementById('someItem'), true) // => "/html[1]/body[1]/div[2]/ul[1]/li[2]"
// Note: boolean second parameter to `getElementTreeXPath` ensures
element indices are stored in the xpath.

```

## API

- getElementXPath
- getElementTreeXPath
- getElementCSSPath
- cssToXPath
- getElementsBySelector
- getElementsByXPath
- getRuleMatchingElements
- getElementCSSSelector

## Credit

[Firebug Team](http://code.google.com/p/fbug/source/browse/branches/firebug1.6/content/firebug/lib.js#1294)
