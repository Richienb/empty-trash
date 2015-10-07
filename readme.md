# empty-trash [![Build Status](https://travis-ci.org/sindresorhus/empty-trash.svg?branch=master)](https://travis-ci.org/sindresorhus/empty-trash)

> Empty the [trash](http://en.wikipedia.org/wiki/Trash_(computing))

Works on OS X, Linux, and Windows.


## CLI

```
$ npm install --global empty-trash
```

```
$ empty-trash --help

  Usage
    $ empty-trash
```


## API

```
$ npm install --save empty-trash
```

```js
const emptyTrash = require('empty-trash');

emptyTrash.then(() => {
	console.log('done');
});
```


## Info

On OS X, AppleScript is used as it's the only way to do it without incurring permission issues.

On Linux, the [XDG spec](http://standards.freedesktop.org/trash-spec/trashspec-1.0.html) is followed.

On Windows, [`recycle-empty-bin`](https://github.com/sindresorhus/empty-recycle-bin) is used.


## Related

See [`trash`](https://github.com/sindresorhus/trash) for moving files/folders to the trash.


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
