# npmdoc-usb

#### api documentation for  usb (v1.2.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-usb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-usb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-usb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-usb)

#### Library to access USB devices

[![NPM](https://nodei.co/npm/usb.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/usb)

- [https://npmdoc.github.io/node-npmdoc-usb/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-usb/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-usb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-usb/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-usb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-usb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "usb",
    "description": "Library to access USB devices",
    "version": "1.2.0",
    "engines": {
        "node": ">=0.12.x"
    },
    "keywords": [
        "usb",
        "hardware"
    ],
    "contributors": [
        {
            "name": "Kevin Mehall",
            "url": "http://kevinmehall.net"
        },
        {
            "name": "Tim Ryan",
            "url": "http://timryan.org"
        },
        {
            "name": "Christopher Klein"
        }
    ],
    "main": "./usb",
    "repository": {
        "type": "git",
        "url": "https://github.com/tessel/node-usb.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build",
        "test": "mocha --compilers coffee:coffee-script --grep Module",
        "full-test": "mocha --compilers coffee:coffee-script",
        "valgrind": "coffee -c test/usb.coffee; valgrind --leak-check=full --show-possibly-lost=no node --expose-gc --trace-gc node_modules/mocha/bin/_mocha -R spec"
    },
    "binary": {
        "module_name": "usb_bindings",
        "module_path": "./src/binding",
        "host": "https://github.com/tessel/node-usb/releases/download/",
        "remote_path": "{version}"
    },
    "dependencies": {
        "nan": "^2.4.0",
        "node-pre-gyp": "^0.6.30"
    },
    "bundledDependencies": [
        "node-pre-gyp"
    ],
    "devDependencies": {
        "coffee-script": "~1.6.2",
        "mocha": "~1.8.2",
        "aws-sdk": "~2.0.0-rc.15"
    },
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
