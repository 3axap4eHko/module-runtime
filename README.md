# Module Runtime

Tiny library to create runtime node modules

## Usage

create module
``` javascript
// index.js
const moduleRuntime = require('module-runtime');

moduleRuntime('add', `
module.exports = function(a, b) {
    return a + b;
};
`);

```
use module
``` javascript
const add = require('add');

console.log(add(1,2)); // 3
```

## LICENSE

[The MIT License](http://opensource.org/licenses/MIT)
Copyright (c) 2017-present Ivan Zakharchenko


