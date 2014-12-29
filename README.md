# upyun-dispenser
[![NPM version](https://img.shields.io/npm/v/upyun-dispenser.svg?style=flat-square)](https://www.npmjs.org/package/upyun-dispenser)

fast create a ablum with the photos in a dir using upyun

------

## Installation

```bash
$ npm install upyun-dispenser
```

## Usage
```js
dispenser(files, config, callback)
```
__Arguments__

* `files`: files path list to upload
* `config`: config for upyun
    * `bucket`: upyun bucket
    * `operator`: upyun bucket's operator
    * `password`: password of operator
    * `path`: store in which dir
* `callback`: it will come with two arguments
    * first: `err`: for catch error
    * second: `result`: an array contains the urls of the files which uploaded to upyun bucket

## Example
```js
var dispenser = require('upyun-dispenser');

var config = {
    bucket: 'lisposter',
    operator: 'lisposter',
    password: 'test2014',
    path: 'dispenser'
};

var files = [
    './Makefile', 
    './lib/dispenser.js', 
    './LICENSE'
];

dispenser(files, config, function(err, result) {
    console.log(result);
});
```

## License

MIT © [Leigh Zhu](http://zhu.li)
