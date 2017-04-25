# npmdoc-twit

#### basic api documentation for  [twit (v2.2.5)](https://github.com/ttezel/twit)  [![npm package](https://img.shields.io/npm/v/npmdoc-twit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-twit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-twit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-twit)

#### Twitter API client for node (REST & Streaming)

[![NPM](https://nodei.co/npm/twit.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/twit)

- [https://npmdoc.github.io/node-npmdoc-twit/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-twit/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-twit/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-twit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-twit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-twit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tolga Tezel"
    },
    "bugs": {
        "url": "https://github.com/ttezel/twit/issues"
    },
    "dependencies": {
        "bluebird": "^3.1.5",
        "mime": "^1.3.4",
        "request": "^2.68.0"
    },
    "description": "Twitter API client for node (REST & Streaming)",
    "devDependencies": {
        "async": "0.2.9",
        "colors": "0.6.x",
        "commander": "2.6.0",
        "mocha": "2.1.0",
        "rewire": "2.3.4",
        "sinon": "1.15.4"
    },
    "directories": {},
    "dist": {
        "shasum": "241480bab71731162d2a87b27450e4aa3bb5be5f",
        "tarball": "https://registry.npmjs.org/twit/-/twit-2.2.5.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "fa4d346fd564220e5dc41e8866fad3abb74b6479",
    "homepage": "https://github.com/ttezel/twit",
    "keywords": [
        "twitter",
        "api",
        "rest",
        "stream",
        "streaming",
        "oauth"
    ],
    "license": "MIT",
    "main": "./lib/twitter",
    "maintainers": [
        {
            "name": "ttezel"
        }
    ],
    "name": "twit",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/ttezel/twit.git"
    },
    "scripts": {
        "test": "mocha tests/* -t 70000 -R spec --bail --globals domain,_events,_maxListeners"
    },
    "version": "2.2.5",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
