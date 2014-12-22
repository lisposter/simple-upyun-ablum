# simple-upyun-ablum
[![NPM version](https://img.shields.io/npm/v/simple-upyun-ablum.svg?style=flat-square)](https://www.npmjs.org/package/simple-upyun-ablum)

fast create a ablum with the photos in a dir using upyun

------

## Installation

```bash
$ npm install simple-upyun-ablum
```

## Usage

```js
var up = require('simple-upyun-ablum');
up('/path/to/images/dir', function(err, res) {
  console.log(res);
});
```

**CLI**

```sh
$ up2ablum /path/to/dir
```


## License

MIT © [Leigh Zhu](#)
