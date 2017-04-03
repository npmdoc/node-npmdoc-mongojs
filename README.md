# api documentation for  [mongojs (v2.4.0)](https://github.com/mafintosh/mongojs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mongojs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mongojs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mongojs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mongojs)
#### Easy to use module that implements the mongo api

[![NPM](https://nodei.co/npm/mongojs.png?downloads=true)](https://www.npmjs.com/package/mongojs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mongojs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mongojs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mongojs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mongojs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mongojs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Buus Madsen",
        "email": "mathiasbuus@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/mafintosh/mongojs/issues"
    },
    "contributors": [
        {
            "name": "Mathias Buus Madsen",
            "email": "mathiasbuus@gmail.com"
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
            "name": "Thomas Watson Steen",
            "email": "w@tson.dk"
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
            "name": "mafintosh",
            "email": "mathiasbuus@gmail.com"
        },
        {
            "name": "sorribas",
            "email": "eduardo@sorribas.org"
        },
        {
            "name": "watson",
            "email": "w@tson.dk"
        },
        {
            "name": "saintedlama",
            "email": "christoph.walcher@gmail.com"
        }
    ],
    "name": "mongojs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mafintosh/mongojs.git"
    },
    "scripts": {
        "cover": "node --harmony --harmony-proxies node_modules/istanbul/lib/cli.js cover node_modules/tape/bin/tape \"test/test-*.js\" --report html",
        "geotag": "geopkg update",
        "test": "standard && (tape \"test/test-*.js\" && node --harmony --harmony-proxies node_modules/tape/bin/tape \"test/test-*.js\") | tap-spec"
    },
    "version": "2.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mongojs](#apidoc.module.mongojs)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Binary (buffer, subType)](#apidoc.element.mongojs.Binary)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Code (code, scope)](#apidoc.element.mongojs.Code)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>DBRef (namespace, oid, db)](#apidoc.element.mongojs.DBRef)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Double (value)](#apidoc.element.mongojs.Double)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Long (low, high)](#apidoc.element.mongojs.Long)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>MaxKey ()](#apidoc.element.mongojs.MaxKey)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>MinKey ()](#apidoc.element.mongojs.MinKey)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>NumberLong (low, high)](#apidoc.element.mongojs.NumberLong)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>ObjectID (id)](#apidoc.element.mongojs.ObjectID)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>ObjectId (id)](#apidoc.element.mongojs.ObjectId)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Symbol (value)](#apidoc.element.mongojs.Symbol)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Timestamp (low, high)](#apidoc.element.mongojs.Timestamp)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>bulk (colName, ordered, onserver)](#apidoc.element.mongojs.bulk)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>collection (opts, getConnection)](#apidoc.element.mongojs.collection)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>cursor (getCursor)](#apidoc.element.mongojs.cursor)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>database (connString, cols, options)](#apidoc.element.mongojs.database)
1.  object <span class="apidocSignatureSpan">mongojs.</span>Binary.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>Code.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>DBRef.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>Double.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>Long.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>ObjectID.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>Symbol.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>Timestamp.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>bulk.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>collection.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>cursor.prototype
1.  object <span class="apidocSignatureSpan">mongojs.</span>database.prototype

#### [module mongojs.Binary](#apidoc.module.mongojs.Binary)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Binary (buffer, subType)](#apidoc.element.mongojs.Binary.Binary)
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>BUFFER_SIZE
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_BYTE_ARRAY
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_DEFAULT
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_FUNCTION
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_MD5
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_USER_DEFINED
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_UUID
1.  number <span class="apidocSignatureSpan">mongojs.Binary.</span>SUBTYPE_UUID_OLD

