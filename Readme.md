console-stream
=====

Stream interface around console methods

## install

Install with [component(1)](http://component.io):

```sh
$ component install jwerle/console-stream
```

## api

### ConsoleStream(/*Console|Object*/ console [, /*String*/fn])

* `console` - A `Console` object
* `fn` - The method name to write with (default: log)

## usage

```js
var ConsoleStream = require('console-stream');
var stream = require('through')();
var cstream = ConsoleStream(console);

stream.pipe(cstream);
stream.write('beep');
```

## license

MIT
