# npmdoc-mongojs

#### basic api documentation for  [mongojs (v2.4.0)](https://github.com/mafintosh/mongojs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mongojs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mongojs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mongojs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mongojs)

#### Easy to use module that implements the mongo api

[![NPM](https://nodei.co/npm/mongojs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mongojs)

- [https://npmdoc.github.io/node-npmdoc-mongojs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mongojs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mongojs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mongojs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mongojs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mongojs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Buus Madsen"
    },
    "bugs": {
        "url": "https://github.com/mafintosh/mongojs/issues"
    },
    "contributors": [
        {
            "name": "Mathias Buus Madsen"
        },
        {
            "name": "Ian Jorgensen"
        },
        {
            "name": "Eduardo Sorribas"
        },
        {
            "name": "Taeho Kim"
        },
        {
            "name": "Forbes Lindesay"
        },
        {
            "name": "Robert S."
        },
        {
            "name": "Srirangan"
        },
        {
            "name": "Erkan Yilmaz"
        },
        {
            "name": "Jake Maskiewicz"
        },
        {
            "name": "Bjarke Walling"
        },
        {
            "name": "Tobias Baunbæk"
        },
        {
            "name": "Benedikt Arnold"
        },
        {
            "name": "Kevin McTigue"
        },
        {
            "name": "Thomas Watson Steen"
        }
    ],
    "coordinates": [
        48.2317966,
        16.3996661
    ],
    "dependencies": {
        "each-series": "^1.0.0",
        "mongodb": "^2.0.45",
        "once": "^1.3.2",
        "parse-mongo-url": "^1.1.0",
        "readable-stream": "^2.0.2",
        "thunky": "^0.1.0",
        "to-mongodb-core": "^2.0.0",
        "xtend": "^4.0.0"
    },
    "description": "Easy to use module that implements the mongo api",
    "devDependencies": {
        "concat-stream": "^1.5.0",
        "geopkg": "^4.0.3",
        "istanbul": "^0.4.1",
        "shelljs": "^0.7.0",
        "standard": "^6.0.8",
        "tap-spec": "^4.1.1",
        "tape": "^4.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "f287fbfd457fedf588b5a9011e68513d9dd32bfb",
        "tarball": "https://registry.npmjs.org/mongojs/-/mongojs-2.4.0.tgz"
    },
    "gitHead": "8e7ae24c3963d706c2b94f1778dcc0fcba2fbc99",
    "homepage": "https://github.com/mafintosh/mongojs#readme",
    "keywords": [
        "mongo",
        "db",
        "mongodb"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "mafintosh"
        },
        {
            "name": "sorribas"
        },
        {
            "name": "watson"
        },
        {
            "name": "saintedlama"
        }
    ],
    "name": "mongojs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/mafintosh/mongojs.git"
    },
    "scripts": {
        "cover": "node --harmony --harmony-proxies node_modules/istanbul/lib/cli.js cover node_modules/tape/bin/tape \"test/test-*.js\" --report html",
        "geotag": "geopkg update",
        "test": "standard && (tape \"test/test-*.js\" && node --harmony --harmony-proxies node_modules/tape/bin/tape \"test/test-*.js\") | tap-spec"
    },
    "version": "2.4.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
