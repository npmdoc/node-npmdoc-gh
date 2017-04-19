# npmdoc-gh

#### api documentation for  [gh (v1.12.8)](http://nodegh.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-gh.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gh) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gh.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gh)

#### GitHub command line tools.

[![NPM](https://nodei.co/npm/gh.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gh)

- [https://npmdoc.github.io/node-npmdoc-gh/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gh/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gh/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gh/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gh/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gh/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Eduardo Lundgren",
        "url": "http://eduardo.io"
    },
    "bin": {
        "gh": "bin/gh.js"
    },
    "bugs": {
        "url": "https://github.com/node-gh/gh/issues"
    },
    "contributors": [
        {
            "name": "Zeno Rocha",
            "url": "http://zenorocha.com"
        }
    ],
    "dependencies": {
        "async": "^1.5.0",
        "babel-polyfill": "^6.0.16",
        "colors": "^1.1.2",
        "github": "^0.2.4",
        "handlebars": "^4.0.4",
        "inquirer": "^0.11.0",
        "insight": "^0.7.0",
        "lodash": "^3.10.1",
        "moment": "^2.13.0",
        "nopt": "^3.0.4",
        "open": "^0.0.5",
        "request": "^2.65.0",
        "truncate": "^2.0.0",
        "update-notifier": "^0.5.0",
        "userhome": "^1.0.0",
        "which": "^1.2.0",
        "wordwrap": "^1.0.0"
    },
    "description": "GitHub command line tools.",
    "devDependencies": {
        "babel": "^5.8",
        "gulp": "^3.9.0",
        "gulp-complexity": "^0.3.2",
        "gulp-istanbul": "^0.10.2",
        "gulp-jscs": "^3.0.2",
        "gulp-jshint": "^1.12.0",
        "gulp-mocha": "^2.1.3",
        "jshint-stylish": "^2.0.1",
        "plato": "^1.5.0",
        "rewire": "^2.3.4",
        "run-sequence": "^1.1.4"
    },
    "directories": {},
    "dist": {
        "shasum": "115e64a2748a0fedef57b1a68f1c5175980a86c2",
        "tarball": "https://registry.npmjs.org/gh/-/gh-1.12.8.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "10205cc07abbccc6c18ccf5c976da3a5ac0913f7",
    "homepage": "http://nodegh.io",
    "keywords": [
        "git",
        "github",
        "external",
        "commands",
        "helpers"
    ],
    "license": "BSD-3-Clause",
    "maintainers": [
        {
            "name": "eduardolundgren"
        },
        {
            "name": "zenorocha"
        },
        {
            "name": "henvic"
        }
    ],
    "name": "gh",
    "optionalDependencies": {},
    "preferGlobal": "true",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/node-gh/gh.git"
    },
    "scripts": {
        "ci": "gulp ci",
        "postpublish": "sh postpublish.sh",
        "prepublish": "sh prepublish.sh",
        "test": "gulp test"
    },
    "trackingCode": "UA-58265773-2",
    "version": "1.12.8"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
