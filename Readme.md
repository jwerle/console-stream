console-stream
=====

Stream interface around console methods

## install

Install with [component(1)](http://component.io):

```sh
$ component install jwerle/console-stream
```

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