#### [module mongojs.Binary.prototype](#apidoc.module.mongojs.Binary.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>length ()](#apidoc.element.mongojs.Binary.prototype.length)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>put (byte_value)](#apidoc.element.mongojs.Binary.prototype.put)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>read (position, length)](#apidoc.element.mongojs.Binary.prototype.read)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>toJSON ()](#apidoc.element.mongojs.Binary.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>toString (format)](#apidoc.element.mongojs.Binary.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>value (asRaw)](#apidoc.element.mongojs.Binary.prototype.value)
1.  [function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>write (string, offset)](#apidoc.element.mongojs.Binary.prototype.write)

#### [module mongojs.Code](#apidoc.module.mongojs.Code)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Code (code, scope)](#apidoc.element.mongojs.Code.Code)

#### [module mongojs.Code.prototype](#apidoc.module.mongojs.Code.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.Code.prototype.</span>toJSON ()](#apidoc.element.mongojs.Code.prototype.toJSON)

#### [module mongojs.DBRef](#apidoc.module.mongojs.DBRef)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>DBRef (namespace, oid, db)](#apidoc.element.mongojs.DBRef.DBRef)

#### [module mongojs.DBRef.prototype](#apidoc.module.mongojs.DBRef.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.DBRef.prototype.</span>toJSON ()](#apidoc.element.mongojs.DBRef.prototype.toJSON)

#### [module mongojs.Double](#apidoc.module.mongojs.Double)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Double (value)](#apidoc.element.mongojs.Double.Double)

#### [module mongojs.Double.prototype](#apidoc.module.mongojs.Double.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.Double.prototype.</span>toJSON ()](#apidoc.element.mongojs.Double.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongojs.Double.prototype.</span>valueOf ()](#apidoc.element.mongojs.Double.prototype.valueOf)

#### [module mongojs.Long](#apidoc.module.mongojs.Long)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Long (low, high)](#apidoc.element.mongojs.Long.Long)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.</span>fromBits (lowBits, highBits)](#apidoc.element.mongojs.Long.fromBits)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.</span>fromInt (value)](#apidoc.element.mongojs.Long.fromInt)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.</span>fromNumber (value)](#apidoc.element.mongojs.Long.fromNumber)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.</span>fromString (str, opt_radix)](#apidoc.element.mongojs.Long.fromString)
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_16_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_24_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_31_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_32_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_48_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_63_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_64_DBL_
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>INT_CACHE_
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>MAX_VALUE
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>MIN_VALUE
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>NEG_ONE
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>ONE
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>TWO_PWR_24_
1.  object <span class="apidocSignatureSpan">mongojs.Long.</span>ZERO

#### [module mongojs.Long.prototype](#apidoc.module.mongojs.Long.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>add (other)](#apidoc.element.mongojs.Long.prototype.add)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>and (other)](#apidoc.element.mongojs.Long.prototype.and)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>compare (other)](#apidoc.element.mongojs.Long.prototype.compare)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>div (other)](#apidoc.element.mongojs.Long.prototype.div)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>equals (other)](#apidoc.element.mongojs.Long.prototype.equals)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getHighBits ()](#apidoc.element.mongojs.Long.prototype.getHighBits)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getLowBits ()](#apidoc.element.mongojs.Long.prototype.getLowBits)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.mongojs.Long.prototype.getLowBitsUnsigned)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getNumBitsAbs ()](#apidoc.element.mongojs.Long.prototype.getNumBitsAbs)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>greaterThan (other)](#apidoc.element.mongojs.Long.prototype.greaterThan)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.mongojs.Long.prototype.greaterThanOrEqual)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>isNegative ()](#apidoc.element.mongojs.Long.prototype.isNegative)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>isOdd ()](#apidoc.element.mongojs.Long.prototype.isOdd)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>isZero ()](#apidoc.element.mongojs.Long.prototype.isZero)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>lessThan (other)](#apidoc.element.mongojs.Long.prototype.lessThan)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>lessThanOrEqual (other)](#apidoc.element.mongojs.Long.prototype.lessThanOrEqual)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>modulo (other)](#apidoc.element.mongojs.Long.prototype.modulo)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>multiply (other)](#apidoc.element.mongojs.Long.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>negate ()](#apidoc.element.mongojs.Long.prototype.negate)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>not ()](#apidoc.element.mongojs.Long.prototype.not)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>notEquals (other)](#apidoc.element.mongojs.Long.prototype.notEquals)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>or (other)](#apidoc.element.mongojs.Long.prototype.or)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>shiftLeft (numBits)](#apidoc.element.mongojs.Long.prototype.shiftLeft)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>shiftRight (numBits)](#apidoc.element.mongojs.Long.prototype.shiftRight)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.mongojs.Long.prototype.shiftRightUnsigned)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>subtract (other)](#apidoc.element.mongojs.Long.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toInt ()](#apidoc.element.mongojs.Long.prototype.toInt)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toJSON ()](#apidoc.element.mongojs.Long.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toNumber ()](#apidoc.element.mongojs.Long.prototype.toNumber)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toString (opt_radix)](#apidoc.element.mongojs.Long.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>xor (other)](#apidoc.element.mongojs.Long.prototype.xor)

#### [module mongojs.MaxKey](#apidoc.module.mongojs.MaxKey)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>MaxKey ()](#apidoc.element.mongojs.MaxKey.MaxKey)

#### [module mongojs.MinKey](#apidoc.module.mongojs.MinKey)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>MinKey ()](#apidoc.element.mongojs.MinKey.MinKey)

#### [module mongojs.ObjectID](#apidoc.module.mongojs.ObjectID)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>ObjectID (id)](#apidoc.element.mongojs.ObjectID.ObjectID)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>ObjectId (id)](#apidoc.element.mongojs.ObjectID.ObjectId)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>createFromHexString (string)](#apidoc.element.mongojs.ObjectID.createFromHexString)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>createFromTime (time)](#apidoc.element.mongojs.ObjectID.createFromTime)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>createPk ()](#apidoc.element.mongojs.ObjectID.createPk)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>isValid (id)](#apidoc.element.mongojs.ObjectID.isValid)
1.  number <span class="apidocSignatureSpan">mongojs.ObjectID.</span>index

#### [module mongojs.ObjectID.prototype](#apidoc.module.mongojs.ObjectID.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>equals (otherId)](#apidoc.element.mongojs.ObjectID.prototype.equals)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>generate (time)](#apidoc.element.mongojs.ObjectID.prototype.generate)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>getInc ()](#apidoc.element.mongojs.ObjectID.prototype.getInc)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>getTimestamp ()](#apidoc.element.mongojs.ObjectID.prototype.getTimestamp)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>get_inc ()](#apidoc.element.mongojs.ObjectID.prototype.get_inc)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>inspect (format)](#apidoc.element.mongojs.ObjectID.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>toHexString ()](#apidoc.element.mongojs.ObjectID.prototype.toHexString)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>toJSON ()](#apidoc.element.mongojs.ObjectID.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>toString (format)](#apidoc.element.mongojs.ObjectID.prototype.toString)

#### [module mongojs.Symbol](#apidoc.module.mongojs.Symbol)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Symbol (value)](#apidoc.element.mongojs.Symbol.Symbol)

#### [module mongojs.Symbol.prototype](#apidoc.module.mongojs.Symbol.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>inspect ()](#apidoc.element.mongojs.Symbol.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>toJSON ()](#apidoc.element.mongojs.Symbol.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>toString ()](#apidoc.element.mongojs.Symbol.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>valueOf ()](#apidoc.element.mongojs.Symbol.prototype.valueOf)

#### [module mongojs.Timestamp](#apidoc.module.mongojs.Timestamp)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>Timestamp (low, high)](#apidoc.element.mongojs.Timestamp.Timestamp)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromBits (lowBits, highBits)](#apidoc.element.mongojs.Timestamp.fromBits)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromInt (value)](#apidoc.element.mongojs.Timestamp.fromInt)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromNumber (value)](#apidoc.element.mongojs.Timestamp.fromNumber)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromString (str, opt_radix)](#apidoc.element.mongojs.Timestamp.fromString)
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_16_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_24_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_31_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_32_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_48_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_63_DBL_
1.  number <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_64_DBL_
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>INT_CACHE_
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>MAX_VALUE
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>MIN_VALUE
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>NEG_ONE
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>ONE
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>TWO_PWR_24_
1.  object <span class="apidocSignatureSpan">mongojs.Timestamp.</span>ZERO

#### [module mongojs.Timestamp.prototype](#apidoc.module.mongojs.Timestamp.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>add (other)](#apidoc.element.mongojs.Timestamp.prototype.add)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>and (other)](#apidoc.element.mongojs.Timestamp.prototype.and)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>compare (other)](#apidoc.element.mongojs.Timestamp.prototype.compare)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>div (other)](#apidoc.element.mongojs.Timestamp.prototype.div)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>equals (other)](#apidoc.element.mongojs.Timestamp.prototype.equals)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getHighBits ()](#apidoc.element.mongojs.Timestamp.prototype.getHighBits)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getLowBits ()](#apidoc.element.mongojs.Timestamp.prototype.getLowBits)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.mongojs.Timestamp.prototype.getLowBitsUnsigned)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getNumBitsAbs ()](#apidoc.element.mongojs.Timestamp.prototype.getNumBitsAbs)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>greaterThan (other)](#apidoc.element.mongojs.Timestamp.prototype.greaterThan)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.mongojs.Timestamp.prototype.greaterThanOrEqual)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>isNegative ()](#apidoc.element.mongojs.Timestamp.prototype.isNegative)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>isOdd ()](#apidoc.element.mongojs.Timestamp.prototype.isOdd)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>isZero ()](#apidoc.element.mongojs.Timestamp.prototype.isZero)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>lessThan (other)](#apidoc.element.mongojs.Timestamp.prototype.lessThan)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>lessThanOrEqual (other)](#apidoc.element.mongojs.Timestamp.prototype.lessThanOrEqual)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>modulo (other)](#apidoc.element.mongojs.Timestamp.prototype.modulo)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>multiply (other)](#apidoc.element.mongojs.Timestamp.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>negate ()](#apidoc.element.mongojs.Timestamp.prototype.negate)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>not ()](#apidoc.element.mongojs.Timestamp.prototype.not)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>notEquals (other)](#apidoc.element.mongojs.Timestamp.prototype.notEquals)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>or (other)](#apidoc.element.mongojs.Timestamp.prototype.or)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>shiftLeft (numBits)](#apidoc.element.mongojs.Timestamp.prototype.shiftLeft)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>shiftRight (numBits)](#apidoc.element.mongojs.Timestamp.prototype.shiftRight)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.mongojs.Timestamp.prototype.shiftRightUnsigned)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>subtract (other)](#apidoc.element.mongojs.Timestamp.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toInt ()](#apidoc.element.mongojs.Timestamp.prototype.toInt)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toJSON ()](#apidoc.element.mongojs.Timestamp.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toNumber ()](#apidoc.element.mongojs.Timestamp.prototype.toNumber)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toString (opt_radix)](#apidoc.element.mongojs.Timestamp.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>xor (other)](#apidoc.element.mongojs.Timestamp.prototype.xor)

#### [module mongojs.bulk](#apidoc.module.mongojs.bulk)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>bulk (colName, ordered, onserver)](#apidoc.element.mongojs.bulk.bulk)

#### [module mongojs.bulk.prototype](#apidoc.module.mongojs.bulk.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>execute (cb)](#apidoc.element.mongojs.bulk.prototype.execute)
1.  [function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>insert (doc)](#apidoc.element.mongojs.bulk.prototype.insert)
1.  [function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>toString ()](#apidoc.element.mongojs.bulk.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>tojson ()](#apidoc.element.mongojs.bulk.prototype.tojson)

#### [module mongojs.collection](#apidoc.module.mongojs.collection)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>collection (opts, getConnection)](#apidoc.element.mongojs.collection.collection)

#### [module mongojs.collection.prototype](#apidoc.module.mongojs.collection.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>aggregate ()](#apidoc.element.mongojs.collection.prototype.aggregate)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>count (query, cb)](#apidoc.element.mongojs.collection.prototype.count)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>createIndex (index, opts, cb)](#apidoc.element.mongojs.collection.prototype.createIndex)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>distinct (field, query, cb)](#apidoc.element.mongojs.collection.prototype.distinct)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>drop (cb)](#apidoc.element.mongojs.collection.prototype.drop)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>dropIndex (index, cb)](#apidoc.element.mongojs.collection.prototype.dropIndex)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>dropIndexes (cb)](#apidoc.element.mongojs.collection.prototype.dropIndexes)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>ensureIndex (index, opts, cb)](#apidoc.element.mongojs.collection.prototype.ensureIndex)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>find (query, projection, opts, cb)](#apidoc.element.mongojs.collection.prototype.find)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>findAndModify (opts, cb)](#apidoc.element.mongojs.collection.prototype.findAndModify)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>findOne (query, projection, cb)](#apidoc.element.mongojs.collection.prototype.findOne)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>getIndexes (cb)](#apidoc.element.mongojs.collection.prototype.getIndexes)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>group (doc, cb)](#apidoc.element.mongojs.collection.prototype.group)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>initializeOrderedBulkOp ()](#apidoc.element.mongojs.collection.prototype.initializeOrderedBulkOp)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>initializeUnorderedBulkOp ()](#apidoc.element.mongojs.collection.prototype.initializeUnorderedBulkOp)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>insert (docOrDocs, opts, cb)](#apidoc.element.mongojs.collection.prototype.insert)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>isCapped (cb)](#apidoc.element.mongojs.collection.prototype.isCapped)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>mapReduce (map, reduce, opts, cb)](#apidoc.element.mongojs.collection.prototype.mapReduce)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>reIndex (cb)](#apidoc.element.mongojs.collection.prototype.reIndex)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>remove (query, opts, cb)](#apidoc.element.mongojs.collection.prototype.remove)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>rename (name, opts, cb)](#apidoc.element.mongojs.collection.prototype.rename)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>runCommand (cmd, opts, cb)](#apidoc.element.mongojs.collection.prototype.runCommand)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>save (doc, opts, cb)](#apidoc.element.mongojs.collection.prototype.save)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>stats (cb)](#apidoc.element.mongojs.collection.prototype.stats)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>toString ()](#apidoc.element.mongojs.collection.prototype.toString)
1.  [function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>update (query, update, opts, cb)](#apidoc.element.mongojs.collection.prototype.update)

#### [module mongojs.cursor](#apidoc.module.mongojs.cursor)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>cursor (getCursor)](#apidoc.element.mongojs.cursor.cursor)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.</span>super_ (options)](#apidoc.element.mongojs.cursor.super_)

#### [module mongojs.cursor.prototype](#apidoc.module.mongojs.cursor.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>_read ()](#apidoc.element.mongojs.cursor.prototype._read)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>batchSize (obj, cb)](#apidoc.element.mongojs.cursor.prototype.batchSize)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>count (cb)](#apidoc.element.mongojs.cursor.prototype.count)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>destroy ()](#apidoc.element.mongojs.cursor.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>explain (cb)](#apidoc.element.mongojs.cursor.prototype.explain)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>forEach (fn)](#apidoc.element.mongojs.cursor.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>hint (obj, cb)](#apidoc.element.mongojs.cursor.prototype.hint)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>limit (obj, cb)](#apidoc.element.mongojs.cursor.prototype.limit)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>map (mapfn, cb)](#apidoc.element.mongojs.cursor.prototype.map)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>max (obj, cb)](#apidoc.element.mongojs.cursor.prototype.max)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>maxTimeMS (obj, cb)](#apidoc.element.mongojs.cursor.prototype.maxTimeMS)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>min (obj, cb)](#apidoc.element.mongojs.cursor.prototype.min)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>next (cb)](#apidoc.element.mongojs.cursor.prototype.next)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>rewind (cb)](#apidoc.element.mongojs.cursor.prototype.rewind)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>size (cb)](#apidoc.element.mongojs.cursor.prototype.size)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>skip (obj, cb)](#apidoc.element.mongojs.cursor.prototype.skip)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>snapshot (obj, cb)](#apidoc.element.mongojs.cursor.prototype.snapshot)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>sort (obj, cb)](#apidoc.element.mongojs.cursor.prototype.sort)
1.  [function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>toArray (cb)](#apidoc.element.mongojs.cursor.prototype.toArray)

#### [module mongojs.database](#apidoc.module.mongojs.database)
1.  [function <span class="apidocSignatureSpan">mongojs.</span>database (connString, cols, options)](#apidoc.element.mongojs.database.database)
1.  [function <span class="apidocSignatureSpan">mongojs.database.</span>super_ ()](#apidoc.element.mongojs.database.super_)

#### [module mongojs.database.prototype](#apidoc.module.mongojs.database.prototype)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>addUser (usr, cb)](#apidoc.element.mongojs.database.prototype.addUser)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>close (force, cb)](#apidoc.element.mongojs.database.prototype.close)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>collection (colName)](#apidoc.element.mongojs.database.prototype.collection)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>createCollection (name, opts, cb)](#apidoc.element.mongojs.database.prototype.createCollection)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>createUser (usr, cb)](#apidoc.element.mongojs.database.prototype.createUser)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>dropDatabase (cb)](#apidoc.element.mongojs.database.prototype.dropDatabase)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>dropUser (username, cb)](#apidoc.element.mongojs.database.prototype.dropUser)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>eval (fn)](#apidoc.element.mongojs.database.prototype.eval)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>getCollectionNames (cb)](#apidoc.element.mongojs.database.prototype.getCollectionNames)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>getLastError (cb)](#apidoc.element.mongojs.database.prototype.getLastError)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>getLastErrorObj (cb)](#apidoc.element.mongojs.database.prototype.getLastErrorObj)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>listCollections (cb)](#apidoc.element.mongojs.database.prototype.listCollections)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>removeUser (username, cb)](#apidoc.element.mongojs.database.prototype.removeUser)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>runCommand (opts, cb)](#apidoc.element.mongojs.database.prototype.runCommand)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>stats (scale, cb)](#apidoc.element.mongojs.database.prototype.stats)
1.  [function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>toString ()](#apidoc.element.mongojs.database.prototype.toString)



# <a name="apidoc.module.mongojs"></a>[module mongojs](#apidoc.module.mongojs)

#### <a name="apidoc.element.mongojs.Binary"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Binary (buffer, subType)](#apidoc.element.mongojs.Binary)
- description and source-code
```javascript
function Binary(buffer, subType) {
  if(!(this instanceof Binary)) return new Binary(buffer, subType);

  this._bsontype = 'Binary';

  if(buffer instanceof Number) {
    this.sub_type = buffer;
    this.position = 0;
  } else {
    this.sub_type = subType == null ? BSON_BINARY_SUBTYPE_DEFAULT : subType;
    this.position = 0;
  }

  if(buffer != null && !(buffer instanceof Number)) {
    // Only accept Buffer, Uint8Array or Arrays
    if(typeof buffer == 'string') {
      // Different ways of writing the length of the string for the different types
      if(typeof Buffer != 'undefined') {
        this.buffer = new Buffer(buffer);
      } else if(typeof Uint8Array != 'undefined' || (Object.prototype.toString.call(buffer) == '[object Array]')) {
        this.buffer = writeStringToArray(buffer);
      } else {
        throw new Error("only String, Buffer, Uint8Array or Array accepted");
      }
    } else {
      this.buffer = buffer;
    }
    this.position = buffer.length;
  } else {
    if(typeof Buffer != 'undefined') {
      this.buffer =  new Buffer(Binary.BUFFER_SIZE);
    } else if(typeof Uint8Array != 'undefined'){
      this.buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE));
    } else {
      this.buffer = new Array(Binary.BUFFER_SIZE);
    }
    // Set position to start of buffer
    this.position = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Code"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Code (code, scope)](#apidoc.element.mongojs.Code)
- description and source-code
```javascript
function Code(code, scope) {
  if(!(this instanceof Code)) return new Code(code, scope);
  this._bsontype = 'Code';
  this.code = code;
  this.scope = scope;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.DBRef"></a>[function <span class="apidocSignatureSpan">mongojs.</span>DBRef (namespace, oid, db)](#apidoc.element.mongojs.DBRef)
- description and source-code
```javascript
function DBRef(namespace, oid, db) {
  if(!(this instanceof DBRef)) return new DBRef(namespace, oid, db);

  this._bsontype = 'DBRef';
  this.namespace = namespace;
  this.oid = oid;
  this.db = db;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Double"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Double (value)](#apidoc.element.mongojs.Double)
- description and source-code
```javascript
function Double(value) {
  if(!(this instanceof Double)) return new Double(value);

  this._bsontype = 'Double';
  this.value = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Long (low, high)](#apidoc.element.mongojs.Long)
- description and source-code
```javascript
function Long(low, high) {
  if(!(this instanceof Long)) return new Long(low, high);

  this._bsontype = 'Long';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.MaxKey"></a>[function <span class="apidocSignatureSpan">mongojs.</span>MaxKey ()](#apidoc.element.mongojs.MaxKey)
- description and source-code
```javascript
function MaxKey() {
  if(!(this instanceof MaxKey)) return new MaxKey();

  this._bsontype = 'MaxKey';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.MinKey"></a>[function <span class="apidocSignatureSpan">mongojs.</span>MinKey ()](#apidoc.element.mongojs.MinKey)
- description and source-code
```javascript
function MinKey() {
  if(!(this instanceof MinKey)) return new MinKey();

  this._bsontype = 'MinKey';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.NumberLong"></a>[function <span class="apidocSignatureSpan">mongojs.</span>NumberLong (low, high)](#apidoc.element.mongojs.NumberLong)
- description and source-code
```javascript
function Long(low, high) {
  if(!(this instanceof Long)) return new Long(low, high);

  this._bsontype = 'Long';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID"></a>[function <span class="apidocSignatureSpan">mongojs.</span>ObjectID (id)](#apidoc.element.mongojs.ObjectID)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectId"></a>[function <span class="apidocSignatureSpan">mongojs.</span>ObjectId (id)](#apidoc.element.mongojs.ObjectId)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
...
		return
	}
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
...
```

#### <a name="apidoc.element.mongojs.Symbol"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Symbol (value)](#apidoc.element.mongojs.Symbol)
- description and source-code
```javascript
function Symbol(value) {
  if(!(this instanceof Symbol)) return new Symbol(value);
  this._bsontype = 'Symbol';
  this.value = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Timestamp (low, high)](#apidoc.element.mongojs.Timestamp)
- description and source-code
```javascript
function Timestamp(low, high) {
  if(!(this instanceof Timestamp)) return new Timestamp(low, high);
  this._bsontype = 'Timestamp';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.bulk"></a>[function <span class="apidocSignatureSpan">mongojs.</span>bulk (colName, ordered, onserver)](#apidoc.element.mongojs.bulk)
- description and source-code
```javascript
bulk = function (colName, ordered, onserver) {
  this._colname = colName
  this._cmds = []
  this._currCmd = null
  this._ordered = ordered
  this._getConnection = onserver

  var self = this
  this.find = function (query) {
    var upsert = false
    var findobj = {}
    var remove = function (lim) {
      if (!self._currCmd) {
        self._currCmd = {
          delete: self._colname,
          deletes: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      if (!self._currCmd.delete) {
        self._cmds.push(self._currCmd)
        self._currCmd = {
          delete: self._colname,
          deletes: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      self._currCmd.deletes.push({q: query, limit: lim})
    }

    var update = function (updObj, multi) {
      if (!self._currCmd) {
        self._currCmd = {
          update: self._colname,
          updates: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      if (!self._currCmd.update) {
        self._cmds.push(self._currCmd)
        self._currCmd = {
          update: self._colname,
          updates: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      self._currCmd.updates.push({q: query, u: updObj, multi: multi, upsert: upsert})
    }

    findobj.upsert = function () {
      upsert = true
      return findobj
    }

    findobj.remove = function () {
      remove(0)
    }

    findobj.removeOne = function () {
      remove(1)
    }

    findobj.update = function (updObj) {
      update(updObj, true)
    }

    findobj.updateOne = function (updObj) {
      update(updObj, false)
    }

    findobj.replaceOne = function (updObj) {
      this.updateOne(updObj)
    }

    return findobj
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.collection"></a>[function <span class="apidocSignatureSpan">mongojs.</span>collection (opts, getConnection)](#apidoc.element.mongojs.collection)
- description and source-code
```javascript
collection = function (opts, getConnection) {
  this._name = opts.name
  this._getConnection = getConnection
  this._getCollection = function (cb) {
    var collectionName = this._name

    this._getConnection(function (err, connection) {
      if (err) { return cb(err) }

      cb(null, connection.collection(collectionName))
    })
  }
}
```
- example usage
```shell
...
var db = mongojs('username:password@example.com/mydb?authSource=authdb', ['mycollection'])

// connect with options
var db = mongojs('username:password@example.com/mydb', ['mycollection'], { ssl: true })

// connect now, and worry about collections later
var db = mongojs('mydb')
var mycollection = db.collection('mycollection')
'''

[More connection string examples](http://mongodb.github.io/node-mongodb-native/2.0/reference/connecting/)

After we connected we can query or update the database just how we would using the mongo API with the exception that we use a callback
.
The format for callbacks is always 'callback(error, value)' where error is null if no exception has occured. The update methods '
save', 'remove', 'update' and 'findAndModify' also pass the 'lastErrorObject' as the last argument to the callback function.
...
```

#### <a name="apidoc.element.mongojs.cursor"></a>[function <span class="apidocSignatureSpan">mongojs.</span>cursor (getCursor)](#apidoc.element.mongojs.cursor)
- description and source-code
```javascript
cursor = function (getCursor) {
  Readable.call(this, {objectMode: true, highWaterMark: 0})

  this._opts = {}

  var self = this
  this._get = thunky(function (cb) {
    getCursor(function (err, cursor) {
      if (err) { return cb(err) }

      // Apply all opts
      for (var key in self._opts) {
        if (self._opts.hasOwnProperty(key)) {
          cursor = cursor[key](self._opts[key])
        }
      }

      cb(null, cursor)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.database"></a>[function <span class="apidocSignatureSpan">mongojs.</span>database (connString, cols, options)](#apidoc.element.mongojs.database)
- description and source-code
```javascript
database = function (connString, cols, options) {
  var self = this

  EventEmitter.call(this)

  if (typeof connString === 'string') {
    this._dbname = parse(connString).dbName

    // Fix short cut connection URLs consisting only of a db name or db + host
    if (connString.indexOf('/') < 0) {
      connString = 'localhost/' + connString
    }

    if (connString.indexOf('mongodb://') < 0) {
      connString = 'mongodb://' + connString
    }

    this._getConnection = thunky(function (cb) {
      mongodb.connect(connString, options, function (err, db) {
        if (err) {
          self.emit('error', err) // It's safer to emit an error instead of rely on the cb to handle the error
          return cb(err)
        }

        self.emit('connect')
        cb(null, db)
      })
    })
  } else if (typeof connString._getConnection === 'function') { // mongojs
    this._dbname = connString._dbname
    this._getConnection = connString._getConnection
  } else { // try mongodb-native
    this._dbname = parse(connString.options.url).dbName

    this._getConnection = thunky(function (cb) {
      cb(null, connString)
    })
  }

  this.ObjectId = mongodb.ObjectId

  cols = cols || []
  cols.forEach(function (colName) {
    self[colName] = self.collection(colName)

    var parts = colName.split('.')

    var last = parts.pop()
    var parent = parts.reduce(function (parent, prefix) {
      parent[prefix] = parent[prefix] || {}
      return parent[prefix]
    }, self)

    parent[last] = self.collection(colName)
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Binary"></a>[module mongojs.Binary](#apidoc.module.mongojs.Binary)

#### <a name="apidoc.element.mongojs.Binary.Binary"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Binary (buffer, subType)](#apidoc.element.mongojs.Binary.Binary)
- description and source-code
```javascript
function Binary(buffer, subType) {
  if(!(this instanceof Binary)) return new Binary(buffer, subType);

  this._bsontype = 'Binary';

  if(buffer instanceof Number) {
    this.sub_type = buffer;
    this.position = 0;
  } else {
    this.sub_type = subType == null ? BSON_BINARY_SUBTYPE_DEFAULT : subType;
    this.position = 0;
  }

  if(buffer != null && !(buffer instanceof Number)) {
    // Only accept Buffer, Uint8Array or Arrays
    if(typeof buffer == 'string') {
      // Different ways of writing the length of the string for the different types
      if(typeof Buffer != 'undefined') {
        this.buffer = new Buffer(buffer);
      } else if(typeof Uint8Array != 'undefined' || (Object.prototype.toString.call(buffer) == '[object Array]')) {
        this.buffer = writeStringToArray(buffer);
      } else {
        throw new Error("only String, Buffer, Uint8Array or Array accepted");
      }
    } else {
      this.buffer = buffer;
    }
    this.position = buffer.length;
  } else {
    if(typeof Buffer != 'undefined') {
      this.buffer =  new Buffer(Binary.BUFFER_SIZE);
    } else if(typeof Uint8Array != 'undefined'){
      this.buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE));
    } else {
      this.buffer = new Array(Binary.BUFFER_SIZE);
    }
    // Set position to start of buffer
    this.position = 0;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Binary.prototype"></a>[module mongojs.Binary.prototype](#apidoc.module.mongojs.Binary.prototype)

#### <a name="apidoc.element.mongojs.Binary.prototype.length"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>length ()](#apidoc.element.mongojs.Binary.prototype.length)
- description and source-code
```javascript
function length() {
  return this.position;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Binary.prototype.put"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>put (byte_value)](#apidoc.element.mongojs.Binary.prototype.put)
- description and source-code
```javascript
function put(byte_value) {
  // If it's a string and a has more than one character throw an error
  if(byte_value['length'] != null && typeof byte_value != 'number' && byte_value.length != 1) throw new Error("only accepts single
 character String, Uint8Array or Array");
  if(typeof byte_value != 'number' && byte_value < 0 || byte_value > 255) throw new Error("only accepts number in a valid unsigned
 byte range 0-255");

  // Decode the byte value once
  var decoded_byte = null;
  if(typeof byte_value == 'string') {
    decoded_byte = byte_value.charCodeAt(0);
  } else if(byte_value['length'] != null) {
    decoded_byte = byte_value[0];
  } else {
    decoded_byte = byte_value;
  }

  if(this.buffer.length > this.position) {
    this.buffer[this.position++] = decoded_byte;
  } else {
    if(typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer)) {
      // Create additional overflow buffer
      var buffer = new Buffer(Binary.BUFFER_SIZE + this.buffer.length);
      // Combine the two buffers together
      this.buffer.copy(buffer, 0, 0, this.buffer.length);
      this.buffer = buffer;
      this.buffer[this.position++] = decoded_byte;
    } else {
      var buffer = null;
      // Create a new buffer (typed or normal array)
      if(Object.prototype.toString.call(this.buffer) == '[object Uint8Array]') {
        buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE + this.buffer.length));
      } else {
        buffer = new Array(Binary.BUFFER_SIZE + this.buffer.length);
      }

      // We need to copy all the content to the new array
      for(var i = 0; i < this.buffer.length; i++) {
        buffer[i] = this.buffer[i];
      }

      // Reassign the buffer
      this.buffer = buffer;
      // Write the byte
      this.buffer[this.position++] = decoded_byte;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Binary.prototype.read"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>read (position, length)](#apidoc.element.mongojs.Binary.prototype.read)
- description and source-code
```javascript
function read(position, length) {
  length = length && length > 0
    ? length
    : this.position;

  // Let's return the data based on the type we have
  if(this.buffer['slice']) {
    return this.buffer.slice(position, position + length);
  } else {
    // Create a buffer to keep the result
    var buffer = typeof Uint8Array != 'undefined' ? new Uint8Array(new ArrayBuffer(length)) : new Array(length);
    for(var i = 0; i < length; i++) {
      buffer[i] = this.buffer[position++];
    }
  }
  // Return the buffer
  return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Binary.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>toJSON ()](#apidoc.element.mongojs.Binary.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.buffer != null ? this.buffer.toString('base64') : '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Binary.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>toString (format)](#apidoc.element.mongojs.Binary.prototype.toString)
- description and source-code
```javascript
toString = function (format) {
  return this.buffer != null ? this.buffer.slice(0, this.position).toString(format) : '';
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```

#### <a name="apidoc.element.mongojs.Binary.prototype.value"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>value (asRaw)](#apidoc.element.mongojs.Binary.prototype.value)
- description and source-code
```javascript
function value(asRaw) {
  asRaw = asRaw == null ? false : asRaw;

  // Optimize to serialize for the situation where the data == size of buffer
  if(asRaw && typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer) && this.buffer.length == this.position)
    return this.buffer;

  // If it's a node.js buffer object
  if(typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer)) {
    return asRaw ? this.buffer.slice(0, this.position) : this.buffer.toString('binary', 0, this.position);
  } else {
    if(asRaw) {
      // we support the slice command use it
      if(this.buffer['slice'] != null) {
        return this.buffer.slice(0, this.position);
      } else {
        // Create a new buffer to copy content to
        var newBuffer = Object.prototype.toString.call(this.buffer) == '[object Uint8Array]' ? new Uint8Array(new ArrayBuffer(this
.position)) : new Array(this.position);
        // Copy content
        for(var i = 0; i < this.position; i++) {
          newBuffer[i] = this.buffer[i];
        }
        // Return the buffer
        return newBuffer;
      }
    } else {
      return convertArraytoUtf8BinaryString(this.buffer, 0, this.position);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Binary.prototype.write"></a>[function <span class="apidocSignatureSpan">mongojs.Binary.prototype.</span>write (string, offset)](#apidoc.element.mongojs.Binary.prototype.write)
- description and source-code
```javascript
function write(string, offset) {
  offset = typeof offset == 'number' ? offset : this.position;

  // If the buffer is to small let's extend the buffer
  if(this.buffer.length < offset + string.length) {
    var buffer = null;
    // If we are in node.js
    if(typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer)) {
      buffer = new Buffer(this.buffer.length + string.length);
      this.buffer.copy(buffer, 0, 0, this.buffer.length);
    } else if(Object.prototype.toString.call(this.buffer) == '[object Uint8Array]') {
      // Create a new buffer
      buffer = new Uint8Array(new ArrayBuffer(this.buffer.length + string.length))
      // Copy the content
      for(var i = 0; i < this.position; i++) {
        buffer[i] = this.buffer[i];
      }
    }

    // Assign the new buffer
    this.buffer = buffer;
  }

  if(typeof Buffer != 'undefined' && Buffer.isBuffer(string) && Buffer.isBuffer(this.buffer)) {
    string.copy(this.buffer, offset, 0, string.length);
    this.position = (offset + string.length) > this.position ? (offset + string.length) : this.position;
    // offset = string.length
  } else if(typeof Buffer != 'undefined' && typeof string == 'string' && Buffer.isBuffer(this.buffer)) {
    this.buffer.write(string, offset, 'binary');
    this.position = (offset + string.length) > this.position ? (offset + string.length) : this.position;
    // offset = string.length;
  } else if(Object.prototype.toString.call(string) == '[object Uint8Array]'
    || Object.prototype.toString.call(string) == '[object Array]' && typeof string != 'string') {
    for(var i = 0; i < string.length; i++) {
      this.buffer[offset++] = string[i];
    }

    this.position = offset > this.position ? offset : this.position;
  } else if(typeof string == 'string') {
    for(var i = 0; i < string.length; i++) {
      this.buffer[offset++] = string.charCodeAt(i);
    }

    this.position = offset > this.position ? offset : this.position;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Code"></a>[module mongojs.Code](#apidoc.module.mongojs.Code)

#### <a name="apidoc.element.mongojs.Code.Code"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Code (code, scope)](#apidoc.element.mongojs.Code.Code)
- description and source-code
```javascript
function Code(code, scope) {
  if(!(this instanceof Code)) return new Code(code, scope);
  this._bsontype = 'Code';
  this.code = code;
  this.scope = scope;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Code.prototype"></a>[module mongojs.Code.prototype](#apidoc.module.mongojs.Code.prototype)

#### <a name="apidoc.element.mongojs.Code.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.Code.prototype.</span>toJSON ()](#apidoc.element.mongojs.Code.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {scope:this.scope, code:this.code};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.DBRef"></a>[module mongojs.DBRef](#apidoc.module.mongojs.DBRef)

#### <a name="apidoc.element.mongojs.DBRef.DBRef"></a>[function <span class="apidocSignatureSpan">mongojs.</span>DBRef (namespace, oid, db)](#apidoc.element.mongojs.DBRef.DBRef)
- description and source-code
```javascript
function DBRef(namespace, oid, db) {
  if(!(this instanceof DBRef)) return new DBRef(namespace, oid, db);

  this._bsontype = 'DBRef';
  this.namespace = namespace;
  this.oid = oid;
  this.db = db;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.DBRef.prototype"></a>[module mongojs.DBRef.prototype](#apidoc.module.mongojs.DBRef.prototype)

#### <a name="apidoc.element.mongojs.DBRef.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.DBRef.prototype.</span>toJSON ()](#apidoc.element.mongojs.DBRef.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {
    '$ref':this.namespace,
    '$id':this.oid,
    '$db':this.db == null ? '' : this.db
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Double"></a>[module mongojs.Double](#apidoc.module.mongojs.Double)

#### <a name="apidoc.element.mongojs.Double.Double"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Double (value)](#apidoc.element.mongojs.Double.Double)
- description and source-code
```javascript
function Double(value) {
  if(!(this instanceof Double)) return new Double(value);

  this._bsontype = 'Double';
  this.value = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Double.prototype"></a>[module mongojs.Double.prototype](#apidoc.module.mongojs.Double.prototype)

#### <a name="apidoc.element.mongojs.Double.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.Double.prototype.</span>toJSON ()](#apidoc.element.mongojs.Double.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Double.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">mongojs.Double.prototype.</span>valueOf ()](#apidoc.element.mongojs.Double.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Long"></a>[module mongojs.Long](#apidoc.module.mongojs.Long)

#### <a name="apidoc.element.mongojs.Long.Long"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Long (low, high)](#apidoc.element.mongojs.Long.Long)
- description and source-code
```javascript
function Long(low, high) {
  if(!(this instanceof Long)) return new Long(low, high);

  this._bsontype = 'Long';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.fromBits"></a>[function <span class="apidocSignatureSpan">mongojs.Long.</span>fromBits (lowBits, highBits)](#apidoc.element.mongojs.Long.fromBits)
- description and source-code
```javascript
fromBits = function (lowBits, highBits) {
  return new Long(lowBits, highBits);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.fromInt"></a>[function <span class="apidocSignatureSpan">mongojs.Long.</span>fromInt (value)](#apidoc.element.mongojs.Long.fromInt)
- description and source-code
```javascript
fromInt = function (value) {
  if (-128 <= value && value < 128) {
    var cachedObj = Long.INT_CACHE_[value];
    if (cachedObj) {
      return cachedObj;
    }
  }

  var obj = new Long(value | 0, value < 0 ? -1 : 0);
  if (-128 <= value && value < 128) {
    Long.INT_CACHE_[value] = obj;
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.fromNumber"></a>[function <span class="apidocSignatureSpan">mongojs.Long.</span>fromNumber (value)](#apidoc.element.mongojs.Long.fromNumber)
- description and source-code
```javascript
fromNumber = function (value) {
  if (isNaN(value) || !isFinite(value)) {
    return Long.ZERO;
  } else if (value <= -Long.TWO_PWR_63_DBL_) {
    return Long.MIN_VALUE;
  } else if (value + 1 >= Long.TWO_PWR_63_DBL_) {
    return Long.MAX_VALUE;
  } else if (value < 0) {
    return Long.fromNumber(-value).negate();
  } else {
    return new Long(
               (value % Long.TWO_PWR_32_DBL_) | 0,
               (value / Long.TWO_PWR_32_DBL_) | 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.fromString"></a>[function <span class="apidocSignatureSpan">mongojs.Long.</span>fromString (str, opt_radix)](#apidoc.element.mongojs.Long.fromString)
- description and source-code
```javascript
fromString = function (str, opt_radix) {
  if (str.length == 0) {
    throw Error('number format error: empty string');
  }

  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (str.charAt(0) == '-') {
    return Long.fromString(str.substring(1), radix).negate();
  } else if (str.indexOf('-') >= 0) {
    throw Error('number format error: interior "-" character: ' + str);
  }

  // Do several (8) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Long.fromNumber(Math.pow(radix, 8));

  var result = Long.ZERO;
  for (var i = 0; i < str.length; i += 8) {
    var size = Math.min(8, str.length - i);
    var value = parseInt(str.substring(i, i + size), radix);
    if (size < 8) {
      var power = Long.fromNumber(Math.pow(radix, size));
      result = result.multiply(power).add(Long.fromNumber(value));
    } else {
      result = result.multiply(radixToPower);
      result = result.add(Long.fromNumber(value));
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Long.prototype"></a>[module mongojs.Long.prototype](#apidoc.module.mongojs.Long.prototype)

#### <a name="apidoc.element.mongojs.Long.prototype.add"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>add (other)](#apidoc.element.mongojs.Long.prototype.add)
- description and source-code
```javascript
add = function (other) {
  // Divide each number into 4 chunks of 16 bits, and then sum the chunks.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 + b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 + b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 + b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 + b48;
  c48 &= 0xFFFF;
  return Long.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.and"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>and (other)](#apidoc.element.mongojs.Long.prototype.and)
- description and source-code
```javascript
and = function (other) {
  return Long.fromBits(this.low_ & other.low_, this.high_ & other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.compare"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>compare (other)](#apidoc.element.mongojs.Long.prototype.compare)
- description and source-code
```javascript
compare = function (other) {
  if (this.equals(other)) {
    return 0;
  }

  var thisNeg = this.isNegative();
  var otherNeg = other.isNegative();
  if (thisNeg && !otherNeg) {
    return -1;
  }
  if (!thisNeg && otherNeg) {
    return 1;
  }

  // at this point, the signs are the same, so subtraction will not overflow
  if (this.subtract(other).isNegative()) {
    return -1;
  } else {
    return 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.div"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>div (other)](#apidoc.element.mongojs.Long.prototype.div)
- description and source-code
```javascript
div = function (other) {
  if (other.isZero()) {
    throw Error('division by zero');
  } else if (this.isZero()) {
    return Long.ZERO;
  }

  if (this.equals(Long.MIN_VALUE)) {
    if (other.equals(Long.ONE) ||
        other.equals(Long.NEG_ONE)) {
      return Long.MIN_VALUE;  // recall that -MIN_VALUE == MIN_VALUE
    } else if (other.equals(Long.MIN_VALUE)) {
      return Long.ONE;
    } else {
      // At this point, we have |other| >= 2, so |this/other| < |MIN_VALUE|.
      var halfThis = this.shiftRight(1);
      var approx = halfThis.div(other).shiftLeft(1);
      if (approx.equals(Long.ZERO)) {
        return other.isNegative() ? Long.ONE : Long.NEG_ONE;
      } else {
        var rem = this.subtract(other.multiply(approx));
        var result = approx.add(rem.div(other));
        return result;
      }
    }
  } else if (other.equals(Long.MIN_VALUE)) {
    return Long.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().div(other.negate());
    } else {
      return this.negate().div(other).negate();
    }
  } else if (other.isNegative()) {
    return this.div(other.negate()).negate();
  }

  // Repeat the following until the remainder is less than other:  find a
  // floating-point that approximates remainder / other *from below*, add this
  // into the result, and subtract it from the remainder.  It is critical that
  // the approximate value is less than or equal to the real value so that the
  // remainder never becomes negative.
  var res = Long.ZERO;
  var rem = this;
  while (rem.greaterThanOrEqual(other)) {
    // Approximate the result of division. This may be a little greater or
    // smaller than the actual value.
    var approx = Math.max(1, Math.floor(rem.toNumber() / other.toNumber()));

    // We will tweak the approximate result by changing it in the 48-th digit or
    // the smallest non-fractional digit, whichever is larger.
    var log2 = Math.ceil(Math.log(approx) / Math.LN2);
    var delta = (log2 <= 48) ? 1 : Math.pow(2, log2 - 48);

    // Decrease the approximation until it is smaller than the remainder.  Note
    // that if it is too large, the product overflows and is negative.
    var approxRes = Long.fromNumber(approx);
    var approxRem = approxRes.multiply(other);
    while (approxRem.isNegative() || approxRem.greaterThan(rem)) {
      approx -= delta;
      approxRes = Long.fromNumber(approx);
      approxRem = approxRes.multiply(other);
    }

    // We know the answer can't be zero... and actually, zero would cause
    // infinite recursion since we would make no progress.
    if (approxRes.isZero()) {
      approxRes = Long.ONE;
    }

    res = res.add(approxRes);
    rem = rem.subtract(approxRem);
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.equals"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>equals (other)](#apidoc.element.mongojs.Long.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return (this.high_ == other.high_) && (this.low_ == other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.getHighBits"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getHighBits ()](#apidoc.element.mongojs.Long.prototype.getHighBits)
- description and source-code
```javascript
getHighBits = function () {
  return this.high_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.getLowBits"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getLowBits ()](#apidoc.element.mongojs.Long.prototype.getLowBits)
- description and source-code
```javascript
getLowBits = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.getLowBitsUnsigned"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.mongojs.Long.prototype.getLowBitsUnsigned)
- description and source-code
```javascript
getLowBitsUnsigned = function () {
  return (this.low_ >= 0) ?
      this.low_ : Long.TWO_PWR_32_DBL_ + this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.getNumBitsAbs"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>getNumBitsAbs ()](#apidoc.element.mongojs.Long.prototype.getNumBitsAbs)
- description and source-code
```javascript
getNumBitsAbs = function () {
  if (this.isNegative()) {
    if (this.equals(Long.MIN_VALUE)) {
      return 64;
    } else {
      return this.negate().getNumBitsAbs();
    }
  } else {
    var val = this.high_ != 0 ? this.high_ : this.low_;
    for (var bit = 31; bit > 0; bit--) {
      if ((val & (1 << bit)) != 0) {
        break;
      }
    }
    return this.high_ != 0 ? bit + 33 : bit + 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.greaterThan"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>greaterThan (other)](#apidoc.element.mongojs.Long.prototype.greaterThan)
- description and source-code
```javascript
greaterThan = function (other) {
  return this.compare(other) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.greaterThanOrEqual"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.mongojs.Long.prototype.greaterThanOrEqual)
- description and source-code
```javascript
greaterThanOrEqual = function (other) {
  return this.compare(other) >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.isNegative"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>isNegative ()](#apidoc.element.mongojs.Long.prototype.isNegative)
- description and source-code
```javascript
isNegative = function () {
  return this.high_ < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.isOdd"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>isOdd ()](#apidoc.element.mongojs.Long.prototype.isOdd)
- description and source-code
```javascript
isOdd = function () {
  return (this.low_ & 1) == 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.isZero"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>isZero ()](#apidoc.element.mongojs.Long.prototype.isZero)
- description and source-code
```javascript
isZero = function () {
  return this.high_ == 0 && this.low_ == 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.lessThan"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>lessThan (other)](#apidoc.element.mongojs.Long.prototype.lessThan)
- description and source-code
```javascript
lessThan = function (other) {
  return this.compare(other) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.lessThanOrEqual"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>lessThanOrEqual (other)](#apidoc.element.mongojs.Long.prototype.lessThanOrEqual)
- description and source-code
```javascript
lessThanOrEqual = function (other) {
  return this.compare(other) <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.modulo"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>modulo (other)](#apidoc.element.mongojs.Long.prototype.modulo)
- description and source-code
```javascript
modulo = function (other) {
  return this.subtract(this.div(other).multiply(other));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.multiply"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>multiply (other)](#apidoc.element.mongojs.Long.prototype.multiply)
- description and source-code
```javascript
multiply = function (other) {
  if (this.isZero()) {
    return Long.ZERO;
  } else if (other.isZero()) {
    return Long.ZERO;
  }

  if (this.equals(Long.MIN_VALUE)) {
    return other.isOdd() ? Long.MIN_VALUE : Long.ZERO;
  } else if (other.equals(Long.MIN_VALUE)) {
    return this.isOdd() ? Long.MIN_VALUE : Long.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().multiply(other.negate());
    } else {
      return this.negate().multiply(other).negate();
    }
  } else if (other.isNegative()) {
    return this.multiply(other.negate()).negate();
  }

  // If both Longs are small, use float multiplication
  if (this.lessThan(Long.TWO_PWR_24_) &&
      other.lessThan(Long.TWO_PWR_24_)) {
    return Long.fromNumber(this.toNumber() * other.toNumber());
  }

  // Divide each Long into 4 chunks of 16 bits, and then add up 4x4 products.
  // We can skip products that would overflow.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 * b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 * b00;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c16 += a00 * b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 * b00;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a16 * b16;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a00 * b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 * b00 + a32 * b16 + a16 * b32 + a00 * b48;
  c48 &= 0xFFFF;
  return Long.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.negate"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>negate ()](#apidoc.element.mongojs.Long.prototype.negate)
- description and source-code
```javascript
negate = function () {
  if (this.equals(Long.MIN_VALUE)) {
    return Long.MIN_VALUE;
  } else {
    return this.not().add(Long.ONE);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.not"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>not ()](#apidoc.element.mongojs.Long.prototype.not)
- description and source-code
```javascript
not = function () {
  return Long.fromBits(~this.low_, ~this.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.notEquals"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>notEquals (other)](#apidoc.element.mongojs.Long.prototype.notEquals)
- description and source-code
```javascript
notEquals = function (other) {
  return (this.high_ != other.high_) || (this.low_ != other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.or"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>or (other)](#apidoc.element.mongojs.Long.prototype.or)
- description and source-code
```javascript
or = function (other) {
  return Long.fromBits(this.low_ | other.low_, this.high_ | other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.shiftLeft"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>shiftLeft (numBits)](#apidoc.element.mongojs.Long.prototype.shiftLeft)
- description and source-code
```javascript
shiftLeft = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var low = this.low_;
    if (numBits < 32) {
      var high = this.high_;
      return Long.fromBits(
                 low << numBits,
                 (high << numBits) | (low >>> (32 - numBits)));
    } else {
      return Long.fromBits(0, low << (numBits - 32));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.shiftRight"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>shiftRight (numBits)](#apidoc.element.mongojs.Long.prototype.shiftRight)
- description and source-code
```javascript
shiftRight = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Long.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >> numBits);
    } else {
      return Long.fromBits(
                 high >> (numBits - 32),
                 high >= 0 ? 0 : -1);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.shiftRightUnsigned"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.mongojs.Long.prototype.shiftRightUnsigned)
- description and source-code
```javascript
shiftRightUnsigned = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Long.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >>> numBits);
    } else if (numBits == 32) {
      return Long.fromBits(high, 0);
    } else {
      return Long.fromBits(high >>> (numBits - 32), 0);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.subtract"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>subtract (other)](#apidoc.element.mongojs.Long.prototype.subtract)
- description and source-code
```javascript
subtract = function (other) {
  return this.add(other.negate());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.toInt"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toInt ()](#apidoc.element.mongojs.Long.prototype.toInt)
- description and source-code
```javascript
toInt = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toJSON ()](#apidoc.element.mongojs.Long.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.toNumber"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toNumber ()](#apidoc.element.mongojs.Long.prototype.toNumber)
- description and source-code
```javascript
toNumber = function () {
  return this.high_ * Long.TWO_PWR_32_DBL_ +
         this.getLowBitsUnsigned();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Long.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>toString (opt_radix)](#apidoc.element.mongojs.Long.prototype.toString)
- description and source-code
```javascript
toString = function (opt_radix) {
  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (this.isZero()) {
    return '0';
  }

  if (this.isNegative()) {
    if (this.equals(Long.MIN_VALUE)) {
      // We need to change the Long value before it can be negated, so we remove
      // the bottom-most digit in this base and then recurse to do the rest.
      var radixLong = Long.fromNumber(radix);
      var div = this.div(radixLong);
      var rem = div.multiply(radixLong).subtract(this);
      return div.toString(radix) + rem.toInt().toString(radix);
    } else {
      return '-' + this.negate().toString(radix);
    }
  }

  // Do several (6) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Long.fromNumber(Math.pow(radix, 6));

  var rem = this;
  var result = '';
  while (true) {
    var remDiv = rem.div(radixToPower);
    var intval = rem.subtract(remDiv.multiply(radixToPower)).toInt();
    var digits = intval.toString(radix);

    rem = remDiv;
    if (rem.isZero()) {
      return digits + result;
    } else {
      while (digits.length < 6) {
        digits = '0' + digits;
      }
      result = '' + digits + result;
    }
  }
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```

#### <a name="apidoc.element.mongojs.Long.prototype.xor"></a>[function <span class="apidocSignatureSpan">mongojs.Long.prototype.</span>xor (other)](#apidoc.element.mongojs.Long.prototype.xor)
- description and source-code
```javascript
xor = function (other) {
  return Long.fromBits(this.low_ ^ other.low_, this.high_ ^ other.high_);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.MaxKey"></a>[module mongojs.MaxKey](#apidoc.module.mongojs.MaxKey)

#### <a name="apidoc.element.mongojs.MaxKey.MaxKey"></a>[function <span class="apidocSignatureSpan">mongojs.</span>MaxKey ()](#apidoc.element.mongojs.MaxKey.MaxKey)
- description and source-code
```javascript
function MaxKey() {
  if(!(this instanceof MaxKey)) return new MaxKey();

  this._bsontype = 'MaxKey';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.MinKey"></a>[module mongojs.MinKey](#apidoc.module.mongojs.MinKey)

#### <a name="apidoc.element.mongojs.MinKey.MinKey"></a>[function <span class="apidocSignatureSpan">mongojs.</span>MinKey ()](#apidoc.element.mongojs.MinKey.MinKey)
- description and source-code
```javascript
function MinKey() {
  if(!(this instanceof MinKey)) return new MinKey();

  this._bsontype = 'MinKey';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.ObjectID"></a>[module mongojs.ObjectID](#apidoc.module.mongojs.ObjectID)

#### <a name="apidoc.element.mongojs.ObjectID.ObjectID"></a>[function <span class="apidocSignatureSpan">mongojs.</span>ObjectID (id)](#apidoc.element.mongojs.ObjectID.ObjectID)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.ObjectId"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>ObjectId (id)](#apidoc.element.mongojs.ObjectID.ObjectId)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
...
		return
	}
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
...
```

#### <a name="apidoc.element.mongojs.ObjectID.createFromHexString"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>createFromHexString (string)](#apidoc.element.mongojs.ObjectID.createFromHexString)
- description and source-code
```javascript
function createFromHexString(string) {
  // Throw an error if it's not a valid setup
  if(typeof string === 'undefined' || string != null && string.length != 24) {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  // Use Buffer.from method if available
  if(hasBufferType) return new ObjectID(new Buffer(string, 'hex'));

  // Calculate lengths
  var array = new _Buffer(12);
  var n = 0;
  var i = 0;

  while (i < 24) {
    array[n++] = decodeLookup[string.charCodeAt(i++)] << 4 | decodeLookup[string.charCodeAt(i++)]
  }

  return new ObjectID(array);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.createFromTime"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>createFromTime (time)](#apidoc.element.mongojs.ObjectID.createFromTime)
- description and source-code
```javascript
function createFromTime(time) {
  var buffer = new Buffer([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]);
  // Encode time into first 4 bytes
  buffer[3] = time & 0xff;
  buffer[2] = (time >> 8) & 0xff;
  buffer[1] = (time >> 16) & 0xff;
  buffer[0] = (time >> 24) & 0xff;
  // Return the new objectId
  return new ObjectID(buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.createPk"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>createPk ()](#apidoc.element.mongojs.ObjectID.createPk)
- description and source-code
```javascript
function createPk() {
  return new ObjectID();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.isValid"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.</span>isValid (id)](#apidoc.element.mongojs.ObjectID.isValid)
- description and source-code
```javascript
function isValid(id) {
  if(id == null) return false;

  if(typeof id == 'number') {
    return true;
  }

  if(typeof id == 'string') {
    return id.length == 12 || (id.length == 24 && checkForHexRegExp.test(id));
  }

  if(id instanceof ObjectID) {
    return true;
  }

  if(id instanceof _Buffer) {
    return true;
  }

  // Duck-Typing detection of ObjectId like objects
  if(id.toHexString) {
    return id.id.length == 12 || (id.id.length == 24 && checkForHexRegExp.test(id.id));
  }

  return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.ObjectID.prototype"></a>[module mongojs.ObjectID.prototype](#apidoc.module.mongojs.ObjectID.prototype)

#### <a name="apidoc.element.mongojs.ObjectID.prototype.equals"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>equals (otherId)](#apidoc.element.mongojs.ObjectID.prototype.equals)
- description and source-code
```javascript
function equals(otherId) {
  var id;

  if(otherId instanceof ObjectID) {
    return this.toString() == otherId.toString();
  } else if(typeof otherId == 'string' && ObjectID.isValid(otherId) && otherId.length == 12 && this.id instanceof _Buffer) {
    return otherId === this.id.toString('binary');
  } else if(typeof otherId == 'string' && ObjectID.isValid(otherId) && otherId.length == 24) {
    return otherId.toLowerCase() === this.toHexString();
  } else if(typeof otherId == 'string' && ObjectID.isValid(otherId) && otherId.length == 12) {
    return otherId === this.id;
  } else if(otherId != null && (otherId instanceof ObjectID || otherId.toHexString)) {
    return otherId.toHexString() === this.toHexString();
  } else {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.generate"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>generate (time)](#apidoc.element.mongojs.ObjectID.prototype.generate)
- description and source-code
```javascript
generate = function (time) {
  if ('number' != typeof time) {
    time = ~~(Date.now()/1000);
  }

  // Use pid
  var pid = (typeof process === 'undefined' ? Math.floor(Math.random() * 100000) : process.pid) % 0xFFFF;
  var inc = this.get_inc();
  // Buffer used
  var buffer = new Buffer(12);
  // Encode time
  buffer[3] = time & 0xff;
  buffer[2] = (time >> 8) & 0xff;
  buffer[1] = (time >> 16) & 0xff;
  buffer[0] = (time >> 24) & 0xff;
  // Encode machine
  buffer[6] = MACHINE_ID & 0xff;
  buffer[5] = (MACHINE_ID >> 8) & 0xff;
  buffer[4] = (MACHINE_ID >> 16) & 0xff;
  // Encode pid
  buffer[8] = pid & 0xff;
  buffer[7] = (pid >> 8) & 0xff;
  // Encode index
  buffer[11] = inc & 0xff;
  buffer[10] = (inc >> 8) & 0xff;
  buffer[9] = (inc >> 16) & 0xff;
  // Return the buffer
  return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.getInc"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>getInc ()](#apidoc.element.mongojs.ObjectID.prototype.getInc)
- description and source-code
```javascript
getInc = function () {
  return this.get_inc();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.getTimestamp"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>getTimestamp ()](#apidoc.element.mongojs.ObjectID.prototype.getTimestamp)
- description and source-code
```javascript
getTimestamp = function () {
  var timestamp = new Date();
  var time = this.id[3] | this.id[2] << 8 | this.id[1] << 16 | this.id[0] << 24;
  timestamp.setTime(Math.floor(time) * 1000);
  return timestamp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.get_inc"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>get_inc ()](#apidoc.element.mongojs.ObjectID.prototype.get_inc)
- description and source-code
```javascript
get_inc = function () {
  return ObjectID.index = (ObjectID.index + 1) % 0xFFFFFF;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.inspect"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>inspect (format)](#apidoc.element.mongojs.ObjectID.prototype.inspect)
- description and source-code
```javascript
inspect = function (format) {
  // Is the id a buffer then use the buffer toString method to return the format
  if(this.id && this.id.copy) {
    return this.id.toString(typeof format === 'string' ? format : 'hex');
  }

  // if(this.buffer )
  return this.toHexString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.toHexString"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>toHexString ()](#apidoc.element.mongojs.ObjectID.prototype.toHexString)
- description and source-code
```javascript
toHexString = function () {
  if(ObjectID.cacheHexString && this.__id) return this.__id;

  var hexString = '';
  if(!this.id || !this.id.length) {
    throw new Error('invalid ObjectId, ObjectId.id must be either a string or a Buffer, but is [' + JSON.stringify(this.id) + ']');
  }

  if(this.id instanceof _Buffer) {
    hexString = convertToHex(this.id);
    if(ObjectID.cacheHexString) this.__id = hexString;
    return hexString;
  }

  for (var i = 0; i < this.id.length; i++) {
    hexString += hexTable[this.id.charCodeAt(i)];
  }

  if(ObjectID.cacheHexString) this.__id = hexString;
  return hexString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>toJSON ()](#apidoc.element.mongojs.ObjectID.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toHexString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.ObjectID.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.ObjectID.prototype.</span>toString (format)](#apidoc.element.mongojs.ObjectID.prototype.toString)
- description and source-code
```javascript
toString = function (format) {
  // Is the id a buffer then use the buffer toString method to return the format
  if(this.id && this.id.copy) {
    return this.id.toString(typeof format === 'string' ? format : 'hex');
  }

  // if(this.buffer )
  return this.toHexString();
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```



# <a name="apidoc.module.mongojs.Symbol"></a>[module mongojs.Symbol](#apidoc.module.mongojs.Symbol)

#### <a name="apidoc.element.mongojs.Symbol.Symbol"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Symbol (value)](#apidoc.element.mongojs.Symbol.Symbol)
- description and source-code
```javascript
function Symbol(value) {
  if(!(this instanceof Symbol)) return new Symbol(value);
  this._bsontype = 'Symbol';
  this.value = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Symbol.prototype"></a>[module mongojs.Symbol.prototype](#apidoc.module.mongojs.Symbol.prototype)

#### <a name="apidoc.element.mongojs.Symbol.prototype.inspect"></a>[function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>inspect ()](#apidoc.element.mongojs.Symbol.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Symbol.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>toJSON ()](#apidoc.element.mongojs.Symbol.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Symbol.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>toString ()](#apidoc.element.mongojs.Symbol.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.value;
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```

#### <a name="apidoc.element.mongojs.Symbol.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">mongojs.Symbol.prototype.</span>valueOf ()](#apidoc.element.mongojs.Symbol.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Timestamp"></a>[module mongojs.Timestamp](#apidoc.module.mongojs.Timestamp)

#### <a name="apidoc.element.mongojs.Timestamp.Timestamp"></a>[function <span class="apidocSignatureSpan">mongojs.</span>Timestamp (low, high)](#apidoc.element.mongojs.Timestamp.Timestamp)
- description and source-code
```javascript
function Timestamp(low, high) {
  if(!(this instanceof Timestamp)) return new Timestamp(low, high);
  this._bsontype = 'Timestamp';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.fromBits"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromBits (lowBits, highBits)](#apidoc.element.mongojs.Timestamp.fromBits)
- description and source-code
```javascript
fromBits = function (lowBits, highBits) {
  return new Timestamp(lowBits, highBits);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.fromInt"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromInt (value)](#apidoc.element.mongojs.Timestamp.fromInt)
- description and source-code
```javascript
fromInt = function (value) {
  if (-128 <= value && value < 128) {
    var cachedObj = Timestamp.INT_CACHE_[value];
    if (cachedObj) {
      return cachedObj;
    }
  }

  var obj = new Timestamp(value | 0, value < 0 ? -1 : 0);
  if (-128 <= value && value < 128) {
    Timestamp.INT_CACHE_[value] = obj;
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.fromNumber"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromNumber (value)](#apidoc.element.mongojs.Timestamp.fromNumber)
- description and source-code
```javascript
fromNumber = function (value) {
  if (isNaN(value) || !isFinite(value)) {
    return Timestamp.ZERO;
  } else if (value <= -Timestamp.TWO_PWR_63_DBL_) {
    return Timestamp.MIN_VALUE;
  } else if (value + 1 >= Timestamp.TWO_PWR_63_DBL_) {
    return Timestamp.MAX_VALUE;
  } else if (value < 0) {
    return Timestamp.fromNumber(-value).negate();
  } else {
    return new Timestamp(
               (value % Timestamp.TWO_PWR_32_DBL_) | 0,
               (value / Timestamp.TWO_PWR_32_DBL_) | 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.fromString"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.</span>fromString (str, opt_radix)](#apidoc.element.mongojs.Timestamp.fromString)
- description and source-code
```javascript
fromString = function (str, opt_radix) {
  if (str.length == 0) {
    throw Error('number format error: empty string');
  }

  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (str.charAt(0) == '-') {
    return Timestamp.fromString(str.substring(1), radix).negate();
  } else if (str.indexOf('-') >= 0) {
    throw Error('number format error: interior "-" character: ' + str);
  }

  // Do several (8) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Timestamp.fromNumber(Math.pow(radix, 8));

  var result = Timestamp.ZERO;
  for (var i = 0; i < str.length; i += 8) {
    var size = Math.min(8, str.length - i);
    var value = parseInt(str.substring(i, i + size), radix);
    if (size < 8) {
      var power = Timestamp.fromNumber(Math.pow(radix, size));
      result = result.multiply(power).add(Timestamp.fromNumber(value));
    } else {
      result = result.multiply(radixToPower);
      result = result.add(Timestamp.fromNumber(value));
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.Timestamp.prototype"></a>[module mongojs.Timestamp.prototype](#apidoc.module.mongojs.Timestamp.prototype)

#### <a name="apidoc.element.mongojs.Timestamp.prototype.add"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>add (other)](#apidoc.element.mongojs.Timestamp.prototype.add)
- description and source-code
```javascript
add = function (other) {
  // Divide each number into 4 chunks of 16 bits, and then sum the chunks.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 + b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 + b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 + b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 + b48;
  c48 &= 0xFFFF;
  return Timestamp.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.and"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>and (other)](#apidoc.element.mongojs.Timestamp.prototype.and)
- description and source-code
```javascript
and = function (other) {
  return Timestamp.fromBits(this.low_ & other.low_, this.high_ & other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.compare"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>compare (other)](#apidoc.element.mongojs.Timestamp.prototype.compare)
- description and source-code
```javascript
compare = function (other) {
  if (this.equals(other)) {
    return 0;
  }

  var thisNeg = this.isNegative();
  var otherNeg = other.isNegative();
  if (thisNeg && !otherNeg) {
    return -1;
  }
  if (!thisNeg && otherNeg) {
    return 1;
  }

  // at this point, the signs are the same, so subtraction will not overflow
  if (this.subtract(other).isNegative()) {
    return -1;
  } else {
    return 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.div"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>div (other)](#apidoc.element.mongojs.Timestamp.prototype.div)
- description and source-code
```javascript
div = function (other) {
  if (other.isZero()) {
    throw Error('division by zero');
  } else if (this.isZero()) {
    return Timestamp.ZERO;
  }

  if (this.equals(Timestamp.MIN_VALUE)) {
    if (other.equals(Timestamp.ONE) ||
        other.equals(Timestamp.NEG_ONE)) {
      return Timestamp.MIN_VALUE;  // recall that -MIN_VALUE == MIN_VALUE
    } else if (other.equals(Timestamp.MIN_VALUE)) {
      return Timestamp.ONE;
    } else {
      // At this point, we have |other| >= 2, so |this/other| < |MIN_VALUE|.
      var halfThis = this.shiftRight(1);
      var approx = halfThis.div(other).shiftLeft(1);
      if (approx.equals(Timestamp.ZERO)) {
        return other.isNegative() ? Timestamp.ONE : Timestamp.NEG_ONE;
      } else {
        var rem = this.subtract(other.multiply(approx));
        var result = approx.add(rem.div(other));
        return result;
      }
    }
  } else if (other.equals(Timestamp.MIN_VALUE)) {
    return Timestamp.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().div(other.negate());
    } else {
      return this.negate().div(other).negate();
    }
  } else if (other.isNegative()) {
    return this.div(other.negate()).negate();
  }

  // Repeat the following until the remainder is less than other:  find a
  // floating-point that approximates remainder / other *from below*, add this
  // into the result, and subtract it from the remainder.  It is critical that
  // the approximate value is less than or equal to the real value so that the
  // remainder never becomes negative.
  var res = Timestamp.ZERO;
  var rem = this;
  while (rem.greaterThanOrEqual(other)) {
    // Approximate the result of division. This may be a little greater or
    // smaller than the actual value.
    var approx = Math.max(1, Math.floor(rem.toNumber() / other.toNumber()));

    // We will tweak the approximate result by changing it in the 48-th digit or
    // the smallest non-fractional digit, whichever is larger.
    var log2 = Math.ceil(Math.log(approx) / Math.LN2);
    var delta = (log2 <= 48) ? 1 : Math.pow(2, log2 - 48);

    // Decrease the approximation until it is smaller than the remainder.  Note
    // that if it is too large, the product overflows and is negative.
    var approxRes = Timestamp.fromNumber(approx);
    var approxRem = approxRes.multiply(other);
    while (approxRem.isNegative() || approxRem.greaterThan(rem)) {
      approx -= delta;
      approxRes = Timestamp.fromNumber(approx);
      approxRem = approxRes.multiply(other);
    }

    // We know the answer can't be zero... and actually, zero would cause
    // infinite recursion since we would make no progress.
    if (approxRes.isZero()) {
      approxRes = Timestamp.ONE;
    }

    res = res.add(approxRes);
    rem = rem.subtract(approxRem);
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.equals"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>equals (other)](#apidoc.element.mongojs.Timestamp.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return (this.high_ == other.high_) && (this.low_ == other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.getHighBits"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getHighBits ()](#apidoc.element.mongojs.Timestamp.prototype.getHighBits)
- description and source-code
```javascript
getHighBits = function () {
  return this.high_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.getLowBits"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getLowBits ()](#apidoc.element.mongojs.Timestamp.prototype.getLowBits)
- description and source-code
```javascript
getLowBits = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.getLowBitsUnsigned"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.mongojs.Timestamp.prototype.getLowBitsUnsigned)
- description and source-code
```javascript
getLowBitsUnsigned = function () {
  return (this.low_ >= 0) ?
      this.low_ : Timestamp.TWO_PWR_32_DBL_ + this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.getNumBitsAbs"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>getNumBitsAbs ()](#apidoc.element.mongojs.Timestamp.prototype.getNumBitsAbs)
- description and source-code
```javascript
getNumBitsAbs = function () {
  if (this.isNegative()) {
    if (this.equals(Timestamp.MIN_VALUE)) {
      return 64;
    } else {
      return this.negate().getNumBitsAbs();
    }
  } else {
    var val = this.high_ != 0 ? this.high_ : this.low_;
    for (var bit = 31; bit > 0; bit--) {
      if ((val & (1 << bit)) != 0) {
        break;
      }
    }
    return this.high_ != 0 ? bit + 33 : bit + 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.greaterThan"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>greaterThan (other)](#apidoc.element.mongojs.Timestamp.prototype.greaterThan)
- description and source-code
```javascript
greaterThan = function (other) {
  return this.compare(other) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.greaterThanOrEqual"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.mongojs.Timestamp.prototype.greaterThanOrEqual)
- description and source-code
```javascript
greaterThanOrEqual = function (other) {
  return this.compare(other) >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.isNegative"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>isNegative ()](#apidoc.element.mongojs.Timestamp.prototype.isNegative)
- description and source-code
```javascript
isNegative = function () {
  return this.high_ < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.isOdd"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>isOdd ()](#apidoc.element.mongojs.Timestamp.prototype.isOdd)
- description and source-code
```javascript
isOdd = function () {
  return (this.low_ & 1) == 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.isZero"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>isZero ()](#apidoc.element.mongojs.Timestamp.prototype.isZero)
- description and source-code
```javascript
isZero = function () {
  return this.high_ == 0 && this.low_ == 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.lessThan"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>lessThan (other)](#apidoc.element.mongojs.Timestamp.prototype.lessThan)
- description and source-code
```javascript
lessThan = function (other) {
  return this.compare(other) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.lessThanOrEqual"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>lessThanOrEqual (other)](#apidoc.element.mongojs.Timestamp.prototype.lessThanOrEqual)
- description and source-code
```javascript
lessThanOrEqual = function (other) {
  return this.compare(other) <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.modulo"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>modulo (other)](#apidoc.element.mongojs.Timestamp.prototype.modulo)
- description and source-code
```javascript
modulo = function (other) {
  return this.subtract(this.div(other).multiply(other));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.multiply"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>multiply (other)](#apidoc.element.mongojs.Timestamp.prototype.multiply)
- description and source-code
```javascript
multiply = function (other) {
  if (this.isZero()) {
    return Timestamp.ZERO;
  } else if (other.isZero()) {
    return Timestamp.ZERO;
  }

  if (this.equals(Timestamp.MIN_VALUE)) {
    return other.isOdd() ? Timestamp.MIN_VALUE : Timestamp.ZERO;
  } else if (other.equals(Timestamp.MIN_VALUE)) {
    return this.isOdd() ? Timestamp.MIN_VALUE : Timestamp.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().multiply(other.negate());
    } else {
      return this.negate().multiply(other).negate();
    }
  } else if (other.isNegative()) {
    return this.multiply(other.negate()).negate();
  }

  // If both Timestamps are small, use float multiplication
  if (this.lessThan(Timestamp.TWO_PWR_24_) &&
      other.lessThan(Timestamp.TWO_PWR_24_)) {
    return Timestamp.fromNumber(this.toNumber() * other.toNumber());
  }

  // Divide each Timestamp into 4 chunks of 16 bits, and then add up 4x4 products.
  // We can skip products that would overflow.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 * b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 * b00;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c16 += a00 * b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 * b00;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a16 * b16;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a00 * b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 * b00 + a32 * b16 + a16 * b32 + a00 * b48;
  c48 &= 0xFFFF;
  return Timestamp.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.negate"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>negate ()](#apidoc.element.mongojs.Timestamp.prototype.negate)
- description and source-code
```javascript
negate = function () {
  if (this.equals(Timestamp.MIN_VALUE)) {
    return Timestamp.MIN_VALUE;
  } else {
    return this.not().add(Timestamp.ONE);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.not"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>not ()](#apidoc.element.mongojs.Timestamp.prototype.not)
- description and source-code
```javascript
not = function () {
  return Timestamp.fromBits(~this.low_, ~this.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.notEquals"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>notEquals (other)](#apidoc.element.mongojs.Timestamp.prototype.notEquals)
- description and source-code
```javascript
notEquals = function (other) {
  return (this.high_ != other.high_) || (this.low_ != other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.or"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>or (other)](#apidoc.element.mongojs.Timestamp.prototype.or)
- description and source-code
```javascript
or = function (other) {
  return Timestamp.fromBits(this.low_ | other.low_, this.high_ | other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.shiftLeft"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>shiftLeft (numBits)](#apidoc.element.mongojs.Timestamp.prototype.shiftLeft)
- description and source-code
```javascript
shiftLeft = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var low = this.low_;
    if (numBits < 32) {
      var high = this.high_;
      return Timestamp.fromBits(
                 low << numBits,
                 (high << numBits) | (low >>> (32 - numBits)));
    } else {
      return Timestamp.fromBits(0, low << (numBits - 32));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.shiftRight"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>shiftRight (numBits)](#apidoc.element.mongojs.Timestamp.prototype.shiftRight)
- description and source-code
```javascript
shiftRight = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Timestamp.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >> numBits);
    } else {
      return Timestamp.fromBits(
                 high >> (numBits - 32),
                 high >= 0 ? 0 : -1);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.shiftRightUnsigned"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.mongojs.Timestamp.prototype.shiftRightUnsigned)
- description and source-code
```javascript
shiftRightUnsigned = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Timestamp.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >>> numBits);
    } else if (numBits == 32) {
      return Timestamp.fromBits(high, 0);
    } else {
      return Timestamp.fromBits(high >>> (numBits - 32), 0);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.subtract"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>subtract (other)](#apidoc.element.mongojs.Timestamp.prototype.subtract)
- description and source-code
```javascript
subtract = function (other) {
  return this.add(other.negate());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.toInt"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toInt ()](#apidoc.element.mongojs.Timestamp.prototype.toInt)
- description and source-code
```javascript
toInt = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toJSON ()](#apidoc.element.mongojs.Timestamp.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.toNumber"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toNumber ()](#apidoc.element.mongojs.Timestamp.prototype.toNumber)
- description and source-code
```javascript
toNumber = function () {
  return this.high_ * Timestamp.TWO_PWR_32_DBL_ +
         this.getLowBitsUnsigned();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>toString (opt_radix)](#apidoc.element.mongojs.Timestamp.prototype.toString)
- description and source-code
```javascript
toString = function (opt_radix) {
  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (this.isZero()) {
    return '0';
  }

  if (this.isNegative()) {
    if (this.equals(Timestamp.MIN_VALUE)) {
      // We need to change the Timestamp value before it can be negated, so we remove
      // the bottom-most digit in this base and then recurse to do the rest.
      var radixTimestamp = Timestamp.fromNumber(radix);
      var div = this.div(radixTimestamp);
      var rem = div.multiply(radixTimestamp).subtract(this);
      return div.toString(radix) + rem.toInt().toString(radix);
    } else {
      return '-' + this.negate().toString(radix);
    }
  }

  // Do several (6) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Timestamp.fromNumber(Math.pow(radix, 6));

  var rem = this;
  var result = '';
  while (true) {
    var remDiv = rem.div(radixToPower);
    var intval = rem.subtract(remDiv.multiply(radixToPower)).toInt();
    var digits = intval.toString(radix);

    rem = remDiv;
    if (rem.isZero()) {
      return digits + result;
    } else {
      while (digits.length < 6) {
        digits = '0' + digits;
      }
      result = '' + digits + result;
    }
  }
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```

#### <a name="apidoc.element.mongojs.Timestamp.prototype.xor"></a>[function <span class="apidocSignatureSpan">mongojs.Timestamp.prototype.</span>xor (other)](#apidoc.element.mongojs.Timestamp.prototype.xor)
- description and source-code
```javascript
xor = function (other) {
  return Timestamp.fromBits(this.low_ ^ other.low_, this.high_ ^ other.high_);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.bulk"></a>[module mongojs.bulk](#apidoc.module.mongojs.bulk)

#### <a name="apidoc.element.mongojs.bulk.bulk"></a>[function <span class="apidocSignatureSpan">mongojs.</span>bulk (colName, ordered, onserver)](#apidoc.element.mongojs.bulk.bulk)
- description and source-code
```javascript
bulk = function (colName, ordered, onserver) {
  this._colname = colName
  this._cmds = []
  this._currCmd = null
  this._ordered = ordered
  this._getConnection = onserver

  var self = this
  this.find = function (query) {
    var upsert = false
    var findobj = {}
    var remove = function (lim) {
      if (!self._currCmd) {
        self._currCmd = {
          delete: self._colname,
          deletes: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      if (!self._currCmd.delete) {
        self._cmds.push(self._currCmd)
        self._currCmd = {
          delete: self._colname,
          deletes: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      self._currCmd.deletes.push({q: query, limit: lim})
    }

    var update = function (updObj, multi) {
      if (!self._currCmd) {
        self._currCmd = {
          update: self._colname,
          updates: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      if (!self._currCmd.update) {
        self._cmds.push(self._currCmd)
        self._currCmd = {
          update: self._colname,
          updates: [],
          ordered: self._ordered,
          writeConcern: {w: 1}
        }
      }
      self._currCmd.updates.push({q: query, u: updObj, multi: multi, upsert: upsert})
    }

    findobj.upsert = function () {
      upsert = true
      return findobj
    }

    findobj.remove = function () {
      remove(0)
    }

    findobj.removeOne = function () {
      remove(1)
    }

    findobj.update = function (updObj) {
      update(updObj, true)
    }

    findobj.updateOne = function (updObj) {
      update(updObj, false)
    }

    findobj.replaceOne = function (updObj) {
      this.updateOne(updObj)
    }

    return findobj
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.bulk.prototype"></a>[module mongojs.bulk.prototype](#apidoc.module.mongojs.bulk.prototype)

#### <a name="apidoc.element.mongojs.bulk.prototype.execute"></a>[function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>execute (cb)](#apidoc.element.mongojs.bulk.prototype.execute)
- description and source-code
```javascript
execute = function (cb) {
  if (!cb) return this.execute(noop)

  var self = this
  var result = {
    writeErrors: [ ],
    writeConcernErrors: [ ],
    nInserted: 0,
    nUpserted: 0,
    nMatched: 0,
    nModified: 0,
    nRemoved: 0,
    upserted: [ ]
  }

  if (this._currCmd) {
    this._cmds.push(this._currCmd)
  }

  this._getConnection(function (err, connection) {
    if (err) return cb(err)
    each(self._cmds, function (cmd, i, done) {
      connection.command(cmd, function (err, res) {
        if (err) return done(err)
        result[cmdkeys[Object.keys(cmd)[0]]] += res.n
        done()
      })
    }, function (err) {
      if (err) return cb(err)
      result.ok = 1
      cb(null, result)
    })
  })
}
```
- example usage
```shell
...
bulk.insert({name: 'Spearow', type: 'flying'})
bulk.insert({name: 'Pidgeotto', type: 'flying'})
bulk.insert({name: 'Charmeleon', type: 'fire'})
bulk.find({type: 'flying'}).removeOne()
bulk.find({type: 'fire'}).remove()
bulk.find({type: 'water'}).updateOne({$set: {hp: 100}})

bulk.execute(function (err, res) {
  console.log('Done!')
})
'''

## Replication Sets

Mongojs can also connect to a mongo replication set by providing a connection string with multiple hosts
...
```

#### <a name="apidoc.element.mongojs.bulk.prototype.insert"></a>[function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>insert (doc)](#apidoc.element.mongojs.bulk.prototype.insert)
- description and source-code
```javascript
insert = function (doc) {
  if (!this._currCmd) {
    this._currCmd = {
      insert: this._colname,
      documents: [],
      ordered: this._ordered,
      writeConcern: {w: 1}
    }
  }
  if (!this._currCmd.insert) {
    this._cmds.push(this._currCmd)
    this._currCmd = {
      insert: this._colname,
      documents: [],
      ordered: this._ordered,
      writeConcern: {w: 1}
    }
  }
  if (!doc._id) doc._id = oid()
  this._currCmd.documents.push(doc)
}
```
- example usage
```shell
...

As of 0.15 mongojs supports the Bulk updates introduced in mongodb 2.6. Here's an example of the usage

'''js
var bulk = db.a.initializeOrderedBulkOp()
bulk.find({type: 'water'}).update({$set: {level: 1}})
bulk.find({type: 'water'}).update({$inc: {level: 2}})
bulk.insert({name: 'Spearow', type: 'flying'})
bulk.insert({name: 'Pidgeotto', type: 'flying'})
bulk.insert({name: 'Charmeleon', type: 'fire'})
bulk.find({type: 'flying'}).removeOne()
bulk.find({type: 'fire'}).remove()
bulk.find({type: 'water'}).updateOne({$set: {hp: 100}})

bulk.execute(function (err, res) {
...
```

#### <a name="apidoc.element.mongojs.bulk.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>toString ()](#apidoc.element.mongojs.bulk.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify(this.tojson())
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```

#### <a name="apidoc.element.mongojs.bulk.prototype.tojson"></a>[function <span class="apidocSignatureSpan">mongojs.bulk.prototype.</span>tojson ()](#apidoc.element.mongojs.bulk.prototype.tojson)
- description and source-code
```javascript
tojson = function () {
  if (this._currCmd) this._cmds.push(this._currCmd)

  var obj = {
    nInsertOps: 0,
    nUpdateOps: 0,
    nRemoveOps: 0,
    nBatches: this._cmds.length
  }

  this._cmds.forEach(function (cmd) {
    if (cmd.update) {
      obj.nUpdateOps += cmd.updates.length
    } else if (cmd.insert) {
      obj.nInsertOps += cmd.documents.length
    } else if (cmd.delete) {
      obj.nRemoveOps += cmd.deletes.length
    }
  })

  return obj
}
```
- example usage
```shell
...

#####'bulk.find.upsert(upsertParam)'

#####'bulk.insert(document)'

#####'bulk.toString()'

#####'bulk.tojson()'
...
```



# <a name="apidoc.module.mongojs.collection"></a>[module mongojs.collection](#apidoc.module.mongojs.collection)

#### <a name="apidoc.element.mongojs.collection.collection"></a>[function <span class="apidocSignatureSpan">mongojs.</span>collection (opts, getConnection)](#apidoc.element.mongojs.collection.collection)
- description and source-code
```javascript
collection = function (opts, getConnection) {
  this._name = opts.name
  this._getConnection = getConnection
  this._getCollection = function (cb) {
    var collectionName = this._name

    this._getConnection(function (err, connection) {
      if (err) { return cb(err) }

      cb(null, connection.collection(collectionName))
    })
  }
}
```
- example usage
```shell
...
var db = mongojs('username:password@example.com/mydb?authSource=authdb', ['mycollection'])

// connect with options
var db = mongojs('username:password@example.com/mydb', ['mycollection'], { ssl: true })

// connect now, and worry about collections later
var db = mongojs('mydb')
var mycollection = db.collection('mycollection')
'''

[More connection string examples](http://mongodb.github.io/node-mongodb-native/2.0/reference/connecting/)

After we connected we can query or update the database just how we would using the mongo API with the exception that we use a callback
.
The format for callbacks is always 'callback(error, value)' where error is null if no exception has occured. The update methods '
save', 'remove', 'update' and 'findAndModify' also pass the 'lastErrorObject' as the last argument to the callback function.
...
```



# <a name="apidoc.module.mongojs.collection.prototype"></a>[module mongojs.collection.prototype](#apidoc.module.mongojs.collection.prototype)

#### <a name="apidoc.element.mongojs.collection.prototype.aggregate"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>aggregate ()](#apidoc.element.mongojs.collection.prototype.aggregate)
- description and source-code
```javascript
aggregate = function () {
  var cb
  var opts

  var pipeline = Array.prototype.slice.call(arguments)
  if (typeof pipeline[pipeline.length - 1] === 'function') {
    cb = once(pipeline.pop())
  }

  if ((pipeline.length === 1 || pipeline.length === 2) && Array.isArray(pipeline[0])) {
    opts = pipeline[1]
    pipeline = pipeline[0]
  }

  var self = this

  var strm = new Cursor(function (cb) {
    self._getCollection(function (err, collection) {
      if (err) return cb(err)

      cb(null, collection.aggregate(pipeline, opts))
    })
  })

  if (cb) {
    return strm.toArray(cb)
  }

  return strm
}
```
- example usage
```shell
...

# API

This API documentation is a work in progress.

#### Collection

#####'db.collection.aggregate([pipeline], [options], [callback])'
https://docs.mongodb.org/manual/reference/method/db.collection.aggregate/

#####'db.collection.aggregate([pipelineStep], [pipelineStep], [pipelineStep], ..., [callback])'

#####'db.collection.count([query], callback)'

#####'db.collection.createIndex(keys, options, [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.count"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>count (query, cb)](#apidoc.element.mongojs.collection.prototype.count)
- description and source-code
```javascript
count = function (query, cb) {
  if (typeof query === 'function') return this.count({}, query)
  this.find(query).count(cb)
}
```
- example usage
```shell
...
#### Collection

#####'db.collection.aggregate([pipeline], [options], [callback])'
https://docs.mongodb.org/manual/reference/method/db.collection.aggregate/

#####'db.collection.aggregate([pipelineStep], [pipelineStep], [pipelineStep], ..., [callback])'

#####'db.collection.count([query], callback)'

#####'db.collection.createIndex(keys, options, [callback])'

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.createIndex"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>createIndex (index, opts, cb)](#apidoc.element.mongojs.collection.prototype.createIndex)
- description and source-code
```javascript
createIndex = function (index, opts, cb) {
  if (typeof opts === 'function') return this.createIndex(index, {}, opts)
  if (!opts) return this.createIndex(index, {}, noop)
  if (!cb) return this.createIndex(index, opts, noop)

  this._getCollection(function (err, collection) {
    if (err) return cb(err)

    collection.createIndex(index, opts, cb)
  })
}
```
- example usage
```shell
...
#####'db.collection.aggregate([pipeline], [options], [callback])'
https://docs.mongodb.org/manual/reference/method/db.collection.aggregate/

#####'db.collection.aggregate([pipelineStep], [pipelineStep], [pipelineStep], ..., [callback])'

#####'db.collection.count([query], callback)'

#####'db.collection.createIndex(keys, options, [callback])'

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'

#####'db.collection.dropIndex(index, [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.distinct"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>distinct (field, query, cb)](#apidoc.element.mongojs.collection.prototype.distinct)
- description and source-code
```javascript
distinct = function (field, query, cb) {
  this.runCommand('distinct', {key: field, query: query}, function (err, result) {
    if (err) return cb(err)
    cb(null, result.values)
  })
}
```
- example usage
```shell
...

#####'db.collection.aggregate([pipelineStep], [pipelineStep], [pipelineStep], ..., [callback])'

#####'db.collection.count([query], callback)'

#####'db.collection.createIndex(keys, options, [callback])'

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'

#####'db.collection.dropIndex(index, [callback])'

#####'db.collection.dropIndexes([callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.drop"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>drop (cb)](#apidoc.element.mongojs.collection.prototype.drop)
- description and source-code
```javascript
drop = function (cb) {
  this.runCommand('drop', cb)
}
```
- example usage
```shell
...

#####'db.collection.count([query], callback)'

#####'db.collection.createIndex(keys, options, [callback])'

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'

#####'db.collection.dropIndex(index, [callback])'

#####'db.collection.dropIndexes([callback])'

#####'db.collection.ensureIndex(keys, options, [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.dropIndex"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>dropIndex (index, cb)](#apidoc.element.mongojs.collection.prototype.dropIndex)
- description and source-code
```javascript
dropIndex = function (index, cb) {
  this.runCommand('dropIndexes', {index: index}, cb)
}
```
- example usage
```shell
...

#####'db.collection.createIndex(keys, options, [callback])'

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'

#####'db.collection.dropIndex(index, [callback])'

#####'db.collection.dropIndexes([callback])'

#####'db.collection.ensureIndex(keys, options, [callback])'

#####'db.collection.find([criteria], [projection], [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.dropIndexes"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>dropIndexes (cb)](#apidoc.element.mongojs.collection.prototype.dropIndexes)
- description and source-code
```javascript
dropIndexes = function (cb) {
  this.runCommand('dropIndexes', {index: '*'}, cb)
}
```
- example usage
```shell
...

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'

#####'db.collection.dropIndex(index, [callback])'

#####'db.collection.dropIndexes([callback])'

#####'db.collection.ensureIndex(keys, options, [callback])'

#####'db.collection.find([criteria], [projection], [callback])'

This function applies a query to a collection. You can get the return value, which is a cursor, or pass a callback
as the last parameter. Said callback receives '(err, documents)'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.ensureIndex"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>ensureIndex (index, opts, cb)](#apidoc.element.mongojs.collection.prototype.ensureIndex)
- description and source-code
```javascript
ensureIndex = function (index, opts, cb) {
  if (typeof opts === 'function') return this.ensureIndex(index, {}, opts)
  if (!opts) return this.ensureIndex(index, {}, noop)
  if (!cb) return this.ensureIndex(index, opts, noop)

  this._getCollection(function (err, collection) {
    if (err) return cb(err)

    collection.ensureIndex(index, opts, cb)
  })
}
```
- example usage
```shell
...

#####'db.collection.drop([callback])'

#####'db.collection.dropIndex(index, [callback])'

#####'db.collection.dropIndexes([callback])'

#####'db.collection.ensureIndex(keys, options, [callback])'

#####'db.collection.find([criteria], [projection], [callback])'

This function applies a query to a collection. You can get the return value, which is a cursor, or pass a callback
as the last parameter. Said callback receives '(err, documents)'

#####'db.collection.findOne([criteria], [projection], callback)'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.find"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>find (query, projection, opts, cb)](#apidoc.element.mongojs.collection.prototype.find)
- description and source-code
```javascript
find = function (query, projection, opts, cb) {
  if (typeof query === 'function') return this.find({}, null, null, query)
  if (typeof projection === 'function') return this.find(query, null, null, projection)
  if (typeof opts === 'function') return this.find(query, projection, null, opts)

  var self = this
  function getCursor (cb) {
    self._getCollection(function (err, collection) {
      if (err) { return cb(err) }

      cb(null, collection.find(query, projection, opts))
    })
  }

  var cursor = new Cursor(getCursor)

  if (cb) return cursor.toArray(cb)
  return cursor
}
```
- example usage
```shell
...
[More connection string examples](http://mongodb.github.io/node-mongodb-native/2.0/reference/connecting/)

After we connected we can query or update the database just how we would using the mongo API with the exception that we use a callback
.
The format for callbacks is always 'callback(error, value)' where error is null if no exception has occured. The update methods '
save', 'remove', 'update' and 'findAndModify' also pass the 'lastErrorObject' as the last argument to the callback function.

'''js
// find everything
db.mycollection.find(function (err, docs) {
	// docs is an array of all the documents in mycollection
})

// find everything, but sort by name
db.mycollection.find().sort({name: 1}, function (err, docs) {
	// docs is now a sorted array
})
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.findAndModify"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>findAndModify (opts, cb)](#apidoc.element.mongojs.collection.prototype.findAndModify)
- description and source-code
```javascript
findAndModify = function (opts, cb) {
  this.runCommand('findAndModify', opts, function (err, result) {
    if (err) return cb(err)
    cb(null, result.value, result.lastErrorObject || {n: 0})
  })
}
```
- example usage
```shell
...

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})

// find one named 'mathias', tag him as a contributor and return the modified doc
db.mycollection.findAndModify({
	query: { name: 'mathias' },
	update: { $set: { tag: 'maintainer' } },
	new: true
}, function (err, doc, lastErrorObject) {
	// doc.tag === 'maintainer'
})
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.findOne"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>findOne (query, projection, cb)](#apidoc.element.mongojs.collection.prototype.findOne)
- description and source-code
```javascript
findOne = function (query, projection, cb) {
  if (typeof query === 'function') return this.findOne({}, null, query)
  if (typeof projection === 'function') return this.findOne(query, null, projection)
  this.find(query, projection).next(function (err, doc) {
    if (err) return cb(err)
    cb(null, doc)
  })
}
```
- example usage
```shell
...
		// we visited all docs in the collection
		return
	}
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.getIndexes"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>getIndexes (cb)](#apidoc.element.mongojs.collection.prototype.getIndexes)
- description and source-code
```javascript
getIndexes = function (cb) {
  this._getCollection(function (err, collection) {
    if (err) { return cb(err) }

    collection.indexes(cb)
  })
}
```
- example usage
```shell
...

#####'db.collection.findOne([criteria], [projection], callback)'

Apply a query and get one single document passed as a callback. The callback receives '(err, document)'

#####'db.collection.findAndModify(document, callback)'

#####'db.collection.getIndexes(callback)'

#####'db.collection.group(document, callback)'

#####'db.collection.insert(docOrDocs, [callback])'

#####'db.collection.isCapped(callback)'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.group"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>group (doc, cb)](#apidoc.element.mongojs.collection.prototype.group)
- description and source-code
```javascript
group = function (doc, cb) {
  this._getCollection(function (err, collection) {
    if (err) return cb(err)
    collection.group(doc.key || doc.keyf, doc.cond, doc.initial, doc.reduce, doc.finalize, cb)
  })
}
```
- example usage
```shell
...

Apply a query and get one single document passed as a callback. The callback receives '(err, document)'

#####'db.collection.findAndModify(document, callback)'

#####'db.collection.getIndexes(callback)'

#####'db.collection.group(document, callback)'

#####'db.collection.insert(docOrDocs, [callback])'

#####'db.collection.isCapped(callback)'

#####'db.collection.mapReduce(map, reduce, options, [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.initializeOrderedBulkOp"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>initializeOrderedBulkOp ()](#apidoc.element.mongojs.collection.prototype.initializeOrderedBulkOp)
- description and source-code
```javascript
initializeOrderedBulkOp = function () {
  return new Bulk(this._name, true, this._getConnection, this._dbname)
}
```
- example usage
```shell
...
'''

## Bulk updates

As of 0.15 mongojs supports the Bulk updates introduced in mongodb 2.6. Here's an example of the usage

'''js
var bulk = db.a.initializeOrderedBulkOp()
bulk.find({type: 'water'}).update({$set: {level: 1}})
bulk.find({type: 'water'}).update({$inc: {level: 2}})
bulk.insert({name: 'Spearow', type: 'flying'})
bulk.insert({name: 'Pidgeotto', type: 'flying'})
bulk.insert({name: 'Charmeleon', type: 'fire'})
bulk.find({type: 'flying'}).removeOne()
bulk.find({type: 'fire'}).remove()
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.initializeUnorderedBulkOp"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>initializeUnorderedBulkOp ()](#apidoc.element.mongojs.collection.prototype.initializeUnorderedBulkOp)
- description and source-code
```javascript
initializeUnorderedBulkOp = function () {
  return new Bulk(this._name, false, this._getConnection, this._dbname)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.collection.prototype.insert"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>insert (docOrDocs, opts, cb)](#apidoc.element.mongojs.collection.prototype.insert)
- description and source-code
```javascript
insert = function (docOrDocs, opts, cb) {
  if (!opts && !cb) return this.insert(docOrDocs, {}, noop)
  if (typeof opts === 'function') return this.insert(docOrDocs, {}, opts)
  if (opts && !cb) return this.insert(docOrDocs, opts, noop)

  this._getCollection(function (err, collection) {
    if (err) return cb(err)

    var docs = Array.isArray(docOrDocs) ? docOrDocs : [docOrDocs]
    for (var i = 0; i < docs.length; i++) {
      if (!docs[i]._id) docs[i]._id = oid()
    }

    collection.insert(docs, xtend(writeOpts, opts), function (err) {
      if (err) return cb(err)
      // TODO: Add a test for this - is this really not needed anymore?
      // if (res && res.result && res.result.writeErrors && res.result.writeErrors.length > 0) return cb(res.result.writeErrors[
0])
      cb(null, docOrDocs)
    })
  })
}
```
- example usage
```shell
...

As of 0.15 mongojs supports the Bulk updates introduced in mongodb 2.6. Here's an example of the usage

'''js
var bulk = db.a.initializeOrderedBulkOp()
bulk.find({type: 'water'}).update({$set: {level: 1}})
bulk.find({type: 'water'}).update({$inc: {level: 2}})
bulk.insert({name: 'Spearow', type: 'flying'})
bulk.insert({name: 'Pidgeotto', type: 'flying'})
bulk.insert({name: 'Charmeleon', type: 'fire'})
bulk.find({type: 'flying'}).removeOne()
bulk.find({type: 'fire'}).remove()
bulk.find({type: 'water'}).updateOne({$set: {hp: 100}})

bulk.execute(function (err, res) {
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.isCapped"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>isCapped (cb)](#apidoc.element.mongojs.collection.prototype.isCapped)
- description and source-code
```javascript
isCapped = function (cb) {
  this._getCollection(function (err, collection) {
    if (err) { return cb(err) }

    collection.isCapped(cb)
  })
}
```
- example usage
```shell
...

#####'db.collection.getIndexes(callback)'

#####'db.collection.group(document, callback)'

#####'db.collection.insert(docOrDocs, [callback])'

#####'db.collection.isCapped(callback)'

#####'db.collection.mapReduce(map, reduce, options, [callback])'

#####'db.collection.reIndex([callback])'

#####'db.collection.remove(query, [justOne], [callback])'
#####'db.collection.remove(query, [options], [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.mapReduce"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>mapReduce (map, reduce, opts, cb)](#apidoc.element.mongojs.collection.prototype.mapReduce)
- description and source-code
```javascript
mapReduce = function (map, reduce, opts, cb) {
  if (typeof opts === 'function') { return this.mapReduce(map, reduce, {}, opts) }
  if (!cb) { return this.mapReduce(map, reduce, opts, noop) }

  this._getCollection(function (err, collection) {
    if (err) return cb(err)

    collection.mapReduce(map, reduce, opts, cb)
  })
}
```
- example usage
```shell
...

#####'db.collection.group(document, callback)'

#####'db.collection.insert(docOrDocs, [callback])'

#####'db.collection.isCapped(callback)'

#####'db.collection.mapReduce(map, reduce, options, [callback])'

#####'db.collection.reIndex([callback])'

#####'db.collection.remove(query, [justOne], [callback])'
#####'db.collection.remove(query, [options], [callback])'

#####'db.collection.runCommand(command, [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.reIndex"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>reIndex (cb)](#apidoc.element.mongojs.collection.prototype.reIndex)
- description and source-code
```javascript
reIndex = function (cb) {
  this.runCommand('reIndex', cb)
}
```
- example usage
```shell
...

#####'db.collection.insert(docOrDocs, [callback])'

#####'db.collection.isCapped(callback)'

#####'db.collection.mapReduce(map, reduce, options, [callback])'

#####'db.collection.reIndex([callback])'

#####'db.collection.remove(query, [justOne], [callback])'
#####'db.collection.remove(query, [options], [callback])'

#####'db.collection.runCommand(command, [callback])'

#####'db.collection.save(doc, [options], [callback])'
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.remove"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>remove (query, opts, cb)](#apidoc.element.mongojs.collection.prototype.remove)
- description and source-code
```javascript
remove = function (query, opts, cb) {
  if (typeof query === 'function') return this.remove({}, {justOne: false}, query)
  if (typeof opts === 'function') return this.remove(query, {justOne: false}, opts)
  if (typeof opts === 'boolean') return this.remove(query, {justOne: opts}, cb)
  if (!opts) return this.remove(query, {justOne: false}, cb)
  if (!cb) return this.remove(query, opts, noop)

  this._getCollection(function (err, collection) {
    if (err) return cb(err)

    var deleteOperation = opts.justOne ? 'deleteOne' : 'deleteMany'

    collection[deleteOperation](query, xtend(writeOpts, opts), function (err, result) {
      if (err) return cb(err)
      cb(null, result.result)
    })
  })
}
```
- example usage
```shell
...
var bulk = db.a.initializeOrderedBulkOp()
bulk.find({type: 'water'}).update({$set: {level: 1}})
bulk.find({type: 'water'}).update({$inc: {level: 2}})
bulk.insert({name: 'Spearow', type: 'flying'})
bulk.insert({name: 'Pidgeotto', type: 'flying'})
bulk.insert({name: 'Charmeleon', type: 'fire'})
bulk.find({type: 'flying'}).removeOne()
bulk.find({type: 'fire'}).remove()
bulk.find({type: 'water'}).updateOne({$set: {hp: 100}})

bulk.execute(function (err, res) {
  console.log('Done!')
})
'''
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.rename"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>rename (name, opts, cb)](#apidoc.element.mongojs.collection.prototype.rename)
- description and source-code
```javascript
rename = function (name, opts, cb) {
  if (typeof opts === 'function') return this.rename(name, {}, opts)
  if (!opts) return this.rename(name, {}, noop)
  if (!cb) return this.rename(name, noop)

  this._getCollection(function (err, collection) {
    if (err) return cb(err)
    collection.rename(name, opts, cb)
  })
}
```
- example usage
```shell
...
    if (err) return cb(err)
    cb(null, result.result)
  })
})
}

Collection.prototype.rename = function (name, opts, cb) {
if (typeof opts === 'function') return this.rename(name, {}, opts)
if (!opts) return this.rename(name, {}, noop)
if (!cb) return this.rename(name, noop)

this._getCollection(function (err, collection) {
  if (err) return cb(err)
  collection.rename(name, opts, cb)
})
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.runCommand"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>runCommand (cmd, opts, cb)](#apidoc.element.mongojs.collection.prototype.runCommand)
- description and source-code
```javascript
runCommand = function (cmd, opts, cb) {
  if (typeof opts === 'function') return this.runCommand(cmd, null, opts)
  opts = opts || {}

  var cmdObject = {}
  cmdObject[cmd] = this._name
  Object.keys(opts).forEach(function (key) {
    cmdObject[key] = opts[key]
  })
  this._getConnection(function (err, connection) {
    if (err) return cb(err)
    connection.command(cmdObject, cb)
  })
}
```
- example usage
```shell
...
})
'''

Note that you need to explicitly set the selection parameter in the 'find' call.

## Database commands

With mongojs you can run database commands just like with the mongo shell using 'db.runCommand()'

'''js
db.runCommand({ping: 1}, function (err, res) {
	if(!err && res.ok) console.log('we\'re up')
})
'''
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.save"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>save (doc, opts, cb)](#apidoc.element.mongojs.collection.prototype.save)
- description and source-code
```javascript
save = function (doc, opts, cb) {
  if (!opts && !cb) return this.save(doc, {}, noop)
  if (typeof opts === 'function') return this.save(doc, {}, opts)
  if (!cb) return this.save(doc, opts, noop)

  if (doc._id) {
    this.update({_id: doc._id}, doc, xtend({upsert: true}, opts), function (err) {
      if (err) return cb(err)
      cb(null, doc)
    })
  } else {
    this.insert(doc, opts, cb)
  }
}
```
- example usage
```shell
...
	new: true
}, function (err, doc, lastErrorObject) {
	// doc.tag === 'maintainer'
})


// use the save function to just save a document (callback is optional for all writes)
db.mycollection.save({created: 'just now'})
'''

If you provide a callback to 'find' or any cursor config operation mongojs will call 'toArray' for you

'''js
db.mycollection.find({}, function (err, docs) { ... })
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.stats"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>stats (cb)](#apidoc.element.mongojs.collection.prototype.stats)
- description and source-code
```javascript
stats = function (cb) {
  this.runCommand('collStats', cb)
}
```
- example usage
```shell
...
#####'db.collection.remove(query, [justOne], [callback])'
#####'db.collection.remove(query, [options], [callback])'

#####'db.collection.runCommand(command, [callback])'

#####'db.collection.save(doc, [options], [callback])'

#####'db.collection.stats(callback)'

#####'db.collection.update(query, update, [options], [callback])'

#####'db.collection.toString()'

Get the name of the collection.
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>toString ()](#apidoc.element.mongojs.collection.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this._name
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```

#### <a name="apidoc.element.mongojs.collection.prototype.update"></a>[function <span class="apidocSignatureSpan">mongojs.collection.prototype.</span>update (query, update, opts, cb)](#apidoc.element.mongojs.collection.prototype.update)
- description and source-code
```javascript
update = function (query, update, opts, cb) {
  if (!opts && !cb) return this.update(query, update, {}, noop)
  if (typeof opts === 'function') return this.update(query, update, {}, opts)

  cb = cb || noop
  this._getCollection(function (err, collection) {
    if (err) return cb(err)

    collection.update(query, update, xtend(writeOpts, opts), function (err, result) {
      if (err) { return cb(err) }
      cb(null, result.result)
    })
  })
}
```
- example usage
```shell
...
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})

// find one named 'mathias', tag him as a contributor and return the modified doc
db.mycollection.findAndModify({
	query: { name: 'mathias' },
	update: { $set: { tag: 'maintainer' } },
...
```



# <a name="apidoc.module.mongojs.cursor"></a>[module mongojs.cursor](#apidoc.module.mongojs.cursor)

#### <a name="apidoc.element.mongojs.cursor.cursor"></a>[function <span class="apidocSignatureSpan">mongojs.</span>cursor (getCursor)](#apidoc.element.mongojs.cursor.cursor)
- description and source-code
```javascript
cursor = function (getCursor) {
  Readable.call(this, {objectMode: true, highWaterMark: 0})

  this._opts = {}

  var self = this
  this._get = thunky(function (cb) {
    getCursor(function (err, cursor) {
      if (err) { return cb(err) }

      // Apply all opts
      for (var key in self._opts) {
        if (self._opts.hasOwnProperty(key)) {
          cursor = cursor[key](self._opts[key])
        }
      }

      cb(null, cursor)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.super_"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.</span>super_ (options)](#apidoc.element.mongojs.cursor.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.cursor.prototype"></a>[module mongojs.cursor.prototype](#apidoc.module.mongojs.cursor.prototype)

#### <a name="apidoc.element.mongojs.cursor.prototype._read"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>_read ()](#apidoc.element.mongojs.cursor.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this
  this.next(function (err, data) {
    if (err) return self.emit('error', err)
    self.push(data)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.batchSize"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>batchSize (obj, cb)](#apidoc.element.mongojs.cursor.prototype.batchSize)
- description and source-code
```javascript
batchSize = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
...

#####'db.collection.toString()'

Get the name of the collection.

#### Cursor

#####'cursor.batchSize(size, [callback])'

#####'cursor.count(callback)'

#####'cursor.explain(callback)'

#####'cursor.forEach(function)'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.count"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>count (cb)](#apidoc.element.mongojs.cursor.prototype.count)
- description and source-code
```javascript
count = function (cb) {
  var self = this

  this._get(function (err, cursor) {
    if (err) { return cb(err) }
    cursor.count(false, self.opts, cb)
  })
}
```
- example usage
```shell
...
#### Collection

#####'db.collection.aggregate([pipeline], [options], [callback])'
https://docs.mongodb.org/manual/reference/method/db.collection.aggregate/

#####'db.collection.aggregate([pipelineStep], [pipelineStep], [pipelineStep], ..., [callback])'

#####'db.collection.count([query], callback)'

#####'db.collection.createIndex(keys, options, [callback])'

#####'db.collection.distinct(field, query, callback)'

#####'db.collection.drop([callback])'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.destroy"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>destroy ()](#apidoc.element.mongojs.cursor.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  var self = this
  this._get(function (err, cursor) {
    if (err) return self.emit('error', err)
    if (cursor.close) {
      cursor.close(function (err) {
        if (err) { self.emit('error', err) }
      })
    }
  })
}
```
- example usage
```shell
...

#####'cursor.sort(sortOptions, [callback])'

#####'cursor.toArray(callback)'

#####'cursor.rewind()'

#####'cursor.destroy()'

#### Database

#####'db.addUser(document)'

#####'db.createCollection(name, options, [callback])'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.explain"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>explain (cb)](#apidoc.element.mongojs.cursor.prototype.explain)
- description and source-code
```javascript
explain = function (cb) {
  this._get(function (err, cursor) {
    if (err) { return cb(err) }
    cursor.explain(cb)
  })
}
```
- example usage
```shell
...

#### Cursor

#####'cursor.batchSize(size, [callback])'

#####'cursor.count(callback)'

#####'cursor.explain(callback)'

#####'cursor.forEach(function)'

#####'cursor.limit(n, [callback])'

#####'cursor.map(function, [callback])'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.forEach"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>forEach (fn)](#apidoc.element.mongojs.cursor.prototype.forEach)
- description and source-code
```javascript
forEach = function (fn) {
  var self = this

  var loop = function () {
    self.next(function (err, obj) {
      if (err) return fn(err)
      fn(err, obj)

      if (!obj) return

      // Fix for #270 RangeError: Maximum call stack size exceeded using Collection.find
      setImmediate(loop)
    })
  }

  loop()
}
```
- example usage
```shell
...

// find everything, but sort by name
db.mycollection.find().sort({name: 1}, function (err, docs) {
	// docs is now a sorted array
})

// iterate over all whose level is greater than 90.
db.mycollection.find({level: {$gt: 90}}).forEach(function (err, doc) {
	if (!doc) {
		// we visited all docs in the collection
		return
	}
	// doc is a document in the collection
})
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.hint"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>hint (obj, cb)](#apidoc.element.mongojs.cursor.prototype.hint)
- description and source-code
```javascript
hint = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.limit"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>limit (obj, cb)](#apidoc.element.mongojs.cursor.prototype.limit)
- description and source-code
```javascript
limit = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
...
'''

If you provide a callback to 'find' or any cursor config operation mongojs will call 'toArray' for you

'''js
db.mycollection.find({}, function (err, docs) { ... })

db.mycollection.find({}).limit(2).skip(1, function (err, docs) { ... })
'''
is the same as

'''js
db.mycollection.find({}).toArray(function (err, docs) { ... })

db.mycollection.find({}).limit(2).skip(1).toArray(function (err, docs) { ... })
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.map"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>map (mapfn, cb)](#apidoc.element.mongojs.cursor.prototype.map)
- description and source-code
```javascript
map = function (mapfn, cb) {
  var array = []
  var self = this

  var loop = function () {
    self.next(function (err, obj) {
      if (err) return cb(err)
      if (!obj) return cb(null, array)
      array.push(mapfn(obj))

      // Fix for #270 RangeError: Maximum call stack size exceeded using Collection.find
      setImmediate(loop)
    })
  }

  loop()
}
```
- example usage
```shell
...

#####'cursor.explain(callback)'

#####'cursor.forEach(function)'

#####'cursor.limit(n, [callback])'

#####'cursor.map(function, [callback])'

#####'cursor.next(callback)'

#####'cursor.skip(n, [callback])'

#####'cursor.sort(sortOptions, [callback])'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.max"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>max (obj, cb)](#apidoc.element.mongojs.cursor.prototype.max)
- description and source-code
```javascript
max = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.maxTimeMS"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>maxTimeMS (obj, cb)](#apidoc.element.mongojs.cursor.prototype.maxTimeMS)
- description and source-code
```javascript
maxTimeMS = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.min"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>min (obj, cb)](#apidoc.element.mongojs.cursor.prototype.min)
- description and source-code
```javascript
min = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.next"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>next (cb)](#apidoc.element.mongojs.cursor.prototype.next)
- description and source-code
```javascript
next = function (cb) {
  this._get(function (err, cursor) {
    if (err) return cb(err)

    if (cursor.cursorState.dead || cursor.cursorState.killed) {
      return cb(null, null)
    } else {
      cursor.next(cb)
    }
  })

  return this
}
```
- example usage
```shell
...

#####'cursor.forEach(function)'

#####'cursor.limit(n, [callback])'

#####'cursor.map(function, [callback])'

#####'cursor.next(callback)'

#####'cursor.skip(n, [callback])'

#####'cursor.sort(sortOptions, [callback])'

#####'cursor.toArray(callback)'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.rewind"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>rewind (cb)](#apidoc.element.mongojs.cursor.prototype.rewind)
- description and source-code
```javascript
rewind = function (cb) {
  this._get(function (err, cursor) {
    if (err) return cb(err)
    cursor.rewind(cb)
  })

  return this
}
```
- example usage
```shell
...

#####'cursor.skip(n, [callback])'

#####'cursor.sort(sortOptions, [callback])'

#####'cursor.toArray(callback)'

#####'cursor.rewind()'

#####'cursor.destroy()'

#### Database

#####'db.addUser(document)'
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.size"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>size (cb)](#apidoc.element.mongojs.cursor.prototype.size)
- description and source-code
```javascript
size = function (cb) {
  var self = this

  this._get(function (err, cursor) {
    if (err) { return cb(err) }
    cursor.count(true, self.opts, cb)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.skip"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>skip (obj, cb)](#apidoc.element.mongojs.cursor.prototype.skip)
- description and source-code
```javascript
skip = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
...
'''

If you provide a callback to 'find' or any cursor config operation mongojs will call 'toArray' for you

'''js
db.mycollection.find({}, function (err, docs) { ... })

db.mycollection.find({}).limit(2).skip(1, function (err, docs) { ... })
'''
is the same as

'''js
db.mycollection.find({}).toArray(function (err, docs) { ... })

db.mycollection.find({}).limit(2).skip(1).toArray(function (err, docs) { ... })
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.snapshot"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>snapshot (obj, cb)](#apidoc.element.mongojs.cursor.prototype.snapshot)
- description and source-code
```javascript
snapshot = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.cursor.prototype.sort"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>sort (obj, cb)](#apidoc.element.mongojs.cursor.prototype.sort)
- description and source-code
```javascript
sort = function (obj, cb) {
  this._opts[opt] = obj
  if (cb) return this.toArray(cb)
  return this
}
```
- example usage
```shell
...
'''js
// find everything
db.mycollection.find(function (err, docs) {
	// docs is an array of all the documents in mycollection
})

// find everything, but sort by name
db.mycollection.find().sort({name: 1}, function (err, docs) {
	// docs is now a sorted array
})

// iterate over all whose level is greater than 90.
db.mycollection.find({level: {$gt: 90}}).forEach(function (err, doc) {
	if (!doc) {
		// we visited all docs in the collection
...
```

#### <a name="apidoc.element.mongojs.cursor.prototype.toArray"></a>[function <span class="apidocSignatureSpan">mongojs.cursor.prototype.</span>toArray (cb)](#apidoc.element.mongojs.cursor.prototype.toArray)
- description and source-code
```javascript
toArray = function (cb) {
  var array = []
  var self = this

  var loop = function () {
    self.next(function (err, obj) {
      if (err) return cb(err)
      if (!obj) return cb(null, array)
      array.push(obj)

      // Fix for #270 RangeError: Maximum call stack size exceeded using Collection.find
      setImmediate(loop)
    })
  }

  loop()
}
```
- example usage
```shell
...
db.mycollection.find({}, function (err, docs) { ... })

db.mycollection.find({}).limit(2).skip(1, function (err, docs) { ... })
'''
is the same as

'''js
db.mycollection.find({}).toArray(function (err, docs) { ... })

db.mycollection.find({}).limit(2).skip(1).toArray(function (err, docs) { ... })
'''

For more detailed information about the different usages of update and querying see [the mongo docs](http://www.mongodb.org/display
/DOCS/Manual)
...
```



# <a name="apidoc.module.mongojs.database"></a>[module mongojs.database](#apidoc.module.mongojs.database)

#### <a name="apidoc.element.mongojs.database.database"></a>[function <span class="apidocSignatureSpan">mongojs.</span>database (connString, cols, options)](#apidoc.element.mongojs.database.database)
- description and source-code
```javascript
database = function (connString, cols, options) {
  var self = this

  EventEmitter.call(this)

  if (typeof connString === 'string') {
    this._dbname = parse(connString).dbName

    // Fix short cut connection URLs consisting only of a db name or db + host
    if (connString.indexOf('/') < 0) {
      connString = 'localhost/' + connString
    }

    if (connString.indexOf('mongodb://') < 0) {
      connString = 'mongodb://' + connString
    }

    this._getConnection = thunky(function (cb) {
      mongodb.connect(connString, options, function (err, db) {
        if (err) {
          self.emit('error', err) // It's safer to emit an error instead of rely on the cb to handle the error
          return cb(err)
        }

        self.emit('connect')
        cb(null, db)
      })
    })
  } else if (typeof connString._getConnection === 'function') { // mongojs
    this._dbname = connString._dbname
    this._getConnection = connString._getConnection
  } else { // try mongodb-native
    this._dbname = parse(connString.options.url).dbName

    this._getConnection = thunky(function (cb) {
      cb(null, connString)
    })
  }

  this.ObjectId = mongodb.ObjectId

  cols = cols || []
  cols.forEach(function (colName) {
    self[colName] = self.collection(colName)

    var parts = colName.split('.')

    var last = parts.pop()
    var parent = parts.reduce(function (parent, prefix) {
      parent[prefix] = parent[prefix] || {}
      return parent[prefix]
    }, self)

    parent[last] = self.collection(colName)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.database.super_"></a>[function <span class="apidocSignatureSpan">mongojs.database.</span>super_ ()](#apidoc.element.mongojs.database.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongojs.database.prototype"></a>[module mongojs.database.prototype](#apidoc.module.mongojs.database.prototype)

#### <a name="apidoc.element.mongojs.database.prototype.addUser"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>addUser (usr, cb)](#apidoc.element.mongojs.database.prototype.addUser)
- description and source-code
```javascript
addUser = function (usr, cb) {
  var cmd = xtend({createUser: usr.user}, usr)
  delete cmd.user
  this.runCommand(cmd, cb)
}
```
- example usage
```shell
...

#####'cursor.rewind()'

#####'cursor.destroy()'

#### Database

#####'db.addUser(document)'

#####'db.createCollection(name, options, [callback])'

#####'db.dropDatabase([callback])'

#####'db.eval(code, [params], [options], [callback])'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.close"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>close (force, cb)](#apidoc.element.mongojs.database.prototype.close)
- description and source-code
```javascript
close = function (force, cb) {
  if (typeof force === 'function') { return this.close(false, force) }

  var self = this

  cb = cb || noop
  this._getConnection(function (err, server) {
    if (err) return cb(err)

    server.close(force)

    self.emit('close')
    cb()
  })
}
```
- example usage
```shell
...

#####'db.removeUser(username, [callback])'

#####'db.runCommand(command, [callback])'

#####'db.stats([callback])'

#####'db.close()'

#### Bulk

#####'bulk.execute()'

#####'bulk.find(query)'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.collection"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>collection (colName)](#apidoc.element.mongojs.database.prototype.collection)
- description and source-code
```javascript
collection = function (colName) {
  return new Collection({name: colName}, this._getConnection)
}
```
- example usage
```shell
...
var db = mongojs('username:password@example.com/mydb?authSource=authdb', ['mycollection'])

// connect with options
var db = mongojs('username:password@example.com/mydb', ['mycollection'], { ssl: true })

// connect now, and worry about collections later
var db = mongojs('mydb')
var mycollection = db.collection('mycollection')
'''

[More connection string examples](http://mongodb.github.io/node-mongodb-native/2.0/reference/connecting/)

After we connected we can query or update the database just how we would using the mongo API with the exception that we use a callback
.
The format for callbacks is always 'callback(error, value)' where error is null if no exception has occured. The update methods '
save', 'remove', 'update' and 'findAndModify' also pass the 'lastErrorObject' as the last argument to the callback function.
...
```

#### <a name="apidoc.element.mongojs.database.prototype.createCollection"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>createCollection (name, opts, cb)](#apidoc.element.mongojs.database.prototype.createCollection)
- description and source-code
```javascript
createCollection = function (name, opts, cb) {
  if (typeof opts === 'function') return this.createCollection(name, {}, opts)

  var cmd = {create: name}
  Object.keys(opts).forEach(function (opt) {
    cmd[opt] = opts[opt]
  })
  this.runCommand(cmd, cb)
}
```
- example usage
```shell
...

#####'cursor.destroy()'

#### Database

#####'db.addUser(document)'

#####'db.createCollection(name, options, [callback])'

#####'db.dropDatabase([callback])'

#####'db.eval(code, [params], [options], [callback])'

#####'db.getCollectionNames(callback)'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.createUser"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>createUser (usr, cb)](#apidoc.element.mongojs.database.prototype.createUser)
- description and source-code
```javascript
createUser = function (usr, cb) {
  var cmd = xtend({createUser: usr.user}, usr)
  delete cmd.user
  this.runCommand(cmd, cb)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.database.prototype.dropDatabase"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>dropDatabase (cb)](#apidoc.element.mongojs.database.prototype.dropDatabase)
- description and source-code
```javascript
dropDatabase = function (cb) {
  this.runCommand('dropDatabase', cb)
}
```
- example usage
```shell
...

#### Database

#####'db.addUser(document)'

#####'db.createCollection(name, options, [callback])'

#####'db.dropDatabase([callback])'

#####'db.eval(code, [params], [options], [callback])'

#####'db.getCollectionNames(callback)'

#####'db.getLastError(callback)'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.dropUser"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>dropUser (username, cb)](#apidoc.element.mongojs.database.prototype.dropUser)
- description and source-code
```javascript
dropUser = function (username, cb) {
  this.runCommand({dropUser: username}, cb)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongojs.database.prototype.eval"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>eval (fn)](#apidoc.element.mongojs.database.prototype.eval)
- description and source-code
```javascript
eval = function (fn) {
  var cb = arguments[arguments.length - 1]
  this.runCommand({
    eval: fn.toString(),
    args: Array.prototype.slice.call(arguments, 1, arguments.length - 1)
  }, function (err, res) {
    if (err) return cb(err)
    cb(null, res.retval)
  })
}
```
- example usage
```shell
...

#####'db.addUser(document)'

#####'db.createCollection(name, options, [callback])'

#####'db.dropDatabase([callback])'

#####'db.eval(code, [params], [options], [callback])'

#####'db.getCollectionNames(callback)'

#####'db.getLastError(callback)'

#####'db.getLastErrorObj(callback)'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.getCollectionNames"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>getCollectionNames (cb)](#apidoc.element.mongojs.database.prototype.getCollectionNames)
- description and source-code
```javascript
getCollectionNames = function (cb) {
  this.listCollections(function (err, collections) {
    if (err) { return cb(err) }
    cb(null, collections.map(function (collection) { return collection.name }))
  })
}
```
- example usage
```shell
...

#####'db.createCollection(name, options, [callback])'

#####'db.dropDatabase([callback])'

#####'db.eval(code, [params], [options], [callback])'

#####'db.getCollectionNames(callback)'

#####'db.getLastError(callback)'

#####'db.getLastErrorObj(callback)'

#####'db.removeUser(username, [callback])'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.getLastError"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>getLastError (cb)](#apidoc.element.mongojs.database.prototype.getLastError)
- description and source-code
```javascript
getLastError = function (cb) {
  this.runCommand('getLastError', function (err, res) {
    if (err) return cb(err)
    cb(null, res.err)
  })
}
```
- example usage
```shell
...

#####'db.dropDatabase([callback])'

#####'db.eval(code, [params], [options], [callback])'

#####'db.getCollectionNames(callback)'

#####'db.getLastError(callback)'

#####'db.getLastErrorObj(callback)'

#####'db.removeUser(username, [callback])'

#####'db.runCommand(command, [callback])'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.getLastErrorObj"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>getLastErrorObj (cb)](#apidoc.element.mongojs.database.prototype.getLastErrorObj)
- description and source-code
```javascript
getLastErrorObj = function (cb) {
  this.runCommand('getLastError', cb)
}
```
- example usage
```shell
...

#####'db.eval(code, [params], [options], [callback])'

#####'db.getCollectionNames(callback)'

#####'db.getLastError(callback)'

#####'db.getLastErrorObj(callback)'

#####'db.removeUser(username, [callback])'

#####'db.runCommand(command, [callback])'

#####'db.stats([callback])'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.listCollections"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>listCollections (cb)](#apidoc.element.mongojs.database.prototype.listCollections)
- description and source-code
```javascript
listCollections = function (cb) {
  this._getConnection(function (err, connection) {
    if (err) { return cb(err) }

    connection.listCollections().toArray(function (err, collections) {
      if (err) { return cb(err) }
      cb(null, collections)
    })
  })
}
```
- example usage
```shell
...
  })
}

Database.prototype.listCollections = function (cb) {
  this._getConnection(function (err, connection) {
    if (err) { return cb(err) }

    connection.listCollections().toArray(function (err, collections) {
      if (err) { return cb(err) }
      cb(null, collections)
    })
  })
}

Database.prototype.getCollectionNames = function (cb) {
...
```

#### <a name="apidoc.element.mongojs.database.prototype.removeUser"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>removeUser (username, cb)](#apidoc.element.mongojs.database.prototype.removeUser)
- description and source-code
```javascript
removeUser = function (username, cb) {
  this.runCommand({dropUser: username}, cb)
}
```
- example usage
```shell
...

#####'db.getCollectionNames(callback)'

#####'db.getLastError(callback)'

#####'db.getLastErrorObj(callback)'

#####'db.removeUser(username, [callback])'

#####'db.runCommand(command, [callback])'

#####'db.stats([callback])'

#####'db.close()'
...
```

#### <a name="apidoc.element.mongojs.database.prototype.runCommand"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>runCommand (opts, cb)](#apidoc.element.mongojs.database.prototype.runCommand)
- description and source-code
```javascript
runCommand = function (opts, cb) {
  cb = cb || noop
  if (typeof opts === 'string') {
    var tmp = opts
    opts = {}
    opts[tmp] = 1
  }

  this._getConnection(function (err, connection) {
    if (err) return cb(err)
    connection.command(opts, function (err, result) {
      if (err) return cb(err)
      cb(null, result)
    })
  })
}
```
- example usage
```shell
...
})
'''

Note that you need to explicitly set the selection parameter in the 'find' call.

## Database commands

With mongojs you can run database commands just like with the mongo shell using 'db.runCommand()'

'''js
db.runCommand({ping: 1}, function (err, res) {
	if(!err && res.ok) console.log('we\'re up')
})
'''
...
```

#### <a name="apidoc.element.mongojs.database.prototype.stats"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>stats (scale, cb)](#apidoc.element.mongojs.database.prototype.stats)
- description and source-code
```javascript
stats = function (scale, cb) {
  if (typeof scale === 'function') return this.stats(1, scale)
  this.runCommand({dbStats: 1, scale: scale}, cb)
}
```
- example usage
```shell
...
#####'db.collection.remove(query, [justOne], [callback])'
#####'db.collection.remove(query, [options], [callback])'

#####'db.collection.runCommand(command, [callback])'

#####'db.collection.save(doc, [options], [callback])'

#####'db.collection.stats(callback)'

#####'db.collection.update(query, update, [options], [callback])'

#####'db.collection.toString()'

Get the name of the collection.
...
```

#### <a name="apidoc.element.mongojs.database.prototype.toString"></a>[function <span class="apidocSignatureSpan">mongojs.database.prototype.</span>toString ()](#apidoc.element.mongojs.database.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this._dbname
}
```
- example usage
```shell
...
	// doc is a document in the collection
})

// find a document using a native ObjectId
db.mycollection.findOne({
	_id: mongojs.ObjectId('523209c4561c640000000001')
}, function(err, doc) {
	// doc._id.toString() === '523209c4561c640000000001'
})

// find all named 'mathias' and increment their level
db.mycollection.update({name: 'mathias'}, {$inc: {level: 1}}, {multi: true}, function () {
	// the update is complete
})
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
