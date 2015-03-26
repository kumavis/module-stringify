### Module-Stringify

From WebWorkify - https://github.com/substack/webworkify/blob/master/index.js

### Usage

```js
var stringifyModule = require('module-stringify')
var coolModule = require('myCoolModule')

var string = stringifyModule(coolModule)
// use string in webworker or iframe or whatevs
```

Only works b/c of some browserify magic.
If browerify changes, this may break.