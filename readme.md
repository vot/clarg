# clarg

The simplest command-line parsing utility for node.js

## Why create another library for this?

All of the existing libraries (i.e. commander or nomnom) require you to specify
upfront what options you expect.

Clarg simply returns you a full set of arguments it found allowing you
to bind everything in any way you want, anywhere you want.


## Usage

Simply import clarg anywhere in your code and it will output an object.
You don't have to specify any options upfront, just require this module
and execute it.
It doesn't matter where in code you run it - you will always get the same result
which is really just a broken down list of arguments and options passed to the process.

```
var clarg = require('clarg');

var arguments = clarg();

// node index.js start --debug --format long
// => {args: ['start'], opts: [{debug: true, format: 'long'}]}
```
