# xpath

XPath utilities extracted from [Firebug](http://code.google.com/p/fbug/source/browse/branches/firebug1.6/content/firebug/lib.js#1294).


## Installation

```js
$ component install timoxley/xpath
```

## Example

```js
var xpath = require('xpath')
xPath.getElementTreeXPath(document.getElementById('someItem')) // => "/html[1]/body[1]/div[2]/ul[1]/li[2]"

```

```html
<html>
<body>
  <div></div>
  <div>
    <ul>
      <li></li>
      <li id="someItem"></li>
    </ul>
  </div>
</body>
</html>
```

## Credit

[Firebug Team](http://code.google.com/p/fbug/source/browse/branches/firebug1.6/content/firebug/lib.js#1294)
