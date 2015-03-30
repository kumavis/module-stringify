### Module-Stringify

From WebWorkify - https://github.com/substack/webworkify/blob/master/index.js

This has side effects, e.g., it doesn't create a minimal bundle.
Also seems slow. You may prefer to create the bundle at build time with [:smile_cat:  meowserify :smile_cat: ](https://github.com/kumavis/meowserify).

### Usage

```js
var stringifyModule = require('module-stringify')
var coolModule = require('myCoolModule')

var string = stringifyModule(coolModule)
// use string in webworker or iframe or whatevs
```

Only works b/c of some browserify magic.
If browerify changes, this may break.
