# api documentation for  [immutable (v3.8.1)](https://facebook.github.com/immutable-js)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-immutable.svg)](https://travis-ci.org/npmdoc/node-npmdoc-immutable)
#### Immutable Data Collections

[![NPM](https://nodei.co/npm/immutable.png?downloads=true)](https://www.npmjs.com/package/immutable)

[![apidoc](https://npmdoc.github.io/node-npmdoc-immutable/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-immutable_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-immutable/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-immutable/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Lee Byron",
        "url": "https://github.com/leebyron"
    },
    "bugs": {
        "url": "https://github.com/facebook/immutable-js/issues"
    },
    "dependencies": {},
    "description": "Immutable Data Collections",
    "devDependencies": {
        "acorn": "0.11.x",
        "babel-eslint": "^4.1.8",
        "benchmark": "^1.0.0",
        "bluebird": "3.1.1",
        "browser-sync": "2.11.0",
        "browserify": "^5.11.2",
        "colors": "1.1.2",
        "del": "2.2.0",
        "es6-transpiler": "0.7.18",
        "eslint": "^1.10.3",
        "estraverse": "1.9.3",
        "express": "^4.13.4",
        "fbjs-scripts": "^0.5.0",
        "grunt": "0.4.5",
        "grunt-cli": "0.1.13",
        "grunt-contrib-clean": "0.7.0",
        "grunt-contrib-copy": "0.8.2",
        "grunt-contrib-jshint": "0.11.3",
        "grunt-release": "0.13.0",
        "gulp": "3.9.0",
        "gulp-concat": "2.6.0",
        "gulp-filter": "3.0.1",
        "gulp-header": "1.7.1",
        "gulp-jest": "^0.2.1",
        "gulp-jshint": "^1.8.4",
        "gulp-less": "3.0.5",
        "gulp-size": "2.0.0",
        "gulp-sourcemaps": "1.6.0",
        "gulp-uglify": "1.5.1",
        "gulp-util": "3.0.7",
        "harmonize": "1.4.4",
        "jasmine-check": "^0.1.2",
        "jest-cli": "^0.5.10",
        "jshint-stylish": "^0.4.0",
        "magic-string": "0.10.2",
        "marked": "0.3.5",
        "microtime": "^2.0.0",
        "node-jsx": "^0.12.4",
        "react": "^0.12.0",
        "react-router": "^0.11.2",
        "react-tools": "^0.12.0",
        "rollup": "0.24.0",
        "run-sequence": "1.1.5",
        "through2": "2.0.0",
        "typescript": "1.7.5",
        "uglify-js": "2.6.1",
        "vinyl-buffer": "1.0.0",
        "vinyl-source-stream": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "200807f11ab0f72710ea485542de088075f68cd2",
        "tarball": "https://registry.npmjs.org/immutable/-/immutable-3.8.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "dist",
        "contrib",
        "README.md",
        "LICENSE",
        "PATENTS"
    ],
    "gitHead": "e96d73f7e1fbeff00d03b09aa4352e04de61abb3",
    "homepage": "https://facebook.github.com/immutable-js",
    "jest": {
        "scriptPreprocessor": "resources/jestPreprocessor.js",
        "testFileExtensions": [
            "js",
            "ts"
        ],
        "persistModuleRegistryBetweenSpecs": true
    },
    "keywords": [
        "immutable",
        "persistent",
        "lazy",
        "data",
        "datastructure",
        "functional",
        "collection",
        "stateless",
        "sequence",
        "iteration"
    ],
    "license": "BSD-3-Clause",
    "main": "dist/immutable.js",
    "maintainers": [
        {
            "name": "leebyron",
            "email": "lee@leebyron.com"
        }
    ],
    "name": "immutable",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/facebook/immutable-js.git"
    },
    "scripts": {
        "build": "grunt default && gulp default",
        "deploy": "(cd ./pages/out && git init && git config user.name \"Travis CI\" && git config user.email \"github@fb.com\" && git add . && git commit -m \"Deploy to GitHub Pages\" && git push --force --quiet \"https://${GH_TOKEN}@github.com/facebook/immutable-js.git\" master:gh-pages > /dev/null 2>1)",
        "lint": "eslint src/ && grunt lint && gulp lint",
        "perf": "node ./resources/bench.js",
        "start": "npm run build && node ./pages/resources/start.js",
        "test": "npm run lint && npm run testonly",
        "testonly": "./resources/node_test.sh"
    },
    "typescript": {
        "definition": "dist/immutable.d.ts"
    },
    "typings": "dist/immutable-nonambient.d.ts",
    "version": "3.8.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module immutable](#apidoc.module.immutable)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection ()](#apidoc.element.immutable.Collection)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection.Indexed ()](#apidoc.element.immutable.Collection.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection.Indexed.prototype.constructor (value)](#apidoc.element.immutable.Collection.Indexed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection.Keyed ()](#apidoc.element.immutable.Collection.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection.Keyed.prototype.constructor (value)](#apidoc.element.immutable.Collection.Keyed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection.Set ()](#apidoc.element.immutable.Collection.Set)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection.Set.prototype.constructor (value)](#apidoc.element.immutable.Collection.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Iterable (value)](#apidoc.element.immutable.Iterable)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Iterable.Iterator (next)](#apidoc.element.immutable.Iterable.Iterator)
1.  [function <span class="apidocSignatureSpan">immutable.</span>List (value)](#apidoc.element.immutable.List)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Map (value)](#apidoc.element.immutable.Map)
1.  [function <span class="apidocSignatureSpan">immutable.</span>OrderedMap (value)](#apidoc.element.immutable.OrderedMap)
1.  [function <span class="apidocSignatureSpan">immutable.</span>OrderedSet (value)](#apidoc.element.immutable.OrderedSet)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Range (start, end, step)](#apidoc.element.immutable.Range)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Record (defaultValues, name)](#apidoc.element.immutable.Record)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Repeat (value, times)](#apidoc.element.immutable.Repeat)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Seq (value)](#apidoc.element.immutable.Seq)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Seq.Indexed (value)](#apidoc.element.immutable.Seq.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Seq.Keyed (value)](#apidoc.element.immutable.Seq.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Seq.Set (value)](#apidoc.element.immutable.Seq.Set)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Set (value)](#apidoc.element.immutable.Set)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Stack (value)](#apidoc.element.immutable.Stack)
1.  [function <span class="apidocSignatureSpan">immutable.</span>fromJS (json, converter)](#apidoc.element.immutable.fromJS)
1.  [function <span class="apidocSignatureSpan">immutable.</span>is (valueA, valueB)](#apidoc.element.immutable.is)
1.  object <span class="apidocSignatureSpan">immutable.</span>Collection.Indexed.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Collection.Keyed.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Collection.Set.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Collection.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Iterable.Indexed.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Iterable.Iterator.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Iterable.Keyed.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Iterable.Set.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Iterable.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>List.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Map.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>OrderedMap.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>OrderedSet.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Range.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Record.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Repeat.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Seq.Indexed.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Seq.Keyed.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Seq.Set.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Seq.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Set.prototype
1.  object <span class="apidocSignatureSpan">immutable.</span>Stack.prototype

#### [module immutable.Collection](#apidoc.module.immutable.Collection)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Collection ()](#apidoc.element.immutable.Collection.Collection)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.</span>Indexed ()](#apidoc.element.immutable.Collection.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.</span>Keyed ()](#apidoc.element.immutable.Collection.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.</span>Set ()](#apidoc.element.immutable.Collection.Set)

#### [module immutable.Collection.Indexed](#apidoc.module.immutable.Collection.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.</span>Indexed ()](#apidoc.element.immutable.Collection.Indexed.Indexed)

#### [module immutable.Collection.Indexed.prototype](#apidoc.module.immutable.Collection.Indexed.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>constructor (value)](#apidoc.element.immutable.Collection.Indexed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.filter)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>findIndex (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>findLastIndex (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.findLastIndex)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>first ()](#apidoc.element.immutable.Collection.Indexed.prototype.first)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>flatten (depth)](#apidoc.element.immutable.Collection.Indexed.prototype.flatten)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Collection.Indexed.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>has (index)](#apidoc.element.immutable.Collection.Indexed.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Collection.Indexed.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>interleave ()](#apidoc.element.immutable.Collection.Indexed.prototype.interleave)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>interpose (separator)](#apidoc.element.immutable.Collection.Indexed.prototype.interpose)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>keySeq ()](#apidoc.element.immutable.Collection.Indexed.prototype.keySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>last ()](#apidoc.element.immutable.Collection.Indexed.prototype.last)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Collection.Indexed.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>reverse ()](#apidoc.element.immutable.Collection.Indexed.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.skipWhile)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Collection.Indexed.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>splice (index, removeNum)](#apidoc.element.immutable.Collection.Indexed.prototype.splice)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Collection.Indexed.prototype.toKeyedSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>zip ()](#apidoc.element.immutable.Collection.Indexed.prototype.zip)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>zipWith (zipper)](#apidoc.element.immutable.Collection.Indexed.prototype.zipWith)

#### [module immutable.Collection.Indexed.prototype.constructor](#apidoc.module.immutable.Collection.Indexed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.Indexed.prototype.constructor.constructor)

#### [module immutable.Collection.Keyed](#apidoc.module.immutable.Collection.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.</span>Keyed ()](#apidoc.element.immutable.Collection.Keyed.Keyed)

#### [module immutable.Collection.Keyed.prototype](#apidoc.module.immutable.Collection.Keyed.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>__toJS ()](#apidoc.element.immutable.Collection.Keyed.prototype.__toJS)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>__toStringMapper (v, k)](#apidoc.element.immutable.Collection.Keyed.prototype.__toStringMapper)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>constructor (value)](#apidoc.element.immutable.Collection.Keyed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>flip ()](#apidoc.element.immutable.Collection.Keyed.prototype.flip)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>mapEntries (mapper, context)](#apidoc.element.immutable.Collection.Keyed.prototype.mapEntries)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>mapKeys (mapper, context)](#apidoc.element.immutable.Collection.Keyed.prototype.mapKeys)

#### [module immutable.Collection.Keyed.prototype.constructor](#apidoc.module.immutable.Collection.Keyed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.Keyed.prototype.constructor.constructor)

#### [module immutable.Collection.Set](#apidoc.module.immutable.Collection.Set)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.</span>Set ()](#apidoc.element.immutable.Collection.Set.Set)

#### [module immutable.Collection.Set.prototype](#apidoc.module.immutable.Collection.Set.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Collection.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>contains (value)](#apidoc.element.immutable.Collection.Set.prototype.contains)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>get (value, notSetValue)](#apidoc.element.immutable.Collection.Set.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>has (searchValue)](#apidoc.element.immutable.Collection.Set.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>includes (value)](#apidoc.element.immutable.Collection.Set.prototype.includes)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>keySeq ()](#apidoc.element.immutable.Collection.Set.prototype.keySeq)

#### [module immutable.Collection.Set.prototype.constructor](#apidoc.module.immutable.Collection.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.Set.prototype.constructor.constructor)

#### [module immutable.Collection.prototype](#apidoc.module.immutable.Collection.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Collection.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.prototype.constructor)

#### [module immutable.Iterable](#apidoc.module.immutable.Iterable)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Iterable (value)](#apidoc.element.immutable.Iterable.Iterable)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>Indexed (value)](#apidoc.element.immutable.Iterable.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>Iterator (next)](#apidoc.element.immutable.Iterable.Iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>Keyed (value)](#apidoc.element.immutable.Iterable.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>Set (value)](#apidoc.element.immutable.Iterable.Set)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>isAssociative (maybeAssociative)](#apidoc.element.immutable.Iterable.isAssociative)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>isIndexed (maybeIndexed)](#apidoc.element.immutable.Iterable.isIndexed)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>isIterable (maybeIterable)](#apidoc.element.immutable.Iterable.isIterable)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>isKeyed (maybeKeyed)](#apidoc.element.immutable.Iterable.isKeyed)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>isOrdered (maybeOrdered)](#apidoc.element.immutable.Iterable.isOrdered)

#### [module immutable.Iterable.Indexed.prototype](#apidoc.module.immutable.Iterable.Indexed.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>constructor (value)](#apidoc.element.immutable.Iterable.Indexed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.filter)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>findIndex (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>findLastIndex (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.findLastIndex)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>first ()](#apidoc.element.immutable.Iterable.Indexed.prototype.first)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>flatten (depth)](#apidoc.element.immutable.Iterable.Indexed.prototype.flatten)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Iterable.Indexed.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>has (index)](#apidoc.element.immutable.Iterable.Indexed.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Iterable.Indexed.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>interleave ()](#apidoc.element.immutable.Iterable.Indexed.prototype.interleave)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>interpose (separator)](#apidoc.element.immutable.Iterable.Indexed.prototype.interpose)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>keySeq ()](#apidoc.element.immutable.Iterable.Indexed.prototype.keySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>last ()](#apidoc.element.immutable.Iterable.Indexed.prototype.last)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Iterable.Indexed.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>reverse ()](#apidoc.element.immutable.Iterable.Indexed.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.skipWhile)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Iterable.Indexed.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>splice (index, removeNum)](#apidoc.element.immutable.Iterable.Indexed.prototype.splice)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Iterable.Indexed.prototype.toKeyedSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>zip ()](#apidoc.element.immutable.Iterable.Indexed.prototype.zip)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>zipWith (zipper)](#apidoc.element.immutable.Iterable.Indexed.prototype.zipWith)

#### [module immutable.Iterable.Iterator](#apidoc.module.immutable.Iterable.Iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.</span>Iterator (next)](#apidoc.element.immutable.Iterable.Iterator.Iterator)
1.  number <span class="apidocSignatureSpan">immutable.Iterable.Iterator.</span>ENTRIES
1.  number <span class="apidocSignatureSpan">immutable.Iterable.Iterator.</span>KEYS
1.  number <span class="apidocSignatureSpan">immutable.Iterable.Iterator.</span>VALUES

#### [module immutable.Iterable.Iterator.prototype](#apidoc.module.immutable.Iterable.Iterator.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Iterator.prototype.</span>inspect ()](#apidoc.element.immutable.Iterable.Iterator.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Iterator.prototype.</span>toSource ()](#apidoc.element.immutable.Iterable.Iterator.prototype.toSource)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Iterator.prototype.</span>toString ()](#apidoc.element.immutable.Iterable.Iterator.prototype.toString)

#### [module immutable.Iterable.Keyed.prototype](#apidoc.module.immutable.Iterable.Keyed.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>__toJS ()](#apidoc.element.immutable.Iterable.Keyed.prototype.__toJS)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>__toStringMapper (v, k)](#apidoc.element.immutable.Iterable.Keyed.prototype.__toStringMapper)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>constructor (value)](#apidoc.element.immutable.Iterable.Keyed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>flip ()](#apidoc.element.immutable.Iterable.Keyed.prototype.flip)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>mapEntries (mapper, context)](#apidoc.element.immutable.Iterable.Keyed.prototype.mapEntries)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>mapKeys (mapper, context)](#apidoc.element.immutable.Iterable.Keyed.prototype.mapKeys)

#### [module immutable.Iterable.Set.prototype](#apidoc.module.immutable.Iterable.Set.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Iterable.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>contains (value)](#apidoc.element.immutable.Iterable.Set.prototype.contains)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>get (value, notSetValue)](#apidoc.element.immutable.Iterable.Set.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>has (searchValue)](#apidoc.element.immutable.Iterable.Set.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>includes (value)](#apidoc.element.immutable.Iterable.Set.prototype.includes)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>keySeq ()](#apidoc.element.immutable.Iterable.Set.prototype.keySeq)

#### [module immutable.Iterable.prototype](#apidoc.module.immutable.Iterable.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>__toJS ()](#apidoc.element.immutable.Iterable.prototype.__toJS)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>__toString (head, tail)](#apidoc.element.immutable.Iterable.prototype.__toString)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>__toStringMapper (value)](#apidoc.element.immutable.Iterable.prototype.__toStringMapper)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>butLast ()](#apidoc.element.immutable.Iterable.prototype.butLast)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>chain (mapper, context)](#apidoc.element.immutable.Iterable.prototype.chain)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>concat ()](#apidoc.element.immutable.Iterable.prototype.concat)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>contains (searchValue)](#apidoc.element.immutable.Iterable.prototype.contains)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>count (predicate, context)](#apidoc.element.immutable.Iterable.prototype.count)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>countBy (grouper, context)](#apidoc.element.immutable.Iterable.prototype.countBy)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>entries ()](#apidoc.element.immutable.Iterable.prototype.entries)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>entrySeq ()](#apidoc.element.immutable.Iterable.prototype.entrySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>equals (other)](#apidoc.element.immutable.Iterable.prototype.equals)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>every (predicate, context)](#apidoc.element.immutable.Iterable.prototype.every)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Iterable.prototype.filter)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>filterNot (predicate, context)](#apidoc.element.immutable.Iterable.prototype.filterNot)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>find (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.find)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findEntry (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.findEntry)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findKey (predicate, context)](#apidoc.element.immutable.Iterable.prototype.findKey)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findLast (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.findLast)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findLastEntry (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.findLastEntry)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findLastKey (predicate, context)](#apidoc.element.immutable.Iterable.prototype.findLastKey)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>first ()](#apidoc.element.immutable.Iterable.prototype.first)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>flatMap (mapper, context)](#apidoc.element.immutable.Iterable.prototype.flatMap)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>flatten (depth)](#apidoc.element.immutable.Iterable.prototype.flatten)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>forEach (sideEffect, context)](#apidoc.element.immutable.Iterable.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>fromEntrySeq ()](#apidoc.element.immutable.Iterable.prototype.fromEntrySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>get (searchKey, notSetValue)](#apidoc.element.immutable.Iterable.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>getIn (searchKeyPath, notSetValue)](#apidoc.element.immutable.Iterable.prototype.getIn)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>groupBy (grouper, context)](#apidoc.element.immutable.Iterable.prototype.groupBy)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>has (searchKey)](#apidoc.element.immutable.Iterable.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>hasIn (searchKeyPath)](#apidoc.element.immutable.Iterable.prototype.hasIn)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>hashCode ()](#apidoc.element.immutable.Iterable.prototype.hashCode)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>includes (searchValue)](#apidoc.element.immutable.Iterable.prototype.includes)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>inspect ()](#apidoc.element.immutable.Iterable.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>isEmpty ()](#apidoc.element.immutable.Iterable.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>isSubset (iter)](#apidoc.element.immutable.Iterable.prototype.isSubset)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>isSuperset (iter)](#apidoc.element.immutable.Iterable.prototype.isSuperset)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>join (separator)](#apidoc.element.immutable.Iterable.prototype.join)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>keyOf (searchValue)](#apidoc.element.immutable.Iterable.prototype.keyOf)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>keySeq ()](#apidoc.element.immutable.Iterable.prototype.keySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>keys ()](#apidoc.element.immutable.Iterable.prototype.keys)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>last ()](#apidoc.element.immutable.Iterable.prototype.last)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>lastKeyOf (searchValue)](#apidoc.element.immutable.Iterable.prototype.lastKeyOf)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>map (mapper, context)](#apidoc.element.immutable.Iterable.prototype.map)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>max (comparator)](#apidoc.element.immutable.Iterable.prototype.max)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>maxBy (mapper, comparator)](#apidoc.element.immutable.Iterable.prototype.maxBy)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>min (comparator)](#apidoc.element.immutable.Iterable.prototype.min)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>minBy (mapper, comparator)](#apidoc.element.immutable.Iterable.prototype.minBy)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>reduce (reducer, initialReduction, context)](#apidoc.element.immutable.Iterable.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>reduceRight (reducer, initialReduction, context)](#apidoc.element.immutable.Iterable.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>rest ()](#apidoc.element.immutable.Iterable.prototype.rest)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>reverse ()](#apidoc.element.immutable.Iterable.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skip (amount)](#apidoc.element.immutable.Iterable.prototype.skip)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skipLast (amount)](#apidoc.element.immutable.Iterable.prototype.skipLast)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skipUntil (predicate, context)](#apidoc.element.immutable.Iterable.prototype.skipUntil)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Iterable.prototype.skipWhile)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Iterable.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>some (predicate, context)](#apidoc.element.immutable.Iterable.prototype.some)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>sort (comparator)](#apidoc.element.immutable.Iterable.prototype.sort)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>sortBy (mapper, comparator)](#apidoc.element.immutable.Iterable.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>take (amount)](#apidoc.element.immutable.Iterable.prototype.take)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>takeLast (amount)](#apidoc.element.immutable.Iterable.prototype.takeLast)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>takeUntil (predicate, context)](#apidoc.element.immutable.Iterable.prototype.takeUntil)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>takeWhile (predicate, context)](#apidoc.element.immutable.Iterable.prototype.takeWhile)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toArray ()](#apidoc.element.immutable.Iterable.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toIndexedSeq ()](#apidoc.element.immutable.Iterable.prototype.toIndexedSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toJS ()](#apidoc.element.immutable.Iterable.prototype.toJS)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toJSON ()](#apidoc.element.immutable.Iterable.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Iterable.prototype.toKeyedSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toList ()](#apidoc.element.immutable.Iterable.prototype.toList)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toMap ()](#apidoc.element.immutable.Iterable.prototype.toMap)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toObject ()](#apidoc.element.immutable.Iterable.prototype.toObject)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toOrderedMap ()](#apidoc.element.immutable.Iterable.prototype.toOrderedMap)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toOrderedSet ()](#apidoc.element.immutable.Iterable.prototype.toOrderedSet)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSeq ()](#apidoc.element.immutable.Iterable.prototype.toSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSet ()](#apidoc.element.immutable.Iterable.prototype.toSet)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSetSeq ()](#apidoc.element.immutable.Iterable.prototype.toSetSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSource ()](#apidoc.element.immutable.Iterable.prototype.toSource)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toStack ()](#apidoc.element.immutable.Iterable.prototype.toStack)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toString ()](#apidoc.element.immutable.Iterable.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>valueSeq ()](#apidoc.element.immutable.Iterable.prototype.valueSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>values ()](#apidoc.element.immutable.Iterable.prototype.values)

#### [module immutable.List](#apidoc.module.immutable.List)
1.  [function <span class="apidocSignatureSpan">immutable.</span>List (value)](#apidoc.element.immutable.List.List)
1.  [function <span class="apidocSignatureSpan">immutable.List.</span>isList (maybeList)](#apidoc.element.immutable.List.isList)
1.  [function <span class="apidocSignatureSpan">immutable.List.</span>of ()](#apidoc.element.immutable.List.of)

#### [module immutable.List.prototype](#apidoc.module.immutable.List.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.List.prototype.__ensureOwner)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.List.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.List.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>asImmutable ()](#apidoc.element.immutable.List.prototype.asImmutable)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>asMutable ()](#apidoc.element.immutable.List.prototype.asMutable)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>clear ()](#apidoc.element.immutable.List.prototype.clear)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>constructor (value)](#apidoc.element.immutable.List.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>delete (index)](#apidoc.element.immutable.List.prototype.delete)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>deleteIn (keyPath)](#apidoc.element.immutable.List.prototype.deleteIn)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.List.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>insert (index, value)](#apidoc.element.immutable.List.prototype.insert)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>merge ()](#apidoc.element.immutable.List.prototype.merge)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeDeep ()](#apidoc.element.immutable.List.prototype.mergeDeep)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeDeepIn (keyPath)](#apidoc.element.immutable.List.prototype.mergeDeepIn)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.List.prototype.mergeDeepWith)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeIn (keyPath)](#apidoc.element.immutable.List.prototype.mergeIn)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.List.prototype.mergeWith)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>pop ()](#apidoc.element.immutable.List.prototype.pop)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>push ()](#apidoc.element.immutable.List.prototype.push)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>remove (index)](#apidoc.element.immutable.List.prototype.remove)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>removeIn (keyPath)](#apidoc.element.immutable.List.prototype.removeIn)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>set (index, value)](#apidoc.element.immutable.List.prototype.set)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>setIn (keyPath, v)](#apidoc.element.immutable.List.prototype.setIn)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>setSize (size)](#apidoc.element.immutable.List.prototype.setSize)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>shift ()](#apidoc.element.immutable.List.prototype.shift)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>slice (begin, end)](#apidoc.element.immutable.List.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>toString ()](#apidoc.element.immutable.List.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>unshift ()](#apidoc.element.immutable.List.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>update (k, notSetValue, updater)](#apidoc.element.immutable.List.prototype.update)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>updateIn (keyPath, notSetValue, updater)](#apidoc.element.immutable.List.prototype.updateIn)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>wasAltered ()](#apidoc.element.immutable.List.prototype.wasAltered)
1.  [function <span class="apidocSignatureSpan">immutable.List.prototype.</span>withMutations (fn)](#apidoc.element.immutable.List.prototype.withMutations)

#### [module immutable.Map](#apidoc.module.immutable.Map)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Map (value)](#apidoc.element.immutable.Map.Map)
1.  [function <span class="apidocSignatureSpan">immutable.Map.</span>isMap (maybeMap)](#apidoc.element.immutable.Map.isMap)
1.  [function <span class="apidocSignatureSpan">immutable.Map.</span>of ()](#apidoc.element.immutable.Map.of)

#### [module immutable.Map.prototype](#apidoc.module.immutable.Map.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Map.prototype.__ensureOwner)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Map.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Map.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>asImmutable ()](#apidoc.element.immutable.Map.prototype.asImmutable)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>asMutable ()](#apidoc.element.immutable.Map.prototype.asMutable)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>clear ()](#apidoc.element.immutable.Map.prototype.clear)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>constructor (value)](#apidoc.element.immutable.Map.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>delete (k)](#apidoc.element.immutable.Map.prototype.delete)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>deleteIn (keyPath)](#apidoc.element.immutable.Map.prototype.deleteIn)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>get (k, notSetValue)](#apidoc.element.immutable.Map.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>merge ()](#apidoc.element.immutable.Map.prototype.merge)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeDeep ()](#apidoc.element.immutable.Map.prototype.mergeDeep)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeDeepIn (keyPath)](#apidoc.element.immutable.Map.prototype.mergeDeepIn)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.Map.prototype.mergeDeepWith)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeIn (keyPath)](#apidoc.element.immutable.Map.prototype.mergeIn)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.Map.prototype.mergeWith)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>remove (k)](#apidoc.element.immutable.Map.prototype.remove)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>removeIn (keyPath)](#apidoc.element.immutable.Map.prototype.removeIn)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>set (k, v)](#apidoc.element.immutable.Map.prototype.set)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>setIn (keyPath, v)](#apidoc.element.immutable.Map.prototype.setIn)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>sort (comparator)](#apidoc.element.immutable.Map.prototype.sort)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>sortBy (mapper, comparator)](#apidoc.element.immutable.Map.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>toString ()](#apidoc.element.immutable.Map.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>update (k, notSetValue, updater)](#apidoc.element.immutable.Map.prototype.update)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>updateIn (keyPath, notSetValue, updater)](#apidoc.element.immutable.Map.prototype.updateIn)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>wasAltered ()](#apidoc.element.immutable.Map.prototype.wasAltered)
1.  [function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Map.prototype.withMutations)

#### [module immutable.OrderedMap](#apidoc.module.immutable.OrderedMap)
1.  [function <span class="apidocSignatureSpan">immutable.</span>OrderedMap (value)](#apidoc.element.immutable.OrderedMap.OrderedMap)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.</span>isOrderedMap (maybeOrderedMap)](#apidoc.element.immutable.OrderedMap.isOrderedMap)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.</span>of ()](#apidoc.element.immutable.OrderedMap.of)

#### [module immutable.OrderedMap.prototype](#apidoc.module.immutable.OrderedMap.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.OrderedMap.prototype.__ensureOwner)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.OrderedMap.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.OrderedMap.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>clear ()](#apidoc.element.immutable.OrderedMap.prototype.clear)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>constructor (value)](#apidoc.element.immutable.OrderedMap.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>delete (k)](#apidoc.element.immutable.OrderedMap.prototype.delete)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>get (k, notSetValue)](#apidoc.element.immutable.OrderedMap.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>remove (k)](#apidoc.element.immutable.OrderedMap.prototype.remove)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>set (k, v)](#apidoc.element.immutable.OrderedMap.prototype.set)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>toString ()](#apidoc.element.immutable.OrderedMap.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>wasAltered ()](#apidoc.element.immutable.OrderedMap.prototype.wasAltered)

#### [module immutable.OrderedSet](#apidoc.module.immutable.OrderedSet)
1.  [function <span class="apidocSignatureSpan">immutable.</span>OrderedSet (value)](#apidoc.element.immutable.OrderedSet.OrderedSet)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.</span>fromKeys (value)](#apidoc.element.immutable.OrderedSet.fromKeys)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.</span>isOrderedSet (maybeOrderedSet)](#apidoc.element.immutable.OrderedSet.isOrderedSet)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.</span>of ()](#apidoc.element.immutable.OrderedSet.of)

#### [module immutable.OrderedSet.prototype](#apidoc.module.immutable.OrderedSet.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>__empty ()](#apidoc.element.immutable.OrderedSet.prototype.__empty)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>__make (map, ownerID)](#apidoc.element.immutable.OrderedSet.prototype.__make)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>constructor (value)](#apidoc.element.immutable.OrderedSet.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>toString ()](#apidoc.element.immutable.OrderedSet.prototype.toString)

#### [module immutable.Range](#apidoc.module.immutable.Range)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Range (start, end, step)](#apidoc.element.immutable.Range.Range)

#### [module immutable.Range.prototype](#apidoc.module.immutable.Range.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Range.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Range.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>constructor (start, end, step)](#apidoc.element.immutable.Range.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>equals (other)](#apidoc.element.immutable.Range.prototype.equals)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Range.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>includes (searchValue)](#apidoc.element.immutable.Range.prototype.includes)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Range.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Range.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Range.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>toString ()](#apidoc.element.immutable.Range.prototype.toString)

#### [module immutable.Record](#apidoc.module.immutable.Record)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Record (defaultValues, name)](#apidoc.element.immutable.Record.Record)

#### [module immutable.Record.prototype](#apidoc.module.immutable.Record.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Record.prototype.__ensureOwner)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Record.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Record.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>asImmutable ()](#apidoc.element.immutable.Record.prototype.asImmutable)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>asMutable ()](#apidoc.element.immutable.Record.prototype.asMutable)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>clear ()](#apidoc.element.immutable.Record.prototype.clear)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>constructor (defaultValues, name)](#apidoc.element.immutable.Record.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>delete (k)](#apidoc.element.immutable.Record.prototype.delete)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>deleteIn (keyPath)](#apidoc.element.immutable.Record.prototype.deleteIn)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>get (k, notSetValue)](#apidoc.element.immutable.Record.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>has (k)](#apidoc.element.immutable.Record.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>merge ()](#apidoc.element.immutable.Record.prototype.merge)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeDeep ()](#apidoc.element.immutable.Record.prototype.mergeDeep)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeDeepIn (keyPath)](#apidoc.element.immutable.Record.prototype.mergeDeepIn)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.Record.prototype.mergeDeepWith)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeIn (keyPath)](#apidoc.element.immutable.Record.prototype.mergeIn)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.Record.prototype.mergeWith)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>remove (k)](#apidoc.element.immutable.Record.prototype.remove)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>removeIn (keyPath)](#apidoc.element.immutable.Record.prototype.removeIn)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>set (k, v)](#apidoc.element.immutable.Record.prototype.set)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>setIn (keyPath, v)](#apidoc.element.immutable.Record.prototype.setIn)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>toString ()](#apidoc.element.immutable.Record.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>update (k, notSetValue, updater)](#apidoc.element.immutable.Record.prototype.update)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>updateIn (keyPath, notSetValue, updater)](#apidoc.element.immutable.Record.prototype.updateIn)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>wasAltered ()](#apidoc.element.immutable.Record.prototype.wasAltered)
1.  [function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Record.prototype.withMutations)

#### [module immutable.Repeat](#apidoc.module.immutable.Repeat)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Repeat (value, times)](#apidoc.element.immutable.Repeat.Repeat)

#### [module immutable.Repeat.prototype](#apidoc.module.immutable.Repeat.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Repeat.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Repeat.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>constructor (value, times)](#apidoc.element.immutable.Repeat.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>equals (other)](#apidoc.element.immutable.Repeat.prototype.equals)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Repeat.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>includes (searchValue)](#apidoc.element.immutable.Repeat.prototype.includes)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Repeat.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Repeat.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>reverse ()](#apidoc.element.immutable.Repeat.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Repeat.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>toString ()](#apidoc.element.immutable.Repeat.prototype.toString)

#### [module immutable.Seq](#apidoc.module.immutable.Seq)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Seq (value)](#apidoc.element.immutable.Seq.Seq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>Indexed (value)](#apidoc.element.immutable.Seq.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>Keyed (value)](#apidoc.element.immutable.Seq.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>Set (value)](#apidoc.element.immutable.Seq.Set)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>isSeq (maybeSeq)](#apidoc.element.immutable.Seq.isSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>of ()](#apidoc.element.immutable.Seq.of)

#### [module immutable.Seq.Indexed](#apidoc.module.immutable.Seq.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>Indexed (value)](#apidoc.element.immutable.Seq.Indexed.Indexed)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.</span>of ()](#apidoc.element.immutable.Seq.Indexed.of)

#### [module immutable.Seq.Indexed.prototype](#apidoc.module.immutable.Seq.Indexed.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Seq.Indexed.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Seq.Indexed.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.Indexed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.filter)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>findIndex (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>findLastIndex (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.findLastIndex)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>first ()](#apidoc.element.immutable.Seq.Indexed.prototype.first)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>flatten (depth)](#apidoc.element.immutable.Seq.Indexed.prototype.flatten)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Seq.Indexed.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>has (index)](#apidoc.element.immutable.Seq.Indexed.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Seq.Indexed.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>interleave ()](#apidoc.element.immutable.Seq.Indexed.prototype.interleave)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>interpose (separator)](#apidoc.element.immutable.Seq.Indexed.prototype.interpose)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>keySeq ()](#apidoc.element.immutable.Seq.Indexed.prototype.keySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>last ()](#apidoc.element.immutable.Seq.Indexed.prototype.last)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Seq.Indexed.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>reverse ()](#apidoc.element.immutable.Seq.Indexed.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.skipWhile)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Seq.Indexed.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>splice (index, removeNum)](#apidoc.element.immutable.Seq.Indexed.prototype.splice)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>toIndexedSeq ()](#apidoc.element.immutable.Seq.Indexed.prototype.toIndexedSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Seq.Indexed.prototype.toKeyedSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>toString ()](#apidoc.element.immutable.Seq.Indexed.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>zip ()](#apidoc.element.immutable.Seq.Indexed.prototype.zip)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>zipWith (zipper)](#apidoc.element.immutable.Seq.Indexed.prototype.zipWith)

#### [module immutable.Seq.Keyed](#apidoc.module.immutable.Seq.Keyed)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>Keyed (value)](#apidoc.element.immutable.Seq.Keyed.Keyed)

#### [module immutable.Seq.Keyed.prototype](#apidoc.module.immutable.Seq.Keyed.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>__toJS ()](#apidoc.element.immutable.Seq.Keyed.prototype.__toJS)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>__toStringMapper (v, k)](#apidoc.element.immutable.Seq.Keyed.prototype.__toStringMapper)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.Keyed.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>flip ()](#apidoc.element.immutable.Seq.Keyed.prototype.flip)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>mapEntries (mapper, context)](#apidoc.element.immutable.Seq.Keyed.prototype.mapEntries)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>mapKeys (mapper, context)](#apidoc.element.immutable.Seq.Keyed.prototype.mapKeys)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Seq.Keyed.prototype.toKeyedSeq)

#### [module immutable.Seq.Set](#apidoc.module.immutable.Seq.Set)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.</span>Set (value)](#apidoc.element.immutable.Seq.Set.Set)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.</span>of ()](#apidoc.element.immutable.Seq.Set.of)

#### [module immutable.Seq.Set.prototype](#apidoc.module.immutable.Seq.Set.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>contains (value)](#apidoc.element.immutable.Seq.Set.prototype.contains)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>get (value, notSetValue)](#apidoc.element.immutable.Seq.Set.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>has (searchValue)](#apidoc.element.immutable.Seq.Set.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>includes (value)](#apidoc.element.immutable.Seq.Set.prototype.includes)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>keySeq ()](#apidoc.element.immutable.Seq.Set.prototype.keySeq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>toSetSeq ()](#apidoc.element.immutable.Seq.Set.prototype.toSetSeq)

#### [module immutable.Seq.prototype](#apidoc.module.immutable.Seq.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Seq.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Seq.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>cacheResult ()](#apidoc.element.immutable.Seq.prototype.cacheResult)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>toSeq ()](#apidoc.element.immutable.Seq.prototype.toSeq)
1.  [function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>toString ()](#apidoc.element.immutable.Seq.prototype.toString)

#### [module immutable.Set](#apidoc.module.immutable.Set)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Set (value)](#apidoc.element.immutable.Set.Set)
1.  [function <span class="apidocSignatureSpan">immutable.Set.</span>fromKeys (value)](#apidoc.element.immutable.Set.fromKeys)
1.  [function <span class="apidocSignatureSpan">immutable.Set.</span>isSet (maybeSet)](#apidoc.element.immutable.Set.isSet)
1.  [function <span class="apidocSignatureSpan">immutable.Set.</span>of ()](#apidoc.element.immutable.Set.of)

#### [module immutable.Set.prototype](#apidoc.module.immutable.Set.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__empty ()](#apidoc.element.immutable.Set.prototype.__empty)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Set.prototype.__ensureOwner)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Set.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Set.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__make (map, ownerID)](#apidoc.element.immutable.Set.prototype.__make)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>add (value)](#apidoc.element.immutable.Set.prototype.add)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>asImmutable ()](#apidoc.element.immutable.Set.prototype.asImmutable)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>asMutable ()](#apidoc.element.immutable.Set.prototype.asMutable)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>clear ()](#apidoc.element.immutable.Set.prototype.clear)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>delete (value)](#apidoc.element.immutable.Set.prototype.delete)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>has (value)](#apidoc.element.immutable.Set.prototype.has)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>intersect ()](#apidoc.element.immutable.Set.prototype.intersect)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>merge ()](#apidoc.element.immutable.Set.prototype.merge)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>mergeDeep ()](#apidoc.element.immutable.Set.prototype.mergeDeep)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.Set.prototype.mergeDeepWith)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.Set.prototype.mergeWith)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>remove (value)](#apidoc.element.immutable.Set.prototype.remove)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>sort (comparator)](#apidoc.element.immutable.Set.prototype.sort)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>sortBy (mapper, comparator)](#apidoc.element.immutable.Set.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>subtract ()](#apidoc.element.immutable.Set.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>toString ()](#apidoc.element.immutable.Set.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>union ()](#apidoc.element.immutable.Set.prototype.union)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>wasAltered ()](#apidoc.element.immutable.Set.prototype.wasAltered)
1.  [function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Set.prototype.withMutations)

#### [module immutable.Stack](#apidoc.module.immutable.Stack)
1.  [function <span class="apidocSignatureSpan">immutable.</span>Stack (value)](#apidoc.element.immutable.Stack.Stack)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.</span>isStack (maybeStack)](#apidoc.element.immutable.Stack.isStack)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.</span>of ()](#apidoc.element.immutable.Stack.of)

#### [module immutable.Stack.prototype](#apidoc.module.immutable.Stack.prototype)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Stack.prototype.__ensureOwner)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Stack.prototype.__iterate)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Stack.prototype.__iterator)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>asImmutable ()](#apidoc.element.immutable.Stack.prototype.asImmutable)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>asMutable ()](#apidoc.element.immutable.Stack.prototype.asMutable)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>clear ()](#apidoc.element.immutable.Stack.prototype.clear)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>constructor (value)](#apidoc.element.immutable.Stack.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Stack.prototype.get)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>peek ()](#apidoc.element.immutable.Stack.prototype.peek)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>pop ()](#apidoc.element.immutable.Stack.prototype.pop)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>push ()](#apidoc.element.immutable.Stack.prototype.push)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>pushAll (iter)](#apidoc.element.immutable.Stack.prototype.pushAll)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>shift ()](#apidoc.element.immutable.Stack.prototype.shift)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Stack.prototype.slice)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>toString ()](#apidoc.element.immutable.Stack.prototype.toString)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>unshift ()](#apidoc.element.immutable.Stack.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>unshiftAll (iter)](#apidoc.element.immutable.Stack.prototype.unshiftAll)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>wasAltered ()](#apidoc.element.immutable.Stack.prototype.wasAltered)
1.  [function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Stack.prototype.withMutations)



# <a name="apidoc.module.immutable"></a>[module immutable](#apidoc.module.immutable)

#### <a name="apidoc.element.immutable.Collection"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection ()](#apidoc.element.immutable.Collection)
- description and source-code
```javascript
function Collection() {
  throw TypeError('Abstract');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection.Indexed ()](#apidoc.element.immutable.Collection.Indexed)
- description and source-code
```javascript
function IndexedCollection() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection.Indexed.prototype.constructor (value)](#apidoc.element.immutable.Collection.Indexed.prototype.constructor)
- description and source-code
```javascript
function IndexedIterable(value) {
  return isIndexed(value) ? value : IndexedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection.Keyed ()](#apidoc.element.immutable.Collection.Keyed)
- description and source-code
```javascript
function KeyedCollection() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection.Keyed.prototype.constructor (value)](#apidoc.element.immutable.Collection.Keyed.prototype.constructor)
- description and source-code
```javascript
function KeyedIterable(value) {
  return isKeyed(value) ? value : KeyedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection.Set ()](#apidoc.element.immutable.Collection.Set)
- description and source-code
```javascript
function SetCollection() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection.Set.prototype.constructor (value)](#apidoc.element.immutable.Collection.Set.prototype.constructor)
- description and source-code
```javascript
function SetIterable(value) {
  return isIterable(value) && !isAssociative(value) ? value : SetSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable"></a>[function <span class="apidocSignatureSpan">immutable.</span>Iterable (value)](#apidoc.element.immutable.Iterable)
- description and source-code
```javascript
function Iterable(value) {
  return isIterable(value) ? value : Seq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Iterator"></a>[function <span class="apidocSignatureSpan">immutable.</span>Iterable.Iterator (next)](#apidoc.element.immutable.Iterable.Iterator)
- description and source-code
```javascript
function Iterator(next) {
  this.next = next;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List"></a>[function <span class="apidocSignatureSpan">immutable.</span>List (value)](#apidoc.element.immutable.List)
- description and source-code
```javascript
function List(value) {
  var empty = emptyList();
  if (value === null || value === undefined) {
    return empty;
  }
  if (isList(value)) {
    return value;
  }
  var iter = IndexedIterable(value);
  var size = iter.size;
  if (size === 0) {
    return empty;
  }
  assertNotInfinite(size);
  if (size > 0 && size < SIZE) {
    return makeList(0, size, SHIFT, null, new VNode(iter.toArray()));
  }
  return empty.withMutations(function(list ) {
    list.setSize(size);
    iter.forEach(function(v, i)  {return list.set(i, v)});
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map"></a>[function <span class="apidocSignatureSpan">immutable.</span>Map (value)](#apidoc.element.immutable.Map)
- description and source-code
```javascript
function Map(value) {
  return value === null || value === undefined ? emptyMap() :
    isMap(value) && !isOrdered(value) ? value :
    emptyMap().withMutations(function(map ) {
      var iter = KeyedIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v, k)  {return map.set(k, v)});
    });
}
```
- example usage
```shell
...
npm install immutable
'''

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser
...
```

#### <a name="apidoc.element.immutable.OrderedMap"></a>[function <span class="apidocSignatureSpan">immutable.</span>OrderedMap (value)](#apidoc.element.immutable.OrderedMap)
- description and source-code
```javascript
function OrderedMap(value) {
  return value === null || value === undefined ? emptyOrderedMap() :
    isOrderedMap(value) ? value :
    emptyOrderedMap().withMutations(function(map ) {
      var iter = KeyedIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v, k)  {return map.set(k, v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet"></a>[function <span class="apidocSignatureSpan">immutable.</span>OrderedSet (value)](#apidoc.element.immutable.OrderedSet)
- description and source-code
```javascript
function OrderedSet(value) {
  return value === null || value === undefined ? emptyOrderedSet() :
    isOrderedSet(value) ? value :
    emptyOrderedSet().withMutations(function(set ) {
      var iter = SetIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v ) {return set.add(v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range"></a>[function <span class="apidocSignatureSpan">immutable.</span>Range (start, end, step)](#apidoc.element.immutable.Range)
- description and source-code
```javascript
function Range(start, end, step) {
  if (!(this instanceof Range)) {
    return new Range(start, end, step);
  }
  invariant(step !== 0, 'Cannot step a Range by 0');
  start = start || 0;
  if (end === undefined) {
    end = Infinity;
  }
  step = step === undefined ? 1 : Math.abs(step);
  if (end < start) {
    step = -step;
  }
  this._start = start;
  this._end = end;
  this._step = step;
  this.size = Math.max(0, Math.ceil((end - start) / step - 1) + 1);
  if (this.size === 0) {
    if (EMPTY_RANGE) {
      return EMPTY_RANGE;
    }
    EMPTY_RANGE = this;
  }
}
```
- example usage
```shell
...
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
// Map { A: 1, B: 1, C: 1 }

As well as expressing logic that would otherwise seem memory-limited:

Immutable.Range(1, Infinity)
  .skip(1000)
  .map(n => -n)
  .filter(n => n % 2 === 0)
  .take(2)
  .reduce((r, n) => r * n, 1);
// 1006008
...
```

#### <a name="apidoc.element.immutable.Record"></a>[function <span class="apidocSignatureSpan">immutable.</span>Record (defaultValues, name)](#apidoc.element.immutable.Record)
- description and source-code
```javascript
function Record(defaultValues, name) {
  var hasInitialized;

  var RecordType = function Record(values) {
    if (values instanceof RecordType) {
      return values;
    }
    if (!(this instanceof RecordType)) {
      return new RecordType(values);
    }
    if (!hasInitialized) {
      hasInitialized = true;
      var keys = Object.keys(defaultValues);
      setProps(RecordTypePrototype, keys);
      RecordTypePrototype.size = keys.length;
      RecordTypePrototype._name = name;
      RecordTypePrototype._keys = keys;
      RecordTypePrototype._defaultValues = defaultValues;
    }
    this._map = Map(values);
  };

  var RecordTypePrototype = RecordType.prototype = Object.create(RecordPrototype);
  RecordTypePrototype.constructor = RecordType;

  return RecordType;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat"></a>[function <span class="apidocSignatureSpan">immutable.</span>Repeat (value, times)](#apidoc.element.immutable.Repeat)
- description and source-code
```javascript
function Repeat(value, times) {
  if (!(this instanceof Repeat)) {
    return new Repeat(value, times);
  }
  this._value = value;
  this.size = times === undefined ? Infinity : Math.max(0, times);
  if (this.size === 0) {
    if (EMPTY_REPEAT) {
      return EMPTY_REPEAT;
    }
    EMPTY_REPEAT = this;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq"></a>[function <span class="apidocSignatureSpan">immutable.</span>Seq (value)](#apidoc.element.immutable.Seq)
- description and source-code
```javascript
function Seq(value) {
  return value === null || value === undefined ? emptySequence() :
    isIterable(value) ? value.toSeq() : seqFromValue(value);
}
```
- example usage
```shell
...
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
results, these operations can be extremely efficient.

'''javascript
var myObject = {a:1,b:2,c:3};
Immutable.Seq(myObject).map(x => x * x).toObject();
// { a: 1, b: 4, c: 9 }
'''

Keep in mind, when using JS objects to construct Immutable Maps, that
JavaScript Object properties are always strings, even if written in a quote-less
shorthand, while Immutable Maps accept keys of any type.
...
```

#### <a name="apidoc.element.immutable.Seq.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.</span>Seq.Indexed (value)](#apidoc.element.immutable.Seq.Indexed)
- description and source-code
```javascript
function IndexedSeq(value) {
  return value === null || value === undefined ? emptySequence() :
    !isIterable(value) ? indexedSeqFromValue(value) :
    isKeyed(value) ? value.entrySeq() : value.toIndexedSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.</span>Seq.Keyed (value)](#apidoc.element.immutable.Seq.Keyed)
- description and source-code
```javascript
function KeyedSeq(value) {
  return value === null || value === undefined ?
    emptySequence().toKeyedSeq() :
    isIterable(value) ?
      (isKeyed(value) ? value.toSeq() : value.fromEntrySeq()) :
      keyedSeqFromValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set"></a>[function <span class="apidocSignatureSpan">immutable.</span>Seq.Set (value)](#apidoc.element.immutable.Seq.Set)
- description and source-code
```javascript
function SetSeq(value) {
  return (
    value === null || value === undefined ? emptySequence() :
    !isIterable(value) ? indexedSeqFromValue(value) :
    isKeyed(value) ? value.entrySeq() : value
  ).toSetSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set"></a>[function <span class="apidocSignatureSpan">immutable.</span>Set (value)](#apidoc.element.immutable.Set)
- description and source-code
```javascript
function Set(value) {
  return value === null || value === undefined ? emptySet() :
    isSet(value) && !isOrdered(value) ? value :
    emptySet().withMutations(function(set ) {
      var iter = SetIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v ) {return set.add(v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack"></a>[function <span class="apidocSignatureSpan">immutable.</span>Stack (value)](#apidoc.element.immutable.Stack)
- description and source-code
```javascript
function Stack(value) {
  return value === null || value === undefined ? emptyStack() :
    isStack(value) ? value :
    emptyStack().unshiftAll(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.fromJS"></a>[function <span class="apidocSignatureSpan">immutable.</span>fromJS (json, converter)](#apidoc.element.immutable.fromJS)
- description and source-code
```javascript
function fromJS(json, converter) {
  return converter ?
    fromJSWith(converter, json, '', {'': json}) :
    fromJSDefault(json);
}
```
- example usage
```shell
...

'''js
var obj = { 1: "one" };
Object.keys(obj); // [ "1" ]
obj["1"]; // "one"
obj[1];   // "one"

var map = Immutable.fromJS(obj);
map.get("1"); // "one"
map.get(1);   // undefined
'''

Property access for JavaScript Objects first converts the key to a string, but
since Immutable Map keys can be of any type the argument to 'get()' is
not altered.
...
```

#### <a name="apidoc.element.immutable.is"></a>[function <span class="apidocSignatureSpan">immutable.</span>is (valueA, valueB)](#apidoc.element.immutable.is)
- description and source-code
```javascript
function is(valueA, valueB) {
  if (valueA === valueB || (valueA !== valueA && valueB !== valueB)) {
    return true;
  }
  if (!valueA || !valueB) {
    return false;
  }
  if (typeof valueA.valueOf === 'function' &&
      typeof valueB.valueOf === 'function') {
    valueA = valueA.valueOf();
    valueB = valueB.valueOf();
    if (valueA === valueB || (valueA !== valueA && valueB !== valueB)) {
      return true;
    }
    if (!valueA || !valueB) {
      return false;
    }
  }
  if (typeof valueA.equals === 'function' &&
      typeof valueB.equals === 'function' &&
      valueA.equals(valueB)) {
    return true;
  }
  return false;
}
```
- example usage
```shell
...
interested in doing work when something has changed, you can use equality.

Immutable collections should be treated as *values* rather than *objects*. While
objects represents some thing which could change over time, a value represents
the state of that thing at a particular instance of time. This principle is most
important to understanding the appropriate use of immutable data. In order to
treat Immutable.js collections as values, it's important to use the
'Immutable.is()' function or '.equals()' method to determine value equality
instead of the '===' operator which determines object reference identity.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 2);
assert(map1.equals(map2) === true);
var map3 = map1.set('b', 50);
...
```



# <a name="apidoc.module.immutable.Collection"></a>[module immutable.Collection](#apidoc.module.immutable.Collection)

#### <a name="apidoc.element.immutable.Collection.Collection"></a>[function <span class="apidocSignatureSpan">immutable.</span>Collection ()](#apidoc.element.immutable.Collection.Collection)
- description and source-code
```javascript
function Collection() {
  throw TypeError('Abstract');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.Collection.</span>Indexed ()](#apidoc.element.immutable.Collection.Indexed)
- description and source-code
```javascript
function IndexedCollection() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.Collection.</span>Keyed ()](#apidoc.element.immutable.Collection.Keyed)
- description and source-code
```javascript
function KeyedCollection() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set"></a>[function <span class="apidocSignatureSpan">immutable.Collection.</span>Set ()](#apidoc.element.immutable.Collection.Set)
- description and source-code
```javascript
function SetCollection() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Indexed"></a>[module immutable.Collection.Indexed](#apidoc.module.immutable.Collection.Indexed)

#### <a name="apidoc.element.immutable.Collection.Indexed.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.Collection.</span>Indexed ()](#apidoc.element.immutable.Collection.Indexed.Indexed)
- description and source-code
```javascript
function IndexedCollection() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Indexed.prototype"></a>[module immutable.Collection.Indexed.prototype](#apidoc.module.immutable.Collection.Indexed.prototype)

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>constructor (value)](#apidoc.element.immutable.Collection.Indexed.prototype.constructor)
- description and source-code
```javascript
function IndexedIterable(value) {
  return isIndexed(value) ? value : IndexedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.filter"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.filter)
- description and source-code
```javascript
filter = function (predicate, context) {
  return reify(this, filterFactory(this, predicate, context, false));
}
```
- example usage
```shell
...
**Seq is lazy** — Seq does as little work as necessary to respond to any
method call.

For example, the following does not perform any work, because the resulting
Seq is never used:

var oddSquares = Immutable.Seq.of(1,2,3,4,5,6,7,8)
  .filter(x => x % 2).map(x => x * x);

Once the Seq is used, it performs only the work necessary. In this
example, no intermediate arrays are ever created, filter is called three times,
and map is only called twice:

console.log(oddSquares.get(1)); // 9
...
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>findIndex (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.findIndex)
- description and source-code
```javascript
findIndex = function (predicate, context) {
  var entry = this.findEntry(predicate, context);
  return entry ? entry[0] : -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.findLastIndex"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>findLastIndex (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.findLastIndex)
- description and source-code
```javascript
findLastIndex = function (predicate, context) {
  var entry = this.findLastEntry(predicate, context);
  return entry ? entry[0] : -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.first"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>first ()](#apidoc.element.immutable.Collection.Indexed.prototype.first)
- description and source-code
```javascript
first = function () {
  return this.get(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.flatten"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>flatten (depth)](#apidoc.element.immutable.Collection.Indexed.prototype.flatten)
- description and source-code
```javascript
flatten = function (depth) {
  return reify(this, flattenFactory(this, depth, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Collection.Indexed.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  index = wrapIndex(this, index);
  return (index < 0 || (this.size === Infinity ||
      (this.size !== undefined && index > this.size))) ?
    notSetValue :
    this.find(function(_, key)  {return key === index}, undefined, notSetValue);
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>has (index)](#apidoc.element.immutable.Collection.Indexed.prototype.has)
- description and source-code
```javascript
has = function (index) {
  index = wrapIndex(this, index);
  return index >= 0 && (this.size !== undefined ?
    this.size === Infinity || index < this.size :
    this.indexOf(index) !== -1
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Collection.Indexed.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (searchValue) {
  var key = this.keyOf(searchValue);
  return key === undefined ? -1 : key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.interleave"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>interleave ()](#apidoc.element.immutable.Collection.Indexed.prototype.interleave)
- description and source-code
```javascript
interleave = function () {
  var iterables = [this].concat(arrCopy(arguments));
  var zipped = zipWithFactory(this.toSeq(), IndexedSeq.of, iterables);
  var interleaved = zipped.flatten(true);
  if (zipped.size) {
    interleaved.size = zipped.size * iterables.length;
  }
  return reify(this, interleaved);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.interpose"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>interpose (separator)](#apidoc.element.immutable.Collection.Indexed.prototype.interpose)
- description and source-code
```javascript
interpose = function (separator) {
  return reify(this, interposeFactory(this, separator));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>keySeq ()](#apidoc.element.immutable.Collection.Indexed.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return Range(0, this.size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.last"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>last ()](#apidoc.element.immutable.Collection.Indexed.prototype.last)
- description and source-code
```javascript
last = function () {
  return this.get(-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Collection.Indexed.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (searchValue) {
  var key = this.lastKeyOf(searchValue);
  return key === undefined ? -1 : key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.reverse"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>reverse ()](#apidoc.element.immutable.Collection.Indexed.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  return reify(this, reverseFactory(this, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.skipWhile"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Collection.Indexed.prototype.skipWhile)
- description and source-code
```javascript
skipWhile = function (predicate, context) {
  return reify(this, skipWhileFactory(this, predicate, context, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Collection.Indexed.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  return reify(this, sliceFactory(this, begin, end, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.splice"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>splice (index, removeNum)](#apidoc.element.immutable.Collection.Indexed.prototype.splice)
- description and source-code
```javascript
splice = function (index, removeNum) {
  var numArgs = arguments.length;
  removeNum = Math.max(removeNum | 0, 0);
  if (numArgs === 0 || (numArgs === 2 && !removeNum)) {
    return this;
  }
  // If index is negative, it should resolve relative to the size of the
  // collection. However size may be expensive to compute if not cached, so
  // only call count() if the number is in fact negative.
  index = resolveBegin(index, index < 0 ? this.count() : this.size);
  var spliced = this.slice(0, index);
  return reify(
    this,
    numArgs === 1 ?
      spliced :
      spliced.concat(arrCopy(arguments, 2), this.slice(index + removeNum))
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.toKeyedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Collection.Indexed.prototype.toKeyedSeq)
- description and source-code
```javascript
toKeyedSeq = function () {
  return new ToKeyedSequence(this, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.zip"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>zip ()](#apidoc.element.immutable.Collection.Indexed.prototype.zip)
- description and source-code
```javascript
zip = function () {
  var iterables = [this].concat(arrCopy(arguments));
  return reify(this, zipWithFactory(this, defaultZipper, iterables));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.zipWith"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>zipWith (zipper)](#apidoc.element.immutable.Collection.Indexed.prototype.zipWith)
- description and source-code
```javascript
zipWith = function (zipper) {
  var iterables = arrCopy(arguments);
  iterables[0] = this;
  return reify(this, zipWithFactory(this, zipper, iterables));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Indexed.prototype.constructor"></a>[module immutable.Collection.Indexed.prototype.constructor](#apidoc.module.immutable.Collection.Indexed.prototype.constructor)

#### <a name="apidoc.element.immutable.Collection.Indexed.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Indexed.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.Indexed.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Keyed"></a>[module immutable.Collection.Keyed](#apidoc.module.immutable.Collection.Keyed)

#### <a name="apidoc.element.immutable.Collection.Keyed.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.Collection.</span>Keyed ()](#apidoc.element.immutable.Collection.Keyed.Keyed)
- description and source-code
```javascript
function KeyedCollection() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Keyed.prototype"></a>[module immutable.Collection.Keyed.prototype](#apidoc.module.immutable.Collection.Keyed.prototype)

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.__toJS"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>__toJS ()](#apidoc.element.immutable.Collection.Keyed.prototype.__toJS)
- description and source-code
```javascript
__toJS = function () {
  assertNotInfinite(this.size);
  var object = {};
  this.__iterate(function(v, k)  { object[k] = v; });
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.__toStringMapper"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>__toStringMapper (v, k)](#apidoc.element.immutable.Collection.Keyed.prototype.__toStringMapper)
- description and source-code
```javascript
__toStringMapper = function (v, k)  {return JSON.stringify(k) + ': ' + quoteString(v)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>constructor (value)](#apidoc.element.immutable.Collection.Keyed.prototype.constructor)
- description and source-code
```javascript
function KeyedIterable(value) {
  return isKeyed(value) ? value : KeyedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.flip"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>flip ()](#apidoc.element.immutable.Collection.Keyed.prototype.flip)
- description and source-code
```javascript
flip = function () {
  return reify(this, flipFactory(this));
}
```
- example usage
```shell
...
Any collection can be converted to a lazy Seq with '.toSeq()'.

var seq = Immutable.Map({a:1, b:1, c:1}).toSeq();

Seq allow for the efficient chaining of sequence operations, especially when
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
// Map { A: 1, B: 1, C: 1 }

As well as expressing logic that would otherwise seem memory-limited:

Immutable.Range(1, Infinity)
  .skip(1000)
  .map(n => -n)
...
```

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.mapEntries"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>mapEntries (mapper, context)](#apidoc.element.immutable.Collection.Keyed.prototype.mapEntries)
- description and source-code
```javascript
mapEntries = function (mapper, context) {var this$0 = this;
  var iterations = 0;
  return reify(this,
    this.toSeq().map(
      function(v, k)  {return mapper.call(context, [k, v], iterations++, this$0)}
    ).fromEntrySeq()
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.mapKeys"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>mapKeys (mapper, context)](#apidoc.element.immutable.Collection.Keyed.prototype.mapKeys)
- description and source-code
```javascript
mapKeys = function (mapper, context) {var this$0 = this;
  return reify(this,
    this.toSeq().flip().map(
      function(k, v)  {return mapper.call(context, k, v, this$0)}
    ).flip()
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Keyed.prototype.constructor"></a>[module immutable.Collection.Keyed.prototype.constructor](#apidoc.module.immutable.Collection.Keyed.prototype.constructor)

#### <a name="apidoc.element.immutable.Collection.Keyed.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Keyed.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.Keyed.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Set"></a>[module immutable.Collection.Set](#apidoc.module.immutable.Collection.Set)

#### <a name="apidoc.element.immutable.Collection.Set.Set"></a>[function <span class="apidocSignatureSpan">immutable.Collection.</span>Set ()](#apidoc.element.immutable.Collection.Set.Set)
- description and source-code
```javascript
function SetCollection() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Set.prototype"></a>[module immutable.Collection.Set.prototype](#apidoc.module.immutable.Collection.Set.prototype)

#### <a name="apidoc.element.immutable.Collection.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Collection.Set.prototype.constructor)
- description and source-code
```javascript
function SetIterable(value) {
  return isIterable(value) && !isAssociative(value) ? value : SetSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set.prototype.contains"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>contains (value)](#apidoc.element.immutable.Collection.Set.prototype.contains)
- description and source-code
```javascript
contains = function (value) {
  return this.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>get (value, notSetValue)](#apidoc.element.immutable.Collection.Set.prototype.get)
- description and source-code
```javascript
get = function (value, notSetValue) {
  return this.has(value) ? value : notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Collection.Set.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>has (searchValue)](#apidoc.element.immutable.Collection.Set.prototype.has)
- description and source-code
```javascript
has = function (searchValue) {
  return this.some(function(value ) {return is(value, searchValue)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set.prototype.includes"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>includes (value)](#apidoc.element.immutable.Collection.Set.prototype.includes)
- description and source-code
```javascript
includes = function (value) {
  return this.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Collection.Set.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>keySeq ()](#apidoc.element.immutable.Collection.Set.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return this.valueSeq();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.Set.prototype.constructor"></a>[module immutable.Collection.Set.prototype.constructor](#apidoc.module.immutable.Collection.Set.prototype.constructor)

#### <a name="apidoc.element.immutable.Collection.Set.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.Set.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.Set.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Collection.prototype"></a>[module immutable.Collection.prototype](#apidoc.module.immutable.Collection.prototype)

#### <a name="apidoc.element.immutable.Collection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Collection.prototype.</span>constructor ()](#apidoc.element.immutable.Collection.prototype.constructor)
- description and source-code
```javascript
function Collection() {
  throw TypeError('Abstract');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable"></a>[module immutable.Iterable](#apidoc.module.immutable.Iterable)

#### <a name="apidoc.element.immutable.Iterable.Iterable"></a>[function <span class="apidocSignatureSpan">immutable.</span>Iterable (value)](#apidoc.element.immutable.Iterable.Iterable)
- description and source-code
```javascript
function Iterable(value) {
  return isIterable(value) ? value : Seq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>Indexed (value)](#apidoc.element.immutable.Iterable.Indexed)
- description and source-code
```javascript
function IndexedIterable(value) {
  return isIndexed(value) ? value : IndexedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Iterator"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>Iterator (next)](#apidoc.element.immutable.Iterable.Iterator)
- description and source-code
```javascript
function Iterator(next) {
  this.next = next;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>Keyed (value)](#apidoc.element.immutable.Iterable.Keyed)
- description and source-code
```javascript
function KeyedIterable(value) {
  return isKeyed(value) ? value : KeyedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Set"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>Set (value)](#apidoc.element.immutable.Iterable.Set)
- description and source-code
```javascript
function SetIterable(value) {
  return isIterable(value) && !isAssociative(value) ? value : SetSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.isAssociative"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>isAssociative (maybeAssociative)](#apidoc.element.immutable.Iterable.isAssociative)
- description and source-code
```javascript
function isAssociative(maybeAssociative) {
  return isKeyed(maybeAssociative) || isIndexed(maybeAssociative);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.isIndexed"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>isIndexed (maybeIndexed)](#apidoc.element.immutable.Iterable.isIndexed)
- description and source-code
```javascript
function isIndexed(maybeIndexed) {
  return !!(maybeIndexed && maybeIndexed[IS_INDEXED_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.isIterable"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>isIterable (maybeIterable)](#apidoc.element.immutable.Iterable.isIterable)
- description and source-code
```javascript
function isIterable(maybeIterable) {
  return !!(maybeIterable && maybeIterable[IS_ITERABLE_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.isKeyed"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>isKeyed (maybeKeyed)](#apidoc.element.immutable.Iterable.isKeyed)
- description and source-code
```javascript
function isKeyed(maybeKeyed) {
  return !!(maybeKeyed && maybeKeyed[IS_KEYED_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.isOrdered"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>isOrdered (maybeOrdered)](#apidoc.element.immutable.Iterable.isOrdered)
- description and source-code
```javascript
function isOrdered(maybeOrdered) {
  return !!(maybeOrdered && maybeOrdered[IS_ORDERED_SENTINEL]);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable.Indexed.prototype"></a>[module immutable.Iterable.Indexed.prototype](#apidoc.module.immutable.Iterable.Indexed.prototype)

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>constructor (value)](#apidoc.element.immutable.Iterable.Indexed.prototype.constructor)
- description and source-code
```javascript
function IndexedIterable(value) {
  return isIndexed(value) ? value : IndexedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.filter"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.filter)
- description and source-code
```javascript
filter = function (predicate, context) {
  return reify(this, filterFactory(this, predicate, context, false));
}
```
- example usage
```shell
...
**Seq is lazy** — Seq does as little work as necessary to respond to any
method call.

For example, the following does not perform any work, because the resulting
Seq is never used:

var oddSquares = Immutable.Seq.of(1,2,3,4,5,6,7,8)
  .filter(x => x % 2).map(x => x * x);

Once the Seq is used, it performs only the work necessary. In this
example, no intermediate arrays are ever created, filter is called three times,
and map is only called twice:

console.log(oddSquares.get(1)); // 9
...
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>findIndex (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.findIndex)
- description and source-code
```javascript
findIndex = function (predicate, context) {
  var entry = this.findEntry(predicate, context);
  return entry ? entry[0] : -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.findLastIndex"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>findLastIndex (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.findLastIndex)
- description and source-code
```javascript
findLastIndex = function (predicate, context) {
  var entry = this.findLastEntry(predicate, context);
  return entry ? entry[0] : -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.first"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>first ()](#apidoc.element.immutable.Iterable.Indexed.prototype.first)
- description and source-code
```javascript
first = function () {
  return this.get(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.flatten"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>flatten (depth)](#apidoc.element.immutable.Iterable.Indexed.prototype.flatten)
- description and source-code
```javascript
flatten = function (depth) {
  return reify(this, flattenFactory(this, depth, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Iterable.Indexed.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  index = wrapIndex(this, index);
  return (index < 0 || (this.size === Infinity ||
      (this.size !== undefined && index > this.size))) ?
    notSetValue :
    this.find(function(_, key)  {return key === index}, undefined, notSetValue);
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>has (index)](#apidoc.element.immutable.Iterable.Indexed.prototype.has)
- description and source-code
```javascript
has = function (index) {
  index = wrapIndex(this, index);
  return index >= 0 && (this.size !== undefined ?
    this.size === Infinity || index < this.size :
    this.indexOf(index) !== -1
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Iterable.Indexed.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (searchValue) {
  var key = this.keyOf(searchValue);
  return key === undefined ? -1 : key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.interleave"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>interleave ()](#apidoc.element.immutable.Iterable.Indexed.prototype.interleave)
- description and source-code
```javascript
interleave = function () {
  var iterables = [this].concat(arrCopy(arguments));
  var zipped = zipWithFactory(this.toSeq(), IndexedSeq.of, iterables);
  var interleaved = zipped.flatten(true);
  if (zipped.size) {
    interleaved.size = zipped.size * iterables.length;
  }
  return reify(this, interleaved);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.interpose"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>interpose (separator)](#apidoc.element.immutable.Iterable.Indexed.prototype.interpose)
- description and source-code
```javascript
interpose = function (separator) {
  return reify(this, interposeFactory(this, separator));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>keySeq ()](#apidoc.element.immutable.Iterable.Indexed.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return Range(0, this.size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.last"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>last ()](#apidoc.element.immutable.Iterable.Indexed.prototype.last)
- description and source-code
```javascript
last = function () {
  return this.get(-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Iterable.Indexed.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (searchValue) {
  var key = this.lastKeyOf(searchValue);
  return key === undefined ? -1 : key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.reverse"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>reverse ()](#apidoc.element.immutable.Iterable.Indexed.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  return reify(this, reverseFactory(this, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.skipWhile"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Iterable.Indexed.prototype.skipWhile)
- description and source-code
```javascript
skipWhile = function (predicate, context) {
  return reify(this, skipWhileFactory(this, predicate, context, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Iterable.Indexed.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  return reify(this, sliceFactory(this, begin, end, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.splice"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>splice (index, removeNum)](#apidoc.element.immutable.Iterable.Indexed.prototype.splice)
- description and source-code
```javascript
splice = function (index, removeNum) {
  var numArgs = arguments.length;
  removeNum = Math.max(removeNum | 0, 0);
  if (numArgs === 0 || (numArgs === 2 && !removeNum)) {
    return this;
  }
  // If index is negative, it should resolve relative to the size of the
  // collection. However size may be expensive to compute if not cached, so
  // only call count() if the number is in fact negative.
  index = resolveBegin(index, index < 0 ? this.count() : this.size);
  var spliced = this.slice(0, index);
  return reify(
    this,
    numArgs === 1 ?
      spliced :
      spliced.concat(arrCopy(arguments, 2), this.slice(index + removeNum))
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.toKeyedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Iterable.Indexed.prototype.toKeyedSeq)
- description and source-code
```javascript
toKeyedSeq = function () {
  return new ToKeyedSequence(this, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.zip"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>zip ()](#apidoc.element.immutable.Iterable.Indexed.prototype.zip)
- description and source-code
```javascript
zip = function () {
  var iterables = [this].concat(arrCopy(arguments));
  return reify(this, zipWithFactory(this, defaultZipper, iterables));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Indexed.prototype.zipWith"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Indexed.prototype.</span>zipWith (zipper)](#apidoc.element.immutable.Iterable.Indexed.prototype.zipWith)
- description and source-code
```javascript
zipWith = function (zipper) {
  var iterables = arrCopy(arguments);
  iterables[0] = this;
  return reify(this, zipWithFactory(this, zipper, iterables));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable.Iterator"></a>[module immutable.Iterable.Iterator](#apidoc.module.immutable.Iterable.Iterator)

#### <a name="apidoc.element.immutable.Iterable.Iterator.Iterator"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.</span>Iterator (next)](#apidoc.element.immutable.Iterable.Iterator.Iterator)
- description and source-code
```javascript
function Iterator(next) {
  this.next = next;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable.Iterator.prototype"></a>[module immutable.Iterable.Iterator.prototype](#apidoc.module.immutable.Iterable.Iterator.prototype)

#### <a name="apidoc.element.immutable.Iterable.Iterator.prototype.inspect"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Iterator.prototype.</span>inspect ()](#apidoc.element.immutable.Iterable.Iterator.prototype.inspect)
- description and source-code
```javascript
inspect = function () { return this.toString(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Iterator.prototype.toSource"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Iterator.prototype.</span>toSource ()](#apidoc.element.immutable.Iterable.Iterator.prototype.toSource)
- description and source-code
```javascript
toSource = function () { return this.toString(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Iterator.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Iterator.prototype.</span>toString ()](#apidoc.element.immutable.Iterable.Iterator.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return '[Iterator]';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable.Keyed.prototype"></a>[module immutable.Iterable.Keyed.prototype](#apidoc.module.immutable.Iterable.Keyed.prototype)

#### <a name="apidoc.element.immutable.Iterable.Keyed.prototype.__toJS"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>__toJS ()](#apidoc.element.immutable.Iterable.Keyed.prototype.__toJS)
- description and source-code
```javascript
__toJS = function () {
  assertNotInfinite(this.size);
  var object = {};
  this.__iterate(function(v, k)  { object[k] = v; });
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Keyed.prototype.__toStringMapper"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>__toStringMapper (v, k)](#apidoc.element.immutable.Iterable.Keyed.prototype.__toStringMapper)
- description and source-code
```javascript
__toStringMapper = function (v, k)  {return JSON.stringify(k) + ': ' + quoteString(v)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Keyed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>constructor (value)](#apidoc.element.immutable.Iterable.Keyed.prototype.constructor)
- description and source-code
```javascript
function KeyedIterable(value) {
  return isKeyed(value) ? value : KeyedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Keyed.prototype.flip"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>flip ()](#apidoc.element.immutable.Iterable.Keyed.prototype.flip)
- description and source-code
```javascript
flip = function () {
  return reify(this, flipFactory(this));
}
```
- example usage
```shell
...
Any collection can be converted to a lazy Seq with '.toSeq()'.

var seq = Immutable.Map({a:1, b:1, c:1}).toSeq();

Seq allow for the efficient chaining of sequence operations, especially when
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
// Map { A: 1, B: 1, C: 1 }

As well as expressing logic that would otherwise seem memory-limited:

Immutable.Range(1, Infinity)
  .skip(1000)
  .map(n => -n)
...
```

#### <a name="apidoc.element.immutable.Iterable.Keyed.prototype.mapEntries"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>mapEntries (mapper, context)](#apidoc.element.immutable.Iterable.Keyed.prototype.mapEntries)
- description and source-code
```javascript
mapEntries = function (mapper, context) {var this$0 = this;
  var iterations = 0;
  return reify(this,
    this.toSeq().map(
      function(v, k)  {return mapper.call(context, [k, v], iterations++, this$0)}
    ).fromEntrySeq()
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Keyed.prototype.mapKeys"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Keyed.prototype.</span>mapKeys (mapper, context)](#apidoc.element.immutable.Iterable.Keyed.prototype.mapKeys)
- description and source-code
```javascript
mapKeys = function (mapper, context) {var this$0 = this;
  return reify(this,
    this.toSeq().flip().map(
      function(k, v)  {return mapper.call(context, k, v, this$0)}
    ).flip()
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable.Set.prototype"></a>[module immutable.Iterable.Set.prototype](#apidoc.module.immutable.Iterable.Set.prototype)

#### <a name="apidoc.element.immutable.Iterable.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Iterable.Set.prototype.constructor)
- description and source-code
```javascript
function SetIterable(value) {
  return isIterable(value) && !isAssociative(value) ? value : SetSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Set.prototype.contains"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>contains (value)](#apidoc.element.immutable.Iterable.Set.prototype.contains)
- description and source-code
```javascript
contains = function (value) {
  return this.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Set.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>get (value, notSetValue)](#apidoc.element.immutable.Iterable.Set.prototype.get)
- description and source-code
```javascript
get = function (value, notSetValue) {
  return this.has(value) ? value : notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Iterable.Set.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>has (searchValue)](#apidoc.element.immutable.Iterable.Set.prototype.has)
- description and source-code
```javascript
has = function (searchValue) {
  return this.some(function(value ) {return is(value, searchValue)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Set.prototype.includes"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>includes (value)](#apidoc.element.immutable.Iterable.Set.prototype.includes)
- description and source-code
```javascript
includes = function (value) {
  return this.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.Set.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.Set.prototype.</span>keySeq ()](#apidoc.element.immutable.Iterable.Set.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return this.valueSeq();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Iterable.prototype"></a>[module immutable.Iterable.prototype](#apidoc.module.immutable.Iterable.prototype)

#### <a name="apidoc.element.immutable.Iterable.prototype.__toJS"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>__toJS ()](#apidoc.element.immutable.Iterable.prototype.__toJS)
- description and source-code
```javascript
__toJS = function () {
  assertNotInfinite(this.size);
  var array = new Array(this.size || 0);
  this.valueSeq().__iterate(function(v, i)  { array[i] = v; });
  return array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.__toString"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>__toString (head, tail)](#apidoc.element.immutable.Iterable.prototype.__toString)
- description and source-code
```javascript
__toString = function (head, tail) {
  if (this.size === 0) {
    return head + tail;
  }
  return head + ' ' + this.toSeq().map(this.__toStringMapper).join(', ') + ' ' + tail;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.__toStringMapper"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>__toStringMapper (value)](#apidoc.element.immutable.Iterable.prototype.__toStringMapper)
- description and source-code
```javascript
function quoteString(value) {
  return typeof value === 'string' ? JSON.stringify(value) : String(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.butLast"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>butLast ()](#apidoc.element.immutable.Iterable.prototype.butLast)
- description and source-code
```javascript
butLast = function () {
  return this.slice(0, -1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.chain"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>chain (mapper, context)](#apidoc.element.immutable.Iterable.prototype.chain)
- description and source-code
```javascript
chain = function (mapper, context) {
  return reify(this, flatMapFactory(this, mapper, context));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.concat"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>concat ()](#apidoc.element.immutable.Iterable.prototype.concat)
- description and source-code
```javascript
concat = function () {var values = SLICE$0.call(arguments, 0);
  return reify(this, concatFactory(this, values));
}
```
- example usage
```shell
...
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
assert(list4.get(0) === 1);
'''
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.contains"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>contains (searchValue)](#apidoc.element.immutable.Iterable.prototype.contains)
- description and source-code
```javascript
contains = function (searchValue) {
  return this.some(function(value ) {return is(value, searchValue)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.count"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>count (predicate, context)](#apidoc.element.immutable.Iterable.prototype.count)
- description and source-code
```javascript
count = function (predicate, context) {
  return ensureSize(
    predicate ? this.toSeq().filter(predicate, context) : this
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.countBy"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>countBy (grouper, context)](#apidoc.element.immutable.Iterable.prototype.countBy)
- description and source-code
```javascript
countBy = function (grouper, context) {
  return countByFactory(this, grouper, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.entries"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>entries ()](#apidoc.element.immutable.Iterable.prototype.entries)
- description and source-code
```javascript
entries = function () {
  return this.__iterator(ITERATE_ENTRIES);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.entrySeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>entrySeq ()](#apidoc.element.immutable.Iterable.prototype.entrySeq)
- description and source-code
```javascript
entrySeq = function () {
  var iterable = this;
  if (iterable._cache) {
    // We cache as an entries array, so we can just return the cache!
    return new ArraySeq(iterable._cache);
  }
  var entriesSequence = iterable.toSeq().map(entryMapper).toIndexedSeq();
  entriesSequence.fromEntrySeq = function()  {return iterable.toSeq()};
  return entriesSequence;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.equals"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>equals (other)](#apidoc.element.immutable.Iterable.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return deepEqual(this, other);
}
```
- example usage
```shell
...
interested in doing work when something has changed, you can use equality.

Immutable collections should be treated as *values* rather than *objects*. While
objects represents some thing which could change over time, a value represents
the state of that thing at a particular instance of time. This principle is most
important to understanding the appropriate use of immutable data. In order to
treat Immutable.js collections as values, it's important to use the
'Immutable.is()' function or '.equals()' method to determine value equality
instead of the '===' operator which determines object reference identity.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 2);
assert(map1.equals(map2) === true);
var map3 = map1.set('b', 50);
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.every"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>every (predicate, context)](#apidoc.element.immutable.Iterable.prototype.every)
- description and source-code
```javascript
every = function (predicate, context) {
  assertNotInfinite(this.size);
  var returnValue = true;
  this.__iterate(function(v, k, c)  {
    if (!predicate.call(context, v, k, c)) {
      returnValue = false;
      return false;
    }
  });
  return returnValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.filter"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Iterable.prototype.filter)
- description and source-code
```javascript
filter = function (predicate, context) {
  return reify(this, filterFactory(this, predicate, context, true));
}
```
- example usage
```shell
...
**Seq is lazy** — Seq does as little work as necessary to respond to any
method call.

For example, the following does not perform any work, because the resulting
Seq is never used:

var oddSquares = Immutable.Seq.of(1,2,3,4,5,6,7,8)
  .filter(x => x % 2).map(x => x * x);

Once the Seq is used, it performs only the work necessary. In this
example, no intermediate arrays are ever created, filter is called three times,
and map is only called twice:

console.log(oddSquares.get(1)); // 9
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.filterNot"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>filterNot (predicate, context)](#apidoc.element.immutable.Iterable.prototype.filterNot)
- description and source-code
```javascript
filterNot = function (predicate, context) {
  return this.filter(not(predicate), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.find"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>find (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.find)
- description and source-code
```javascript
find = function (predicate, context, notSetValue) {
  var entry = this.findEntry(predicate, context);
  return entry ? entry[1] : notSetValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.findEntry"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findEntry (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.findEntry)
- description and source-code
```javascript
findEntry = function (predicate, context, notSetValue) {
  var found = notSetValue;
  this.__iterate(function(v, k, c)  {
    if (predicate.call(context, v, k, c)) {
      found = [k, v];
      return false;
    }
  });
  return found;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.findKey"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findKey (predicate, context)](#apidoc.element.immutable.Iterable.prototype.findKey)
- description and source-code
```javascript
findKey = function (predicate, context) {
  var entry = this.findEntry(predicate, context);
  return entry && entry[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.findLast"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findLast (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.findLast)
- description and source-code
```javascript
findLast = function (predicate, context, notSetValue) {
  return this.toKeyedSeq().reverse().find(predicate, context, notSetValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.findLastEntry"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findLastEntry (predicate, context, notSetValue)](#apidoc.element.immutable.Iterable.prototype.findLastEntry)
- description and source-code
```javascript
findLastEntry = function (predicate, context, notSetValue) {
  return this.toKeyedSeq().reverse().findEntry(predicate, context, notSetValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.findLastKey"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>findLastKey (predicate, context)](#apidoc.element.immutable.Iterable.prototype.findLastKey)
- description and source-code
```javascript
findLastKey = function (predicate, context) {
  return this.toKeyedSeq().reverse().findKey(predicate, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.first"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>first ()](#apidoc.element.immutable.Iterable.prototype.first)
- description and source-code
```javascript
first = function () {
  return this.find(returnTrue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.flatMap"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>flatMap (mapper, context)](#apidoc.element.immutable.Iterable.prototype.flatMap)
- description and source-code
```javascript
flatMap = function (mapper, context) {
  return reify(this, flatMapFactory(this, mapper, context));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.flatten"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>flatten (depth)](#apidoc.element.immutable.Iterable.prototype.flatten)
- description and source-code
```javascript
flatten = function (depth) {
  return reify(this, flattenFactory(this, depth, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.forEach"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>forEach (sideEffect, context)](#apidoc.element.immutable.Iterable.prototype.forEach)
- description and source-code
```javascript
forEach = function (sideEffect, context) {
  assertNotInfinite(this.size);
  return this.__iterate(context ? sideEffect.bind(context) : sideEffect);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.fromEntrySeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>fromEntrySeq ()](#apidoc.element.immutable.Iterable.prototype.fromEntrySeq)
- description and source-code
```javascript
fromEntrySeq = function () {
  return new FromEntriesSequence(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>get (searchKey, notSetValue)](#apidoc.element.immutable.Iterable.prototype.get)
- description and source-code
```javascript
get = function (searchKey, notSetValue) {
  return this.find(function(_, key)  {return is(key, searchKey)}, undefined, notSetValue);
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.getIn"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>getIn (searchKeyPath, notSetValue)](#apidoc.element.immutable.Iterable.prototype.getIn)
- description and source-code
```javascript
getIn = function (searchKeyPath, notSetValue) {
  var nested = this;
  // Note: in an ES6 environment, we would prefer:
  // for (var key of searchKeyPath) {
  var iter = forceIterator(searchKeyPath);
  var step;
  while (!(step = iter.next()).done) {
    var key = step.value;
    nested = nested && nested.get ? nested.get(key, NOT_SET) : NOT_SET;
    if (nested === NOT_SET) {
      return notSetValue;
    }
  }
  return nested;
}
```
- example usage
```shell
...

'''javascript
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 7 } } }

var nested4 = nested3.updateIn(['a', 'b', 'c'], list => list.push(6));
// Map { a: Map { b: Map { c: List [ 3, 4, 5, 6 ], d: 7 } } }
'''
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.groupBy"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>groupBy (grouper, context)](#apidoc.element.immutable.Iterable.prototype.groupBy)
- description and source-code
```javascript
groupBy = function (grouper, context) {
  return groupByFactory(this, grouper, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>has (searchKey)](#apidoc.element.immutable.Iterable.prototype.has)
- description and source-code
```javascript
has = function (searchKey) {
  return this.get(searchKey, NOT_SET) !== NOT_SET;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.hasIn"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>hasIn (searchKeyPath)](#apidoc.element.immutable.Iterable.prototype.hasIn)
- description and source-code
```javascript
hasIn = function (searchKeyPath) {
  return this.getIn(searchKeyPath, NOT_SET) !== NOT_SET;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.hashCode"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>hashCode ()](#apidoc.element.immutable.Iterable.prototype.hashCode)
- description and source-code
```javascript
hashCode = function () {
  return this.__hash || (this.__hash = hashIterable(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.includes"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>includes (searchValue)](#apidoc.element.immutable.Iterable.prototype.includes)
- description and source-code
```javascript
includes = function (searchValue) {
  return this.some(function(value ) {return is(value, searchValue)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.inspect"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>inspect ()](#apidoc.element.immutable.Iterable.prototype.inspect)
- description and source-code
```javascript
inspect = function () { return this.toString(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>isEmpty ()](#apidoc.element.immutable.Iterable.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return this.size !== undefined ? this.size === 0 : !this.some(function()  {return true});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.isSubset"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>isSubset (iter)](#apidoc.element.immutable.Iterable.prototype.isSubset)
- description and source-code
```javascript
isSubset = function (iter) {
  iter = typeof iter.includes === 'function' ? iter : Iterable(iter);
  return this.every(function(value ) {return iter.includes(value)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.isSuperset"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>isSuperset (iter)](#apidoc.element.immutable.Iterable.prototype.isSuperset)
- description and source-code
```javascript
isSuperset = function (iter) {
  iter = typeof iter.isSubset === 'function' ? iter : Iterable(iter);
  return iter.isSubset(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.join"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>join (separator)](#apidoc.element.immutable.Iterable.prototype.join)
- description and source-code
```javascript
join = function (separator) {
  assertNotInfinite(this.size);
  separator = separator !== undefined ? '' + separator : ',';
  var joined = '';
  var isFirst = true;
  this.__iterate(function(v ) {
    isFirst ? (isFirst = false) : (joined += separator);
    joined += v !== null && v !== undefined ? v.toString() : '';
  });
  return joined;
}
```
- example usage
```shell
...
Almost all of the methods on [Array][] will be found in similar form on
'Immutable.List', those of [Map][] found on 'Immutable.Map', and those of [Set][]
found on 'Immutable.Set', including collection operations like 'forEach()'
and 'map()'.

'''javascript
var alpha = Immutable.Map({a:1, b:2, c:3, d:4});
alpha.map((v, k) => k.toUpperCase()).join();
// 'A,B,C,D'
'''

### Accepts raw JavaScript objects.

Designed to inter-operate with your existing JavaScript, 'immutable'
accepts plain JavaScript Arrays and Objects anywhere a method expects an
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.keyOf"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>keyOf (searchValue)](#apidoc.element.immutable.Iterable.prototype.keyOf)
- description and source-code
```javascript
keyOf = function (searchValue) {
  return this.findKey(function(value ) {return is(value, searchValue)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>keySeq ()](#apidoc.element.immutable.Iterable.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return this.toSeq().map(keyMapper).toIndexedSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.keys"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>keys ()](#apidoc.element.immutable.Iterable.prototype.keys)
- description and source-code
```javascript
keys = function () {
  return this.__iterator(ITERATE_KEYS);
}
```
- example usage
```shell
...

Keep in mind, when using JS objects to construct Immutable Maps, that
JavaScript Object properties are always strings, even if written in a quote-less
shorthand, while Immutable Maps accept keys of any type.

'''js
var obj = { 1: "one" };
Object.keys(obj); // [ "1" ]
obj["1"]; // "one"
obj[1];   // "one"

var map = Immutable.fromJS(obj);
map.get("1"); // "one"
map.get(1);   // undefined
'''
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.last"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>last ()](#apidoc.element.immutable.Iterable.prototype.last)
- description and source-code
```javascript
last = function () {
  return this.toSeq().reverse().first();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.lastKeyOf"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>lastKeyOf (searchValue)](#apidoc.element.immutable.Iterable.prototype.lastKeyOf)
- description and source-code
```javascript
lastKeyOf = function (searchValue) {
  return this.toKeyedSeq().reverse().keyOf(searchValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.map"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>map (mapper, context)](#apidoc.element.immutable.Iterable.prototype.map)
- description and source-code
```javascript
map = function (mapper, context) {
  return reify(this, mapFactory(this, mapper, context));
}
```
- example usage
```shell
...
Almost all of the methods on [Array][] will be found in similar form on
'Immutable.List', those of [Map][] found on 'Immutable.Map', and those of [Set][]
found on 'Immutable.Set', including collection operations like 'forEach()'
and 'map()'.

'''javascript
var alpha = Immutable.Map({a:1, b:2, c:3, d:4});
alpha.map((v, k) => k.toUpperCase()).join();
// 'A,B,C,D'
'''

### Accepts raw JavaScript objects.

Designed to inter-operate with your existing JavaScript, 'immutable'
accepts plain JavaScript Arrays and Objects anywhere a method expects an
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.max"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>max (comparator)](#apidoc.element.immutable.Iterable.prototype.max)
- description and source-code
```javascript
max = function (comparator) {
  return maxFactory(this, comparator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.maxBy"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>maxBy (mapper, comparator)](#apidoc.element.immutable.Iterable.prototype.maxBy)
- description and source-code
```javascript
maxBy = function (mapper, comparator) {
  return maxFactory(this, comparator, mapper);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.min"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>min (comparator)](#apidoc.element.immutable.Iterable.prototype.min)
- description and source-code
```javascript
min = function (comparator) {
  return maxFactory(this, comparator ? neg(comparator) : defaultNegComparator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.minBy"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>minBy (mapper, comparator)](#apidoc.element.immutable.Iterable.prototype.minBy)
- description and source-code
```javascript
minBy = function (mapper, comparator) {
  return maxFactory(this, comparator ? neg(comparator) : defaultNegComparator, mapper);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.reduce"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>reduce (reducer, initialReduction, context)](#apidoc.element.immutable.Iterable.prototype.reduce)
- description and source-code
```javascript
reduce = function (reducer, initialReduction, context) {
  assertNotInfinite(this.size);
  var reduction;
  var useFirst;
  if (arguments.length < 2) {
    useFirst = true;
  } else {
    reduction = initialReduction;
  }
  this.__iterate(function(v, k, c)  {
    if (useFirst) {
      useFirst = false;
      reduction = v;
    } else {
      reduction = reducer.call(context, reduction, v, k, c);
    }
  });
  return reduction;
}
```
- example usage
```shell
...
As well as expressing logic that would otherwise seem memory-limited:

    Immutable.Range(1, Infinity)
      .skip(1000)
      .map(n => -n)
      .filter(n => n % 2 === 0)
      .take(2)
      .reduce((r, n) => r * n, 1);
    // 1006008

Note: An iterable is always iterated in the same order, however that order may
not always be well defined, as is the case for the 'Map'.


Equality treats Collections as Data
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>reduceRight (reducer, initialReduction, context)](#apidoc.element.immutable.Iterable.prototype.reduceRight)
- description and source-code
```javascript
reduceRight = function (reducer, initialReduction, context) {
  var reversed = this.toKeyedSeq().reverse();
  return reversed.reduce.apply(reversed, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.rest"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>rest ()](#apidoc.element.immutable.Iterable.prototype.rest)
- description and source-code
```javascript
rest = function () {
  return this.slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.reverse"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>reverse ()](#apidoc.element.immutable.Iterable.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  return reify(this, reverseFactory(this, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.skip"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skip (amount)](#apidoc.element.immutable.Iterable.prototype.skip)
- description and source-code
```javascript
skip = function (amount) {
  return this.slice(Math.max(0, amount));
}
```
- example usage
```shell
...

    seq.flip().map(key => key.toUpperCase()).flip().toObject();
    // Map { A: 1, B: 1, C: 1 }

As well as expressing logic that would otherwise seem memory-limited:

    Immutable.Range(1, Infinity)
      .skip(1000)
      .map(n => -n)
      .filter(n => n % 2 === 0)
      .take(2)
      .reduce((r, n) => r * n, 1);
    // 1006008

Note: An iterable is always iterated in the same order, however that order may
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.skipLast"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skipLast (amount)](#apidoc.element.immutable.Iterable.prototype.skipLast)
- description and source-code
```javascript
skipLast = function (amount) {
  return reify(this, this.toSeq().reverse().skip(amount).reverse());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.skipUntil"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skipUntil (predicate, context)](#apidoc.element.immutable.Iterable.prototype.skipUntil)
- description and source-code
```javascript
skipUntil = function (predicate, context) {
  return this.skipWhile(not(predicate), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.skipWhile"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Iterable.prototype.skipWhile)
- description and source-code
```javascript
skipWhile = function (predicate, context) {
  return reify(this, skipWhileFactory(this, predicate, context, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Iterable.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  return reify(this, sliceFactory(this, begin, end, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.some"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>some (predicate, context)](#apidoc.element.immutable.Iterable.prototype.some)
- description and source-code
```javascript
some = function (predicate, context) {
  return !this.every(not(predicate), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.sort"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>sort (comparator)](#apidoc.element.immutable.Iterable.prototype.sort)
- description and source-code
```javascript
sort = function (comparator) {
  return reify(this, sortFactory(this, comparator));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>sortBy (mapper, comparator)](#apidoc.element.immutable.Iterable.prototype.sortBy)
- description and source-code
```javascript
sortBy = function (mapper, comparator) {
  return reify(this, sortFactory(this, comparator, mapper));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.take"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>take (amount)](#apidoc.element.immutable.Iterable.prototype.take)
- description and source-code
```javascript
take = function (amount) {
  return this.slice(0, Math.max(0, amount));
}
```
- example usage
```shell
...

As well as expressing logic that would otherwise seem memory-limited:

    Immutable.Range(1, Infinity)
      .skip(1000)
      .map(n => -n)
      .filter(n => n % 2 === 0)
      .take(2)
      .reduce((r, n) => r * n, 1);
    // 1006008

Note: An iterable is always iterated in the same order, however that order may
not always be well defined, as is the case for the 'Map'.
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.takeLast"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>takeLast (amount)](#apidoc.element.immutable.Iterable.prototype.takeLast)
- description and source-code
```javascript
takeLast = function (amount) {
  return reify(this, this.toSeq().reverse().take(amount).reverse());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.takeUntil"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>takeUntil (predicate, context)](#apidoc.element.immutable.Iterable.prototype.takeUntil)
- description and source-code
```javascript
takeUntil = function (predicate, context) {
  return this.takeWhile(not(predicate), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.takeWhile"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>takeWhile (predicate, context)](#apidoc.element.immutable.Iterable.prototype.takeWhile)
- description and source-code
```javascript
takeWhile = function (predicate, context) {
  return reify(this, takeWhileFactory(this, predicate, context));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toArray"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toArray ()](#apidoc.element.immutable.Iterable.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  assertNotInfinite(this.size);
  var array = new Array(this.size || 0);
  this.valueSeq().__iterate(function(v, i)  { array[i] = v; });
  return array;
}
```
- example usage
```shell
...
Objects shallowly with 'toArray()' and 'toObject()' or deeply with 'toJS()'.
All Immutable Iterables also implement 'toJSON()' allowing them to be passed to
'JSON.stringify' directly.

'''javascript
var deep = Immutable.Map({ a: 1, b: 2, c: Immutable.List.of(3, 4, 5) });
deep.toObject() // { a: 1, b: 2, c: List [ 3, 4, 5 ] }
deep.toArray() // [ 1, 2, List [ 3, 4, 5 ] ]
deep.toJS() // { a: 1, b: 2, c: [ 3, 4, 5 ] }
JSON.stringify(deep) // '{"a":1,"b":2,"c":[3,4,5]}'
'''

### Embraces ES6

'Immutable' takes advantage of features added to JavaScript in [ES6][],
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toIndexedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toIndexedSeq ()](#apidoc.element.immutable.Iterable.prototype.toIndexedSeq)
- description and source-code
```javascript
toIndexedSeq = function () {
  return new ToIndexedSequence(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toJS"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toJS ()](#apidoc.element.immutable.Iterable.prototype.toJS)
- description and source-code
```javascript
toJS = function () {
  return this.toSeq().map(
    function(value ) {return value && typeof value.toJS === 'function' ? value.toJS() : value}
  ).__toJS();
}
```
- example usage
```shell
...
All Immutable Iterables also implement 'toJSON()' allowing them to be passed to
'JSON.stringify' directly.

'''javascript
var deep = Immutable.Map({ a: 1, b: 2, c: Immutable.List.of(3, 4, 5) });
deep.toObject() // { a: 1, b: 2, c: List [ 3, 4, 5 ] }
deep.toArray() // [ 1, 2, List [ 3, 4, 5 ] ]
deep.toJS() // { a: 1, b: 2, c: [ 3, 4, 5 ] }
JSON.stringify(deep) // '{"a":1,"b":2,"c":[3,4,5]}'
'''

### Embraces ES6

'Immutable' takes advantage of features added to JavaScript in [ES6][],
the latest standard version of ECMAScript (JavaScript), including [Iterators][],
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toJSON ()](#apidoc.element.immutable.Iterable.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toSeq().map(
    function(value ) {return value && typeof value.toJSON === 'function' ? value.toJSON() : value}
  ).__toJS();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toKeyedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Iterable.prototype.toKeyedSeq)
- description and source-code
```javascript
toKeyedSeq = function () {
  return new ToKeyedSequence(this, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toList"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toList ()](#apidoc.element.immutable.Iterable.prototype.toList)
- description and source-code
```javascript
toList = function () {
  // Use Late Binding here to solve the circular dependency.
  return List(isKeyed(this) ? this.valueSeq() : this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toMap"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toMap ()](#apidoc.element.immutable.Iterable.prototype.toMap)
- description and source-code
```javascript
toMap = function () {
  // Use Late Binding here to solve the circular dependency.
  return Map(this.toKeyedSeq());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toObject"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toObject ()](#apidoc.element.immutable.Iterable.prototype.toObject)
- description and source-code
```javascript
toObject = function () {
  assertNotInfinite(this.size);
  var object = {};
  this.__iterate(function(v, k)  { object[k] = v; });
  return object;
}
```
- example usage
```shell
...
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
results, these operations can be extremely efficient.

'''javascript
var myObject = {a:1,b:2,c:3};
Immutable.Seq(myObject).map(x => x * x).toObject();
// { a: 1, b: 4, c: 9 }
'''

Keep in mind, when using JS objects to construct Immutable Maps, that
JavaScript Object properties are always strings, even if written in a quote-less
shorthand, while Immutable Maps accept keys of any type.
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toOrderedMap"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toOrderedMap ()](#apidoc.element.immutable.Iterable.prototype.toOrderedMap)
- description and source-code
```javascript
toOrderedMap = function () {
  // Use Late Binding here to solve the circular dependency.
  return OrderedMap(this.toKeyedSeq());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toOrderedSet"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toOrderedSet ()](#apidoc.element.immutable.Iterable.prototype.toOrderedSet)
- description and source-code
```javascript
toOrderedSet = function () {
  // Use Late Binding here to solve the circular dependency.
  return OrderedSet(isKeyed(this) ? this.valueSeq() : this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toSeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSeq ()](#apidoc.element.immutable.Iterable.prototype.toSeq)
- description and source-code
```javascript
toSeq = function () {
  return isIndexed(this) ? this.toIndexedSeq() :
    isKeyed(this) ? this.toKeyedSeq() :
    this.toSetSeq();
}
```
- example usage
```shell
...

Once the Seq is used, it performs only the work necessary. In this
example, no intermediate arrays are ever created, filter is called three times,
and map is only called twice:

console.log(oddSquares.get(1)); // 9

Any collection can be converted to a lazy Seq with '.toSeq()'.

var seq = Immutable.Map({a:1, b:1, c:1}).toSeq();

Seq allow for the efficient chaining of sequence operations, especially when
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
...
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toSet"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSet ()](#apidoc.element.immutable.Iterable.prototype.toSet)
- description and source-code
```javascript
toSet = function () {
  // Use Late Binding here to solve the circular dependency.
  return Set(isKeyed(this) ? this.valueSeq() : this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toSetSeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSetSeq ()](#apidoc.element.immutable.Iterable.prototype.toSetSeq)
- description and source-code
```javascript
toSetSeq = function () {
  return new ToSetSequence(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toSource"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toSource ()](#apidoc.element.immutable.Iterable.prototype.toSource)
- description and source-code
```javascript
toSource = function () { return this.toString(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toStack"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toStack ()](#apidoc.element.immutable.Iterable.prototype.toStack)
- description and source-code
```javascript
toStack = function () {
  // Use Late Binding here to solve the circular dependency.
  return Stack(isKeyed(this) ? this.valueSeq() : this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>toString ()](#apidoc.element.immutable.Iterable.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return '[Iterable]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.valueSeq"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>valueSeq ()](#apidoc.element.immutable.Iterable.prototype.valueSeq)
- description and source-code
```javascript
valueSeq = function () {
  return this.toIndexedSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Iterable.prototype.values"></a>[function <span class="apidocSignatureSpan">immutable.Iterable.prototype.</span>values ()](#apidoc.element.immutable.Iterable.prototype.values)
- description and source-code
```javascript
values = function () {
  return this.__iterator(ITERATE_VALUES);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.List"></a>[module immutable.List](#apidoc.module.immutable.List)

#### <a name="apidoc.element.immutable.List.List"></a>[function <span class="apidocSignatureSpan">immutable.</span>List (value)](#apidoc.element.immutable.List.List)
- description and source-code
```javascript
function List(value) {
  var empty = emptyList();
  if (value === null || value === undefined) {
    return empty;
  }
  if (isList(value)) {
    return value;
  }
  var iter = IndexedIterable(value);
  var size = iter.size;
  if (size === 0) {
    return empty;
  }
  assertNotInfinite(size);
  if (size > 0 && size < SIZE) {
    return makeList(0, size, SHIFT, null, new VNode(iter.toArray()));
  }
  return empty.withMutations(function(list ) {
    list.setSize(size);
    iter.forEach(function(v, i)  {return list.set(i, v)});
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.isList"></a>[function <span class="apidocSignatureSpan">immutable.List.</span>isList (maybeList)](#apidoc.element.immutable.List.isList)
- description and source-code
```javascript
function isList(maybeList) {
  return !!(maybeList && maybeList[IS_LIST_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.of"></a>[function <span class="apidocSignatureSpan">immutable.List.</span>of ()](#apidoc.element.immutable.List.of)
- description and source-code
```javascript
of = function () {
  return this(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.List.prototype"></a>[module immutable.List.prototype](#apidoc.module.immutable.List.prototype)

#### <a name="apidoc.element.immutable.List.prototype.__ensureOwner"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.List.prototype.__ensureOwner)
- description and source-code
```javascript
__ensureOwner = function (ownerID) {
  if (ownerID === this.__ownerID) {
    return this;
  }
  if (!ownerID) {
    this.__ownerID = ownerID;
    return this;
  }
  return makeList(this._origin, this._capacity, this._level, this._root, this._tail, ownerID, this.__hash);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.List.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {
  var index = 0;
  var values = iterateList(this, reverse);
  var value;
  while ((value = values()) !== DONE) {
    if (fn(value, index++, this) === false) {
      break;
    }
  }
  return index;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.List.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  var index = 0;
  var values = iterateList(this, reverse);
  return new Iterator(function()  {
    var value = values();
    return value === DONE ?
      iteratorDone() :
      iteratorValue(type, index++, value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.asImmutable"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>asImmutable ()](#apidoc.element.immutable.List.prototype.asImmutable)
- description and source-code
```javascript
asImmutable = function () {
  return this.__ensureOwner();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.asMutable"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>asMutable ()](#apidoc.element.immutable.List.prototype.asMutable)
- description and source-code
```javascript
asMutable = function () {
  return this.__ownerID ? this : this.__ensureOwner(new OwnerID());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.clear"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>clear ()](#apidoc.element.immutable.List.prototype.clear)
- description and source-code
```javascript
clear = function () {
  if (this.size === 0) {
    return this;
  }
  if (this.__ownerID) {
    this.size = this._origin = this._capacity = 0;
    this._level = SHIFT;
    this._root = this._tail = null;
    this.__hash = undefined;
    this.__altered = true;
    return this;
  }
  return emptyList();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>constructor (value)](#apidoc.element.immutable.List.prototype.constructor)
- description and source-code
```javascript
function List(value) {
  var empty = emptyList();
  if (value === null || value === undefined) {
    return empty;
  }
  if (isList(value)) {
    return value;
  }
  var iter = IndexedIterable(value);
  var size = iter.size;
  if (size === 0) {
    return empty;
  }
  assertNotInfinite(size);
  if (size > 0 && size < SIZE) {
    return makeList(0, size, SHIFT, null, new VNode(iter.toArray()));
  }
  return empty.withMutations(function(list ) {
    list.setSize(size);
    iter.forEach(function(v, i)  {return list.set(i, v)});
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.delete"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>delete (index)](#apidoc.element.immutable.List.prototype.delete)
- description and source-code
```javascript
delete = function (index) {
  return !this.has(index) ? this :
    index === 0 ? this.shift() :
    index === this.size - 1 ? this.pop() :
    this.splice(index, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.deleteIn"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>deleteIn (keyPath)](#apidoc.element.immutable.List.prototype.deleteIn)
- description and source-code
```javascript
deleteIn = function (keyPath) {
  return this.updateIn(keyPath, function()  {return NOT_SET});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.List.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  index = wrapIndex(this, index);
  if (index >= 0 && index < this.size) {
    index += this._origin;
    var node = listNodeFor(this, index);
    return node && node.array[index & MASK];
  }
  return notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.List.prototype.insert"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>insert (index, value)](#apidoc.element.immutable.List.prototype.insert)
- description and source-code
```javascript
insert = function (index, value) {
  return this.splice(index, 0, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.merge"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>merge ()](#apidoc.element.immutable.List.prototype.merge)
- description and source-code
```javascript
merge = function () {
  return mergeIntoListWith(this, undefined, arguments);
}
```
- example usage
```shell
...
accepts plain JavaScript Arrays and Objects anywhere a method expects an
'Iterable' with no performance penalty.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3, d:4});
var map2 = Immutable.Map({c:10, a:20, t:30});
var obj = {d:100, o:200, g:300};
var map3 = map1.merge(map2, obj);
// Map { a: 20, b: 2, c: 10, d: 100, t: 30, o: 200, g: 300 }
'''

This is possible because 'immutable' can treat any JavaScript Array or Object
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
...
```

#### <a name="apidoc.element.immutable.List.prototype.mergeDeep"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeDeep ()](#apidoc.element.immutable.List.prototype.mergeDeep)
- description and source-code
```javascript
mergeDeep = function () {
  return mergeIntoListWith(this, deepMerger, arguments);
}
```
- example usage
```shell
...
'''

A few power-tools allow for reading and operating on nested data. The
most useful are 'mergeDeep', 'getIn', 'setIn', and 'updateIn', found on 'List',
'Map' and 'OrderedMap'.

'''javascript
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
...
```

#### <a name="apidoc.element.immutable.List.prototype.mergeDeepIn"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeDeepIn (keyPath)](#apidoc.element.immutable.List.prototype.mergeDeepIn)
- description and source-code
```javascript
mergeDeepIn = function (keyPath) {var iters = SLICE$0.call(arguments, 1);
  return this.updateIn(
    keyPath,
    emptyMap(),
    function(m ) {return typeof m.mergeDeep === 'function' ?
      m.mergeDeep.apply(m, iters) :
      iters[iters.length - 1]}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.mergeDeepWith"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.List.prototype.mergeDeepWith)
- description and source-code
```javascript
mergeDeepWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return mergeIntoListWith(this, deepMergerWith(merger), iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.mergeIn"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeIn (keyPath)](#apidoc.element.immutable.List.prototype.mergeIn)
- description and source-code
```javascript
mergeIn = function (keyPath) {var iters = SLICE$0.call(arguments, 1);
  return this.updateIn(
    keyPath,
    emptyMap(),
    function(m ) {return typeof m.merge === 'function' ?
      m.merge.apply(m, iters) :
      iters[iters.length - 1]}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.mergeWith"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.List.prototype.mergeWith)
- description and source-code
```javascript
mergeWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return mergeIntoListWith(this, merger, iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.pop"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>pop ()](#apidoc.element.immutable.List.prototype.pop)
- description and source-code
```javascript
pop = function () {
  return setListBounds(this, 0, -1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.push"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>push ()](#apidoc.element.immutable.List.prototype.push)
- description and source-code
```javascript
push = function () {
  var values = arguments;
  var oldSize = this.size;
  return this.withMutations(function(list ) {
    setListBounds(list, 0, oldSize + values.length);
    for (var ii = 0; ii < values.length; ii++) {
      list.set(oldSize + ii, values[ii]);
    }
  });
}
```
- example usage
```shell
...
The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
assert(list4.get(0) === 1);
...
```

#### <a name="apidoc.element.immutable.List.prototype.remove"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>remove (index)](#apidoc.element.immutable.List.prototype.remove)
- description and source-code
```javascript
remove = function (index) {
  return !this.has(index) ? this :
    index === 0 ? this.shift() :
    index === this.size - 1 ? this.pop() :
    this.splice(index, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.removeIn"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>removeIn (keyPath)](#apidoc.element.immutable.List.prototype.removeIn)
- description and source-code
```javascript
removeIn = function (keyPath) {
  return this.updateIn(keyPath, function()  {return NOT_SET});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.set"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>set (index, value)](#apidoc.element.immutable.List.prototype.set)
- description and source-code
```javascript
set = function (index, value) {
  return updateList(this, index, value);
}
```
- example usage
```shell
...
'''

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
...
```

#### <a name="apidoc.element.immutable.List.prototype.setIn"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>setIn (keyPath, v)](#apidoc.element.immutable.List.prototype.setIn)
- description and source-code
```javascript
setIn = function (keyPath, v) {
  return this.updateIn(keyPath, NOT_SET, function()  {return v});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.setSize"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>setSize (size)](#apidoc.element.immutable.List.prototype.setSize)
- description and source-code
```javascript
setSize = function (size) {
  return setListBounds(this, 0, size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.shift"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>shift ()](#apidoc.element.immutable.List.prototype.shift)
- description and source-code
```javascript
shift = function () {
  return setListBounds(this, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>slice (begin, end)](#apidoc.element.immutable.List.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  var size = this.size;
  if (wholeSlice(begin, end, size)) {
    return this;
  }
  return setListBounds(
    this,
    resolveBegin(begin, size),
    resolveEnd(end, size)
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>toString ()](#apidoc.element.immutable.List.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('List [', ']');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.unshift"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>unshift ()](#apidoc.element.immutable.List.prototype.unshift)
- description and source-code
```javascript
unshift = function () {
  var values = arguments;
  return this.withMutations(function(list ) {
    setListBounds(list, -values.length);
    for (var ii = 0; ii < values.length; ii++) {
      list.set(ii, values[ii]);
    }
  });
}
```
- example usage
```shell
...
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
assert(list4.get(0) === 1);
'''
...
```

#### <a name="apidoc.element.immutable.List.prototype.update"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>update (k, notSetValue, updater)](#apidoc.element.immutable.List.prototype.update)
- description and source-code
```javascript
update = function (k, notSetValue, updater) {
  return arguments.length === 1 ?
    k(this) :
    this.updateIn([k], notSetValue, updater);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.updateIn"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>updateIn (keyPath, notSetValue, updater)](#apidoc.element.immutable.List.prototype.updateIn)
- description and source-code
```javascript
updateIn = function (keyPath, notSetValue, updater) {
  if (!updater) {
    updater = notSetValue;
    notSetValue = undefined;
  }
  var updatedValue = updateInDeepMap(
    this,
    forceIterator(keyPath),
    notSetValue,
    updater
  );
  return updatedValue === NOT_SET ? undefined : updatedValue;
}
```
- example usage
```shell
...
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 7 } } }

var nested4 = nested3.updateIn(['a', 'b', 'c'], list => list.push(6));
// Map { a: Map { b: Map { c: List [ 3, 4, 5, 6 ], d: 7 } } }
'''
...
```

#### <a name="apidoc.element.immutable.List.prototype.wasAltered"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>wasAltered ()](#apidoc.element.immutable.List.prototype.wasAltered)
- description and source-code
```javascript
wasAltered = function () {
  return this.__altered;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.List.prototype.withMutations"></a>[function <span class="apidocSignatureSpan">immutable.List.prototype.</span>withMutations (fn)](#apidoc.element.immutable.List.prototype.withMutations)
- description and source-code
```javascript
withMutations = function (fn) {
  var mutable = this.asMutable();
  fn(mutable);
  return mutable.wasAltered() ? mutable.__ensureOwner(this.__ownerID) : this;
}
```
- example usage
```shell
...
exactly how  'Immutable' applies complex mutations itself.

As an example, building 'list2' results in the creation of 1, not 3, new
immutable Lists.

'''javascript
var list1 = Immutable.List.of(1,2,3);
var list2 = list1.withMutations(function (list) {
  list.push(4).push(5).push(6);
});
assert(list1.size === 3);
assert(list2.size === 6);
'''

Note: 'immutable' also provides 'asMutable' and 'asImmutable', but only
...
```



# <a name="apidoc.module.immutable.Map"></a>[module immutable.Map](#apidoc.module.immutable.Map)

#### <a name="apidoc.element.immutable.Map.Map"></a>[function <span class="apidocSignatureSpan">immutable.</span>Map (value)](#apidoc.element.immutable.Map.Map)
- description and source-code
```javascript
function Map(value) {
  return value === null || value === undefined ? emptyMap() :
    isMap(value) && !isOrdered(value) ? value :
    emptyMap().withMutations(function(map ) {
      var iter = KeyedIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v, k)  {return map.set(k, v)});
    });
}
```
- example usage
```shell
...
npm install immutable
'''

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser
...
```

#### <a name="apidoc.element.immutable.Map.isMap"></a>[function <span class="apidocSignatureSpan">immutable.Map.</span>isMap (maybeMap)](#apidoc.element.immutable.Map.isMap)
- description and source-code
```javascript
function isMap(maybeMap) {
  return !!(maybeMap && maybeMap[IS_MAP_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.of"></a>[function <span class="apidocSignatureSpan">immutable.Map.</span>of ()](#apidoc.element.immutable.Map.of)
- description and source-code
```javascript
of = function () {var keyValues = SLICE$0.call(arguments, 0);
  return emptyMap().withMutations(function(map ) {
    for (var i = 0; i < keyValues.length; i += 2) {
      if (i + 1 >= keyValues.length) {
        throw new Error('Missing value for key: ' + keyValues[i]);
      }
      map.set(keyValues[i], keyValues[i + 1]);
    }
  });
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.Map.prototype"></a>[module immutable.Map.prototype](#apidoc.module.immutable.Map.prototype)

#### <a name="apidoc.element.immutable.Map.prototype.__ensureOwner"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Map.prototype.__ensureOwner)
- description and source-code
```javascript
__ensureOwner = function (ownerID) {
  if (ownerID === this.__ownerID) {
    return this;
  }
  if (!ownerID) {
    this.__ownerID = ownerID;
    this.__altered = false;
    return this;
  }
  return makeMap(this.size, this._root, ownerID, this.__hash);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Map.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {var this$0 = this;
  var iterations = 0;
  this._root && this._root.iterate(function(entry ) {
    iterations++;
    return fn(entry[1], entry[0], this$0);
  }, reverse);
  return iterations;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Map.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  return new MapIterator(this, type, reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.asImmutable"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>asImmutable ()](#apidoc.element.immutable.Map.prototype.asImmutable)
- description and source-code
```javascript
asImmutable = function () {
  return this.__ensureOwner();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.asMutable"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>asMutable ()](#apidoc.element.immutable.Map.prototype.asMutable)
- description and source-code
```javascript
asMutable = function () {
  return this.__ownerID ? this : this.__ensureOwner(new OwnerID());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.clear"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>clear ()](#apidoc.element.immutable.Map.prototype.clear)
- description and source-code
```javascript
clear = function () {
  if (this.size === 0) {
    return this;
  }
  if (this.__ownerID) {
    this.size = 0;
    this._root = null;
    this.__hash = undefined;
    this.__altered = true;
    return this;
  }
  return emptyMap();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>constructor (value)](#apidoc.element.immutable.Map.prototype.constructor)
- description and source-code
```javascript
function Map(value) {
  return value === null || value === undefined ? emptyMap() :
    isMap(value) && !isOrdered(value) ? value :
    emptyMap().withMutations(function(map ) {
      var iter = KeyedIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v, k)  {return map.set(k, v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.delete"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>delete (k)](#apidoc.element.immutable.Map.prototype.delete)
- description and source-code
```javascript
delete = function (k) {
  return updateMap(this, k, NOT_SET);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.deleteIn"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>deleteIn (keyPath)](#apidoc.element.immutable.Map.prototype.deleteIn)
- description and source-code
```javascript
deleteIn = function (keyPath) {
  return this.updateIn(keyPath, function()  {return NOT_SET});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>get (k, notSetValue)](#apidoc.element.immutable.Map.prototype.get)
- description and source-code
```javascript
get = function (k, notSetValue) {
  return this._root ?
    this._root.get(0, undefined, k, notSetValue) :
    notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Map.prototype.merge"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>merge ()](#apidoc.element.immutable.Map.prototype.merge)
- description and source-code
```javascript
merge = function () {
  return mergeIntoMapWith(this, undefined, arguments);
}
```
- example usage
```shell
...
accepts plain JavaScript Arrays and Objects anywhere a method expects an
'Iterable' with no performance penalty.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3, d:4});
var map2 = Immutable.Map({c:10, a:20, t:30});
var obj = {d:100, o:200, g:300};
var map3 = map1.merge(map2, obj);
// Map { a: 20, b: 2, c: 10, d: 100, t: 30, o: 200, g: 300 }
'''

This is possible because 'immutable' can treat any JavaScript Array or Object
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
...
```

#### <a name="apidoc.element.immutable.Map.prototype.mergeDeep"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeDeep ()](#apidoc.element.immutable.Map.prototype.mergeDeep)
- description and source-code
```javascript
mergeDeep = function () {
  return mergeIntoMapWith(this, deepMerger, arguments);
}
```
- example usage
```shell
...
'''

A few power-tools allow for reading and operating on nested data. The
most useful are 'mergeDeep', 'getIn', 'setIn', and 'updateIn', found on 'List',
'Map' and 'OrderedMap'.

'''javascript
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
...
```

#### <a name="apidoc.element.immutable.Map.prototype.mergeDeepIn"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeDeepIn (keyPath)](#apidoc.element.immutable.Map.prototype.mergeDeepIn)
- description and source-code
```javascript
mergeDeepIn = function (keyPath) {var iters = SLICE$0.call(arguments, 1);
  return this.updateIn(
    keyPath,
    emptyMap(),
    function(m ) {return typeof m.mergeDeep === 'function' ?
      m.mergeDeep.apply(m, iters) :
      iters[iters.length - 1]}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.mergeDeepWith"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.Map.prototype.mergeDeepWith)
- description and source-code
```javascript
mergeDeepWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return mergeIntoMapWith(this, deepMergerWith(merger), iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.mergeIn"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeIn (keyPath)](#apidoc.element.immutable.Map.prototype.mergeIn)
- description and source-code
```javascript
mergeIn = function (keyPath) {var iters = SLICE$0.call(arguments, 1);
  return this.updateIn(
    keyPath,
    emptyMap(),
    function(m ) {return typeof m.merge === 'function' ?
      m.merge.apply(m, iters) :
      iters[iters.length - 1]}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.mergeWith"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.Map.prototype.mergeWith)
- description and source-code
```javascript
mergeWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return mergeIntoMapWith(this, merger, iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.remove"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>remove (k)](#apidoc.element.immutable.Map.prototype.remove)
- description and source-code
```javascript
remove = function (k) {
  return updateMap(this, k, NOT_SET);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.removeIn"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>removeIn (keyPath)](#apidoc.element.immutable.Map.prototype.removeIn)
- description and source-code
```javascript
removeIn = function (keyPath) {
  return this.updateIn(keyPath, function()  {return NOT_SET});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.set"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>set (k, v)](#apidoc.element.immutable.Map.prototype.set)
- description and source-code
```javascript
set = function (k, v) {
  return updateMap(this, k, v);
}
```
- example usage
```shell
...
'''

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
...
```

#### <a name="apidoc.element.immutable.Map.prototype.setIn"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>setIn (keyPath, v)](#apidoc.element.immutable.Map.prototype.setIn)
- description and source-code
```javascript
setIn = function (keyPath, v) {
  return this.updateIn(keyPath, NOT_SET, function()  {return v});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.sort"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>sort (comparator)](#apidoc.element.immutable.Map.prototype.sort)
- description and source-code
```javascript
sort = function (comparator) {
  // Late binding
  return OrderedMap(sortFactory(this, comparator));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>sortBy (mapper, comparator)](#apidoc.element.immutable.Map.prototype.sortBy)
- description and source-code
```javascript
sortBy = function (mapper, comparator) {
  // Late binding
  return OrderedMap(sortFactory(this, comparator, mapper));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>toString ()](#apidoc.element.immutable.Map.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('Map {', '}');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.update"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>update (k, notSetValue, updater)](#apidoc.element.immutable.Map.prototype.update)
- description and source-code
```javascript
update = function (k, notSetValue, updater) {
  return arguments.length === 1 ?
    k(this) :
    this.updateIn([k], notSetValue, updater);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.updateIn"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>updateIn (keyPath, notSetValue, updater)](#apidoc.element.immutable.Map.prototype.updateIn)
- description and source-code
```javascript
updateIn = function (keyPath, notSetValue, updater) {
  if (!updater) {
    updater = notSetValue;
    notSetValue = undefined;
  }
  var updatedValue = updateInDeepMap(
    this,
    forceIterator(keyPath),
    notSetValue,
    updater
  );
  return updatedValue === NOT_SET ? undefined : updatedValue;
}
```
- example usage
```shell
...
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 7 } } }

var nested4 = nested3.updateIn(['a', 'b', 'c'], list => list.push(6));
// Map { a: Map { b: Map { c: List [ 3, 4, 5, 6 ], d: 7 } } }
'''
...
```

#### <a name="apidoc.element.immutable.Map.prototype.wasAltered"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>wasAltered ()](#apidoc.element.immutable.Map.prototype.wasAltered)
- description and source-code
```javascript
wasAltered = function () {
  return this.__altered;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Map.prototype.withMutations"></a>[function <span class="apidocSignatureSpan">immutable.Map.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Map.prototype.withMutations)
- description and source-code
```javascript
withMutations = function (fn) {
  var mutable = this.asMutable();
  fn(mutable);
  return mutable.wasAltered() ? mutable.__ensureOwner(this.__ownerID) : this;
}
```
- example usage
```shell
...
exactly how  'Immutable' applies complex mutations itself.

As an example, building 'list2' results in the creation of 1, not 3, new
immutable Lists.

'''javascript
var list1 = Immutable.List.of(1,2,3);
var list2 = list1.withMutations(function (list) {
  list.push(4).push(5).push(6);
});
assert(list1.size === 3);
assert(list2.size === 6);
'''

Note: 'immutable' also provides 'asMutable' and 'asImmutable', but only
...
```



# <a name="apidoc.module.immutable.OrderedMap"></a>[module immutable.OrderedMap](#apidoc.module.immutable.OrderedMap)

#### <a name="apidoc.element.immutable.OrderedMap.OrderedMap"></a>[function <span class="apidocSignatureSpan">immutable.</span>OrderedMap (value)](#apidoc.element.immutable.OrderedMap.OrderedMap)
- description and source-code
```javascript
function OrderedMap(value) {
  return value === null || value === undefined ? emptyOrderedMap() :
    isOrderedMap(value) ? value :
    emptyOrderedMap().withMutations(function(map ) {
      var iter = KeyedIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v, k)  {return map.set(k, v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.isOrderedMap"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.</span>isOrderedMap (maybeOrderedMap)](#apidoc.element.immutable.OrderedMap.isOrderedMap)
- description and source-code
```javascript
function isOrderedMap(maybeOrderedMap) {
  return isMap(maybeOrderedMap) && isOrdered(maybeOrderedMap);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.of"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.</span>of ()](#apidoc.element.immutable.OrderedMap.of)
- description and source-code
```javascript
of = function () {
  return this(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.OrderedMap.prototype"></a>[module immutable.OrderedMap.prototype](#apidoc.module.immutable.OrderedMap.prototype)

#### <a name="apidoc.element.immutable.OrderedMap.prototype.__ensureOwner"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.OrderedMap.prototype.__ensureOwner)
- description and source-code
```javascript
__ensureOwner = function (ownerID) {
  if (ownerID === this.__ownerID) {
    return this;
  }
  var newMap = this._map.__ensureOwner(ownerID);
  var newList = this._list.__ensureOwner(ownerID);
  if (!ownerID) {
    this.__ownerID = ownerID;
    this._map = newMap;
    this._list = newList;
    return this;
  }
  return makeOrderedMap(newMap, newList, ownerID, this.__hash);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.OrderedMap.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {var this$0 = this;
  return this._list.__iterate(
    function(entry ) {return entry && fn(entry[1], entry[0], this$0)},
    reverse
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.OrderedMap.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  return this._list.fromEntrySeq().__iterator(type, reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.clear"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>clear ()](#apidoc.element.immutable.OrderedMap.prototype.clear)
- description and source-code
```javascript
clear = function () {
  if (this.size === 0) {
    return this;
  }
  if (this.__ownerID) {
    this.size = 0;
    this._map.clear();
    this._list.clear();
    return this;
  }
  return emptyOrderedMap();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>constructor (value)](#apidoc.element.immutable.OrderedMap.prototype.constructor)
- description and source-code
```javascript
function OrderedMap(value) {
  return value === null || value === undefined ? emptyOrderedMap() :
    isOrderedMap(value) ? value :
    emptyOrderedMap().withMutations(function(map ) {
      var iter = KeyedIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v, k)  {return map.set(k, v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.delete"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>delete (k)](#apidoc.element.immutable.OrderedMap.prototype.delete)
- description and source-code
```javascript
delete = function (k) {
  return updateOrderedMap(this, k, NOT_SET);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>get (k, notSetValue)](#apidoc.element.immutable.OrderedMap.prototype.get)
- description and source-code
```javascript
get = function (k, notSetValue) {
  var index = this._map.get(k);
  return index !== undefined ? this._list.get(index)[1] : notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.remove"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>remove (k)](#apidoc.element.immutable.OrderedMap.prototype.remove)
- description and source-code
```javascript
remove = function (k) {
  return updateOrderedMap(this, k, NOT_SET);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.set"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>set (k, v)](#apidoc.element.immutable.OrderedMap.prototype.set)
- description and source-code
```javascript
set = function (k, v) {
  return updateOrderedMap(this, k, v);
}
```
- example usage
```shell
...
'''

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
...
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>toString ()](#apidoc.element.immutable.OrderedMap.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('OrderedMap {', '}');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedMap.prototype.wasAltered"></a>[function <span class="apidocSignatureSpan">immutable.OrderedMap.prototype.</span>wasAltered ()](#apidoc.element.immutable.OrderedMap.prototype.wasAltered)
- description and source-code
```javascript
wasAltered = function () {
  return this._map.wasAltered() || this._list.wasAltered();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.OrderedSet"></a>[module immutable.OrderedSet](#apidoc.module.immutable.OrderedSet)

#### <a name="apidoc.element.immutable.OrderedSet.OrderedSet"></a>[function <span class="apidocSignatureSpan">immutable.</span>OrderedSet (value)](#apidoc.element.immutable.OrderedSet.OrderedSet)
- description and source-code
```javascript
function OrderedSet(value) {
  return value === null || value === undefined ? emptyOrderedSet() :
    isOrderedSet(value) ? value :
    emptyOrderedSet().withMutations(function(set ) {
      var iter = SetIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v ) {return set.add(v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet.fromKeys"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.</span>fromKeys (value)](#apidoc.element.immutable.OrderedSet.fromKeys)
- description and source-code
```javascript
fromKeys = function (value) {
  return this(KeyedIterable(value).keySeq());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet.isOrderedSet"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.</span>isOrderedSet (maybeOrderedSet)](#apidoc.element.immutable.OrderedSet.isOrderedSet)
- description and source-code
```javascript
function isOrderedSet(maybeOrderedSet) {
  return isSet(maybeOrderedSet) && isOrdered(maybeOrderedSet);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet.of"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.</span>of ()](#apidoc.element.immutable.OrderedSet.of)
- description and source-code
```javascript
of = function () {
  return this(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.OrderedSet.prototype"></a>[module immutable.OrderedSet.prototype](#apidoc.module.immutable.OrderedSet.prototype)

#### <a name="apidoc.element.immutable.OrderedSet.prototype.__empty"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>__empty ()](#apidoc.element.immutable.OrderedSet.prototype.__empty)
- description and source-code
```javascript
function emptyOrderedSet() {
  return EMPTY_ORDERED_SET || (EMPTY_ORDERED_SET = makeOrderedSet(emptyOrderedMap()));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet.prototype.__make"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>__make (map, ownerID)](#apidoc.element.immutable.OrderedSet.prototype.__make)
- description and source-code
```javascript
function makeOrderedSet(map, ownerID) {
  var set = Object.create(OrderedSetPrototype);
  set.size = map ? map.size : 0;
  set._map = map;
  set.__ownerID = ownerID;
  return set;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>constructor (value)](#apidoc.element.immutable.OrderedSet.prototype.constructor)
- description and source-code
```javascript
function OrderedSet(value) {
  return value === null || value === undefined ? emptyOrderedSet() :
    isOrderedSet(value) ? value :
    emptyOrderedSet().withMutations(function(set ) {
      var iter = SetIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v ) {return set.add(v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.OrderedSet.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.OrderedSet.prototype.</span>toString ()](#apidoc.element.immutable.OrderedSet.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('OrderedSet {', '}');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Range"></a>[module immutable.Range](#apidoc.module.immutable.Range)

#### <a name="apidoc.element.immutable.Range.Range"></a>[function <span class="apidocSignatureSpan">immutable.</span>Range (start, end, step)](#apidoc.element.immutable.Range.Range)
- description and source-code
```javascript
function Range(start, end, step) {
  if (!(this instanceof Range)) {
    return new Range(start, end, step);
  }
  invariant(step !== 0, 'Cannot step a Range by 0');
  start = start || 0;
  if (end === undefined) {
    end = Infinity;
  }
  step = step === undefined ? 1 : Math.abs(step);
  if (end < start) {
    step = -step;
  }
  this._start = start;
  this._end = end;
  this._step = step;
  this.size = Math.max(0, Math.ceil((end - start) / step - 1) + 1);
  if (this.size === 0) {
    if (EMPTY_RANGE) {
      return EMPTY_RANGE;
    }
    EMPTY_RANGE = this;
  }
}
```
- example usage
```shell
...
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
// Map { A: 1, B: 1, C: 1 }

As well as expressing logic that would otherwise seem memory-limited:

Immutable.Range(1, Infinity)
  .skip(1000)
  .map(n => -n)
  .filter(n => n % 2 === 0)
  .take(2)
  .reduce((r, n) => r * n, 1);
// 1006008
...
```



# <a name="apidoc.module.immutable.Range.prototype"></a>[module immutable.Range.prototype](#apidoc.module.immutable.Range.prototype)

#### <a name="apidoc.element.immutable.Range.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Range.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {
  var maxIndex = this.size - 1;
  var step = this._step;
  var value = reverse ? this._start + maxIndex * step : this._start;
  for (var ii = 0; ii <= maxIndex; ii++) {
    if (fn(value, ii, this) === false) {
      return ii + 1;
    }
    value += reverse ? -step : step;
  }
  return ii;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Range.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  var maxIndex = this.size - 1;
  var step = this._step;
  var value = reverse ? this._start + maxIndex * step : this._start;
  var ii = 0;
  return new Iterator(function()  {
    var v = value;
    value += reverse ? -step : step;
    return ii > maxIndex ? iteratorDone() : iteratorValue(type, ii++, v);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>constructor (start, end, step)](#apidoc.element.immutable.Range.prototype.constructor)
- description and source-code
```javascript
function Range(start, end, step) {
  if (!(this instanceof Range)) {
    return new Range(start, end, step);
  }
  invariant(step !== 0, 'Cannot step a Range by 0');
  start = start || 0;
  if (end === undefined) {
    end = Infinity;
  }
  step = step === undefined ? 1 : Math.abs(step);
  if (end < start) {
    step = -step;
  }
  this._start = start;
  this._end = end;
  this._step = step;
  this.size = Math.max(0, Math.ceil((end - start) / step - 1) + 1);
  if (this.size === 0) {
    if (EMPTY_RANGE) {
      return EMPTY_RANGE;
    }
    EMPTY_RANGE = this;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.equals"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>equals (other)](#apidoc.element.immutable.Range.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return other instanceof Range ?
    this._start === other._start &&
    this._end === other._end &&
    this._step === other._step :
    deepEqual(this, other);
}
```
- example usage
```shell
...
interested in doing work when something has changed, you can use equality.

Immutable collections should be treated as *values* rather than *objects*. While
objects represents some thing which could change over time, a value represents
the state of that thing at a particular instance of time. This principle is most
important to understanding the appropriate use of immutable data. In order to
treat Immutable.js collections as values, it's important to use the
'Immutable.is()' function or '.equals()' method to determine value equality
instead of the '===' operator which determines object reference identity.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 2);
assert(map1.equals(map2) === true);
var map3 = map1.set('b', 50);
...
```

#### <a name="apidoc.element.immutable.Range.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Range.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  return this.has(index) ?
    this._start + wrapIndex(this, index) * this._step :
    notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Range.prototype.includes"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>includes (searchValue)](#apidoc.element.immutable.Range.prototype.includes)
- description and source-code
```javascript
includes = function (searchValue) {
  var possibleIndex = (searchValue - this._start) / this._step;
  return possibleIndex >= 0 &&
    possibleIndex < this.size &&
    possibleIndex === Math.floor(possibleIndex);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Range.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (searchValue) {
  var offsetValue = searchValue - this._start;
  if (offsetValue % this._step === 0) {
    var index = offsetValue / this._step;
    if (index >= 0 && index < this.size) {
      return index
    }
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Range.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (searchValue) {
  return this.indexOf(searchValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Range.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  if (wholeSlice(begin, end, this.size)) {
    return this;
  }
  begin = resolveBegin(begin, this.size);
  end = resolveEnd(end, this.size);
  if (end <= begin) {
    return new Range(0, 0);
  }
  return new Range(this.get(begin, this._end), this.get(end, this._end), this._step);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Range.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Range.prototype.</span>toString ()](#apidoc.element.immutable.Range.prototype.toString)
- description and source-code
```javascript
toString = function () {
  if (this.size === 0) {
    return 'Range []';
  }
  return 'Range [ ' +
    this._start + '...' + this._end +
    (this._step !== 1 ? ' by ' + this._step : '') +
  ' ]';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Record"></a>[module immutable.Record](#apidoc.module.immutable.Record)

#### <a name="apidoc.element.immutable.Record.Record"></a>[function <span class="apidocSignatureSpan">immutable.</span>Record (defaultValues, name)](#apidoc.element.immutable.Record.Record)
- description and source-code
```javascript
function Record(defaultValues, name) {
  var hasInitialized;

  var RecordType = function Record(values) {
    if (values instanceof RecordType) {
      return values;
    }
    if (!(this instanceof RecordType)) {
      return new RecordType(values);
    }
    if (!hasInitialized) {
      hasInitialized = true;
      var keys = Object.keys(defaultValues);
      setProps(RecordTypePrototype, keys);
      RecordTypePrototype.size = keys.length;
      RecordTypePrototype._name = name;
      RecordTypePrototype._keys = keys;
      RecordTypePrototype._defaultValues = defaultValues;
    }
    this._map = Map(values);
  };

  var RecordTypePrototype = RecordType.prototype = Object.create(RecordPrototype);
  RecordTypePrototype.constructor = RecordType;

  return RecordType;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Record.prototype"></a>[module immutable.Record.prototype](#apidoc.module.immutable.Record.prototype)

#### <a name="apidoc.element.immutable.Record.prototype.__ensureOwner"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Record.prototype.__ensureOwner)
- description and source-code
```javascript
__ensureOwner = function (ownerID) {
  if (ownerID === this.__ownerID) {
    return this;
  }
  var newMap = this._map && this._map.__ensureOwner(ownerID);
  if (!ownerID) {
    this.__ownerID = ownerID;
    this._map = newMap;
    return this;
  }
  return makeRecord(this, newMap, ownerID);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Record.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {var this$0 = this;
  return KeyedIterable(this._defaultValues).map(function(_, k)  {return this$0.get(k)}).__iterate(fn, reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Record.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {var this$0 = this;
  return KeyedIterable(this._defaultValues).map(function(_, k)  {return this$0.get(k)}).__iterator(type, reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.asImmutable"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>asImmutable ()](#apidoc.element.immutable.Record.prototype.asImmutable)
- description and source-code
```javascript
asImmutable = function () {
  return this.__ensureOwner();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.asMutable"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>asMutable ()](#apidoc.element.immutable.Record.prototype.asMutable)
- description and source-code
```javascript
asMutable = function () {
  return this.__ownerID ? this : this.__ensureOwner(new OwnerID());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.clear"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>clear ()](#apidoc.element.immutable.Record.prototype.clear)
- description and source-code
```javascript
clear = function () {
  if (this.__ownerID) {
    this._map && this._map.clear();
    return this;
  }
  var RecordType = this.constructor;
  return RecordType._empty || (RecordType._empty = makeRecord(this, emptyMap()));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>constructor (defaultValues, name)](#apidoc.element.immutable.Record.prototype.constructor)
- description and source-code
```javascript
function Record(defaultValues, name) {
  var hasInitialized;

  var RecordType = function Record(values) {
    if (values instanceof RecordType) {
      return values;
    }
    if (!(this instanceof RecordType)) {
      return new RecordType(values);
    }
    if (!hasInitialized) {
      hasInitialized = true;
      var keys = Object.keys(defaultValues);
      setProps(RecordTypePrototype, keys);
      RecordTypePrototype.size = keys.length;
      RecordTypePrototype._name = name;
      RecordTypePrototype._keys = keys;
      RecordTypePrototype._defaultValues = defaultValues;
    }
    this._map = Map(values);
  };

  var RecordTypePrototype = RecordType.prototype = Object.create(RecordPrototype);
  RecordTypePrototype.constructor = RecordType;

  return RecordType;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.delete"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>delete (k)](#apidoc.element.immutable.Record.prototype.delete)
- description and source-code
```javascript
delete = function (k) {
  if (!this.has(k)) {
    return this;
  }
  var newMap = this._map && this._map.remove(k);
  if (this.__ownerID || newMap === this._map) {
    return this;
  }
  return makeRecord(this, newMap);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.deleteIn"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>deleteIn (keyPath)](#apidoc.element.immutable.Record.prototype.deleteIn)
- description and source-code
```javascript
deleteIn = function (keyPath) {
  return this.updateIn(keyPath, function()  {return NOT_SET});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>get (k, notSetValue)](#apidoc.element.immutable.Record.prototype.get)
- description and source-code
```javascript
get = function (k, notSetValue) {
  if (!this.has(k)) {
    return notSetValue;
  }
  var defaultVal = this._defaultValues[k];
  return this._map ? this._map.get(k, defaultVal) : defaultVal;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Record.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>has (k)](#apidoc.element.immutable.Record.prototype.has)
- description and source-code
```javascript
has = function (k) {
  return this._defaultValues.hasOwnProperty(k);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.merge"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>merge ()](#apidoc.element.immutable.Record.prototype.merge)
- description and source-code
```javascript
merge = function () {
  return mergeIntoMapWith(this, undefined, arguments);
}
```
- example usage
```shell
...
accepts plain JavaScript Arrays and Objects anywhere a method expects an
'Iterable' with no performance penalty.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3, d:4});
var map2 = Immutable.Map({c:10, a:20, t:30});
var obj = {d:100, o:200, g:300};
var map3 = map1.merge(map2, obj);
// Map { a: 20, b: 2, c: 10, d: 100, t: 30, o: 200, g: 300 }
'''

This is possible because 'immutable' can treat any JavaScript Array or Object
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
...
```

#### <a name="apidoc.element.immutable.Record.prototype.mergeDeep"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeDeep ()](#apidoc.element.immutable.Record.prototype.mergeDeep)
- description and source-code
```javascript
mergeDeep = function () {
  return mergeIntoMapWith(this, deepMerger, arguments);
}
```
- example usage
```shell
...
'''

A few power-tools allow for reading and operating on nested data. The
most useful are 'mergeDeep', 'getIn', 'setIn', and 'updateIn', found on 'List',
'Map' and 'OrderedMap'.

'''javascript
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
...
```

#### <a name="apidoc.element.immutable.Record.prototype.mergeDeepIn"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeDeepIn (keyPath)](#apidoc.element.immutable.Record.prototype.mergeDeepIn)
- description and source-code
```javascript
mergeDeepIn = function (keyPath) {var iters = SLICE$0.call(arguments, 1);
  return this.updateIn(
    keyPath,
    emptyMap(),
    function(m ) {return typeof m.mergeDeep === 'function' ?
      m.mergeDeep.apply(m, iters) :
      iters[iters.length - 1]}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.mergeDeepWith"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.Record.prototype.mergeDeepWith)
- description and source-code
```javascript
mergeDeepWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return mergeIntoMapWith(this, deepMergerWith(merger), iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.mergeIn"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeIn (keyPath)](#apidoc.element.immutable.Record.prototype.mergeIn)
- description and source-code
```javascript
mergeIn = function (keyPath) {var iters = SLICE$0.call(arguments, 1);
  return this.updateIn(
    keyPath,
    emptyMap(),
    function(m ) {return typeof m.merge === 'function' ?
      m.merge.apply(m, iters) :
      iters[iters.length - 1]}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.mergeWith"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.Record.prototype.mergeWith)
- description and source-code
```javascript
mergeWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return mergeIntoMapWith(this, merger, iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.remove"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>remove (k)](#apidoc.element.immutable.Record.prototype.remove)
- description and source-code
```javascript
remove = function (k) {
  if (!this.has(k)) {
    return this;
  }
  var newMap = this._map && this._map.remove(k);
  if (this.__ownerID || newMap === this._map) {
    return this;
  }
  return makeRecord(this, newMap);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.removeIn"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>removeIn (keyPath)](#apidoc.element.immutable.Record.prototype.removeIn)
- description and source-code
```javascript
removeIn = function (keyPath) {
  return this.updateIn(keyPath, function()  {return NOT_SET});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.set"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>set (k, v)](#apidoc.element.immutable.Record.prototype.set)
- description and source-code
```javascript
set = function (k, v) {
  if (!this.has(k)) {
    throw new Error('Cannot set unknown key "' + k + '" on ' + recordName(this));
  }
  if (this._map && !this._map.has(k)) {
    var defaultVal = this._defaultValues[k];
    if (v === defaultVal) {
      return this;
    }
  }
  var newMap = this._map && this._map.set(k, v);
  if (this.__ownerID || newMap === this._map) {
    return this;
  }
  return makeRecord(this, newMap);
}
```
- example usage
```shell
...
'''

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
...
```

#### <a name="apidoc.element.immutable.Record.prototype.setIn"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>setIn (keyPath, v)](#apidoc.element.immutable.Record.prototype.setIn)
- description and source-code
```javascript
setIn = function (keyPath, v) {
  return this.updateIn(keyPath, NOT_SET, function()  {return v});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>toString ()](#apidoc.element.immutable.Record.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString(recordName(this) + ' {', '}');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.update"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>update (k, notSetValue, updater)](#apidoc.element.immutable.Record.prototype.update)
- description and source-code
```javascript
update = function (k, notSetValue, updater) {
  return arguments.length === 1 ?
    k(this) :
    this.updateIn([k], notSetValue, updater);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.updateIn"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>updateIn (keyPath, notSetValue, updater)](#apidoc.element.immutable.Record.prototype.updateIn)
- description and source-code
```javascript
updateIn = function (keyPath, notSetValue, updater) {
  if (!updater) {
    updater = notSetValue;
    notSetValue = undefined;
  }
  var updatedValue = updateInDeepMap(
    this,
    forceIterator(keyPath),
    notSetValue,
    updater
  );
  return updatedValue === NOT_SET ? undefined : updatedValue;
}
```
- example usage
```shell
...
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 7 } } }

var nested4 = nested3.updateIn(['a', 'b', 'c'], list => list.push(6));
// Map { a: Map { b: Map { c: List [ 3, 4, 5, 6 ], d: 7 } } }
'''
...
```

#### <a name="apidoc.element.immutable.Record.prototype.wasAltered"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>wasAltered ()](#apidoc.element.immutable.Record.prototype.wasAltered)
- description and source-code
```javascript
wasAltered = function () {
  return this._map.wasAltered();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Record.prototype.withMutations"></a>[function <span class="apidocSignatureSpan">immutable.Record.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Record.prototype.withMutations)
- description and source-code
```javascript
withMutations = function (fn) {
  var mutable = this.asMutable();
  fn(mutable);
  return mutable.wasAltered() ? mutable.__ensureOwner(this.__ownerID) : this;
}
```
- example usage
```shell
...
exactly how  'Immutable' applies complex mutations itself.

As an example, building 'list2' results in the creation of 1, not 3, new
immutable Lists.

'''javascript
var list1 = Immutable.List.of(1,2,3);
var list2 = list1.withMutations(function (list) {
  list.push(4).push(5).push(6);
});
assert(list1.size === 3);
assert(list2.size === 6);
'''

Note: 'immutable' also provides 'asMutable' and 'asImmutable', but only
...
```



# <a name="apidoc.module.immutable.Repeat"></a>[module immutable.Repeat](#apidoc.module.immutable.Repeat)

#### <a name="apidoc.element.immutable.Repeat.Repeat"></a>[function <span class="apidocSignatureSpan">immutable.</span>Repeat (value, times)](#apidoc.element.immutable.Repeat.Repeat)
- description and source-code
```javascript
function Repeat(value, times) {
  if (!(this instanceof Repeat)) {
    return new Repeat(value, times);
  }
  this._value = value;
  this.size = times === undefined ? Infinity : Math.max(0, times);
  if (this.size === 0) {
    if (EMPTY_REPEAT) {
      return EMPTY_REPEAT;
    }
    EMPTY_REPEAT = this;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Repeat.prototype"></a>[module immutable.Repeat.prototype](#apidoc.module.immutable.Repeat.prototype)

#### <a name="apidoc.element.immutable.Repeat.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Repeat.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {
  for (var ii = 0; ii < this.size; ii++) {
    if (fn(this._value, ii, this) === false) {
      return ii + 1;
    }
  }
  return ii;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Repeat.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {var this$0 = this;
  var ii = 0;
  return new Iterator(function()
    {return ii < this$0.size ? iteratorValue(type, ii++, this$0._value) : iteratorDone()}
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>constructor (value, times)](#apidoc.element.immutable.Repeat.prototype.constructor)
- description and source-code
```javascript
function Repeat(value, times) {
  if (!(this instanceof Repeat)) {
    return new Repeat(value, times);
  }
  this._value = value;
  this.size = times === undefined ? Infinity : Math.max(0, times);
  if (this.size === 0) {
    if (EMPTY_REPEAT) {
      return EMPTY_REPEAT;
    }
    EMPTY_REPEAT = this;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.equals"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>equals (other)](#apidoc.element.immutable.Repeat.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return other instanceof Repeat ?
    is(this._value, other._value) :
    deepEqual(other);
}
```
- example usage
```shell
...
interested in doing work when something has changed, you can use equality.

Immutable collections should be treated as *values* rather than *objects*. While
objects represents some thing which could change over time, a value represents
the state of that thing at a particular instance of time. This principle is most
important to understanding the appropriate use of immutable data. In order to
treat Immutable.js collections as values, it's important to use the
'Immutable.is()' function or '.equals()' method to determine value equality
instead of the '===' operator which determines object reference identity.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 2);
assert(map1.equals(map2) === true);
var map3 = map1.set('b', 50);
...
```

#### <a name="apidoc.element.immutable.Repeat.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Repeat.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  return this.has(index) ? this._value : notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Repeat.prototype.includes"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>includes (searchValue)](#apidoc.element.immutable.Repeat.prototype.includes)
- description and source-code
```javascript
includes = function (searchValue) {
  return is(this._value, searchValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Repeat.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (searchValue) {
  if (is(this._value, searchValue)) {
    return 0;
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Repeat.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (searchValue) {
  if (is(this._value, searchValue)) {
    return this.size;
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.reverse"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>reverse ()](#apidoc.element.immutable.Repeat.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Repeat.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  var size = this.size;
  return wholeSlice(begin, end, size) ? this :
    new Repeat(this._value, resolveEnd(end, size) - resolveBegin(begin, size));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Repeat.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Repeat.prototype.</span>toString ()](#apidoc.element.immutable.Repeat.prototype.toString)
- description and source-code
```javascript
toString = function () {
  if (this.size === 0) {
    return 'Repeat []';
  }
  return 'Repeat [ ' + this._value + ' ' + this.size + ' times ]';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Seq"></a>[module immutable.Seq](#apidoc.module.immutable.Seq)

#### <a name="apidoc.element.immutable.Seq.Seq"></a>[function <span class="apidocSignatureSpan">immutable.</span>Seq (value)](#apidoc.element.immutable.Seq.Seq)
- description and source-code
```javascript
function Seq(value) {
  return value === null || value === undefined ? emptySequence() :
    isIterable(value) ? value.toSeq() : seqFromValue(value);
}
```
- example usage
```shell
...
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
results, these operations can be extremely efficient.

'''javascript
var myObject = {a:1,b:2,c:3};
Immutable.Seq(myObject).map(x => x * x).toObject();
// { a: 1, b: 4, c: 9 }
'''

Keep in mind, when using JS objects to construct Immutable Maps, that
JavaScript Object properties are always strings, even if written in a quote-less
shorthand, while Immutable Maps accept keys of any type.
...
```

#### <a name="apidoc.element.immutable.Seq.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>Indexed (value)](#apidoc.element.immutable.Seq.Indexed)
- description and source-code
```javascript
function IndexedSeq(value) {
  return value === null || value === undefined ? emptySequence() :
    !isIterable(value) ? indexedSeqFromValue(value) :
    isKeyed(value) ? value.entrySeq() : value.toIndexedSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>Keyed (value)](#apidoc.element.immutable.Seq.Keyed)
- description and source-code
```javascript
function KeyedSeq(value) {
  return value === null || value === undefined ?
    emptySequence().toKeyedSeq() :
    isIterable(value) ?
      (isKeyed(value) ? value.toSeq() : value.fromEntrySeq()) :
      keyedSeqFromValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>Set (value)](#apidoc.element.immutable.Seq.Set)
- description and source-code
```javascript
function SetSeq(value) {
  return (
    value === null || value === undefined ? emptySequence() :
    !isIterable(value) ? indexedSeqFromValue(value) :
    isKeyed(value) ? value.entrySeq() : value
  ).toSetSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.isSeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>isSeq (maybeSeq)](#apidoc.element.immutable.Seq.isSeq)
- description and source-code
```javascript
function isSeq(maybeSeq) {
  return !!(maybeSeq && maybeSeq[IS_SEQ_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.of"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>of ()](#apidoc.element.immutable.Seq.of)
- description and source-code
```javascript
of = function () {
  return Seq(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.Seq.Indexed"></a>[module immutable.Seq.Indexed](#apidoc.module.immutable.Seq.Indexed)

#### <a name="apidoc.element.immutable.Seq.Indexed.Indexed"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>Indexed (value)](#apidoc.element.immutable.Seq.Indexed.Indexed)
- description and source-code
```javascript
function IndexedSeq(value) {
  return value === null || value === undefined ? emptySequence() :
    !isIterable(value) ? indexedSeqFromValue(value) :
    isKeyed(value) ? value.entrySeq() : value.toIndexedSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.of"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.</span>of ()](#apidoc.element.immutable.Seq.Indexed.of)
- description and source-code
```javascript
of = function () {
  return IndexedSeq(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.Seq.Indexed.prototype"></a>[module immutable.Seq.Indexed.prototype](#apidoc.module.immutable.Seq.Indexed.prototype)

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Seq.Indexed.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {
  return seqIterate(this, fn, reverse, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Seq.Indexed.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  return seqIterator(this, type, reverse, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.Indexed.prototype.constructor)
- description and source-code
```javascript
function IndexedIterable(value) {
  return isIndexed(value) ? value : IndexedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.filter"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>filter (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.filter)
- description and source-code
```javascript
filter = function (predicate, context) {
  return reify(this, filterFactory(this, predicate, context, false));
}
```
- example usage
```shell
...
**Seq is lazy** — Seq does as little work as necessary to respond to any
method call.

For example, the following does not perform any work, because the resulting
Seq is never used:

var oddSquares = Immutable.Seq.of(1,2,3,4,5,6,7,8)
  .filter(x => x % 2).map(x => x * x);

Once the Seq is used, it performs only the work necessary. In this
example, no intermediate arrays are ever created, filter is called three times,
and map is only called twice:

console.log(oddSquares.get(1)); // 9
...
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>findIndex (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.findIndex)
- description and source-code
```javascript
findIndex = function (predicate, context) {
  var entry = this.findEntry(predicate, context);
  return entry ? entry[0] : -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.findLastIndex"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>findLastIndex (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.findLastIndex)
- description and source-code
```javascript
findLastIndex = function (predicate, context) {
  var entry = this.findLastEntry(predicate, context);
  return entry ? entry[0] : -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.first"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>first ()](#apidoc.element.immutable.Seq.Indexed.prototype.first)
- description and source-code
```javascript
first = function () {
  return this.get(0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.flatten"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>flatten (depth)](#apidoc.element.immutable.Seq.Indexed.prototype.flatten)
- description and source-code
```javascript
flatten = function (depth) {
  return reify(this, flattenFactory(this, depth, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Seq.Indexed.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  index = wrapIndex(this, index);
  return (index < 0 || (this.size === Infinity ||
      (this.size !== undefined && index > this.size))) ?
    notSetValue :
    this.find(function(_, key)  {return key === index}, undefined, notSetValue);
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>has (index)](#apidoc.element.immutable.Seq.Indexed.prototype.has)
- description and source-code
```javascript
has = function (index) {
  index = wrapIndex(this, index);
  return index >= 0 && (this.size !== undefined ?
    this.size === Infinity || index < this.size :
    this.indexOf(index) !== -1
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>indexOf (searchValue)](#apidoc.element.immutable.Seq.Indexed.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (searchValue) {
  var key = this.keyOf(searchValue);
  return key === undefined ? -1 : key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.interleave"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>interleave ()](#apidoc.element.immutable.Seq.Indexed.prototype.interleave)
- description and source-code
```javascript
interleave = function () {
  var iterables = [this].concat(arrCopy(arguments));
  var zipped = zipWithFactory(this.toSeq(), IndexedSeq.of, iterables);
  var interleaved = zipped.flatten(true);
  if (zipped.size) {
    interleaved.size = zipped.size * iterables.length;
  }
  return reify(this, interleaved);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.interpose"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>interpose (separator)](#apidoc.element.immutable.Seq.Indexed.prototype.interpose)
- description and source-code
```javascript
interpose = function (separator) {
  return reify(this, interposeFactory(this, separator));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>keySeq ()](#apidoc.element.immutable.Seq.Indexed.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return Range(0, this.size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.last"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>last ()](#apidoc.element.immutable.Seq.Indexed.prototype.last)
- description and source-code
```javascript
last = function () {
  return this.get(-1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>lastIndexOf (searchValue)](#apidoc.element.immutable.Seq.Indexed.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (searchValue) {
  var key = this.lastKeyOf(searchValue);
  return key === undefined ? -1 : key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.reverse"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>reverse ()](#apidoc.element.immutable.Seq.Indexed.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  return reify(this, reverseFactory(this, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.skipWhile"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>skipWhile (predicate, context)](#apidoc.element.immutable.Seq.Indexed.prototype.skipWhile)
- description and source-code
```javascript
skipWhile = function (predicate, context) {
  return reify(this, skipWhileFactory(this, predicate, context, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Seq.Indexed.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  return reify(this, sliceFactory(this, begin, end, false));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.splice"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>splice (index, removeNum)](#apidoc.element.immutable.Seq.Indexed.prototype.splice)
- description and source-code
```javascript
splice = function (index, removeNum) {
  var numArgs = arguments.length;
  removeNum = Math.max(removeNum | 0, 0);
  if (numArgs === 0 || (numArgs === 2 && !removeNum)) {
    return this;
  }
  // If index is negative, it should resolve relative to the size of the
  // collection. However size may be expensive to compute if not cached, so
  // only call count() if the number is in fact negative.
  index = resolveBegin(index, index < 0 ? this.count() : this.size);
  var spliced = this.slice(0, index);
  return reify(
    this,
    numArgs === 1 ?
      spliced :
      spliced.concat(arrCopy(arguments, 2), this.slice(index + removeNum))
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.toIndexedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>toIndexedSeq ()](#apidoc.element.immutable.Seq.Indexed.prototype.toIndexedSeq)
- description and source-code
```javascript
toIndexedSeq = function () {
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.toKeyedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Seq.Indexed.prototype.toKeyedSeq)
- description and source-code
```javascript
toKeyedSeq = function () {
  return new ToKeyedSequence(this, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>toString ()](#apidoc.element.immutable.Seq.Indexed.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('Seq [', ']');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.zip"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>zip ()](#apidoc.element.immutable.Seq.Indexed.prototype.zip)
- description and source-code
```javascript
zip = function () {
  var iterables = [this].concat(arrCopy(arguments));
  return reify(this, zipWithFactory(this, defaultZipper, iterables));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Indexed.prototype.zipWith"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Indexed.prototype.</span>zipWith (zipper)](#apidoc.element.immutable.Seq.Indexed.prototype.zipWith)
- description and source-code
```javascript
zipWith = function (zipper) {
  var iterables = arrCopy(arguments);
  iterables[0] = this;
  return reify(this, zipWithFactory(this, zipper, iterables));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Seq.Keyed"></a>[module immutable.Seq.Keyed](#apidoc.module.immutable.Seq.Keyed)

#### <a name="apidoc.element.immutable.Seq.Keyed.Keyed"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>Keyed (value)](#apidoc.element.immutable.Seq.Keyed.Keyed)
- description and source-code
```javascript
function KeyedSeq(value) {
  return value === null || value === undefined ?
    emptySequence().toKeyedSeq() :
    isIterable(value) ?
      (isKeyed(value) ? value.toSeq() : value.fromEntrySeq()) :
      keyedSeqFromValue(value);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Seq.Keyed.prototype"></a>[module immutable.Seq.Keyed.prototype](#apidoc.module.immutable.Seq.Keyed.prototype)

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.__toJS"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>__toJS ()](#apidoc.element.immutable.Seq.Keyed.prototype.__toJS)
- description and source-code
```javascript
__toJS = function () {
  assertNotInfinite(this.size);
  var object = {};
  this.__iterate(function(v, k)  { object[k] = v; });
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.__toStringMapper"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>__toStringMapper (v, k)](#apidoc.element.immutable.Seq.Keyed.prototype.__toStringMapper)
- description and source-code
```javascript
__toStringMapper = function (v, k)  {return JSON.stringify(k) + ': ' + quoteString(v)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.Keyed.prototype.constructor)
- description and source-code
```javascript
function KeyedIterable(value) {
  return isKeyed(value) ? value : KeyedSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.flip"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>flip ()](#apidoc.element.immutable.Seq.Keyed.prototype.flip)
- description and source-code
```javascript
flip = function () {
  return reify(this, flipFactory(this));
}
```
- example usage
```shell
...
Any collection can be converted to a lazy Seq with '.toSeq()'.

var seq = Immutable.Map({a:1, b:1, c:1}).toSeq();

Seq allow for the efficient chaining of sequence operations, especially when
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
// Map { A: 1, B: 1, C: 1 }

As well as expressing logic that would otherwise seem memory-limited:

Immutable.Range(1, Infinity)
  .skip(1000)
  .map(n => -n)
...
```

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.mapEntries"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>mapEntries (mapper, context)](#apidoc.element.immutable.Seq.Keyed.prototype.mapEntries)
- description and source-code
```javascript
mapEntries = function (mapper, context) {var this$0 = this;
  var iterations = 0;
  return reify(this,
    this.toSeq().map(
      function(v, k)  {return mapper.call(context, [k, v], iterations++, this$0)}
    ).fromEntrySeq()
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.mapKeys"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>mapKeys (mapper, context)](#apidoc.element.immutable.Seq.Keyed.prototype.mapKeys)
- description and source-code
```javascript
mapKeys = function (mapper, context) {var this$0 = this;
  return reify(this,
    this.toSeq().flip().map(
      function(k, v)  {return mapper.call(context, k, v, this$0)}
    ).flip()
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Keyed.prototype.toKeyedSeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Keyed.prototype.</span>toKeyedSeq ()](#apidoc.element.immutable.Seq.Keyed.prototype.toKeyedSeq)
- description and source-code
```javascript
toKeyedSeq = function () {
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Seq.Set"></a>[module immutable.Seq.Set](#apidoc.module.immutable.Seq.Set)

#### <a name="apidoc.element.immutable.Seq.Set.Set"></a>[function <span class="apidocSignatureSpan">immutable.Seq.</span>Set (value)](#apidoc.element.immutable.Seq.Set.Set)
- description and source-code
```javascript
function SetSeq(value) {
  return (
    value === null || value === undefined ? emptySequence() :
    !isIterable(value) ? indexedSeqFromValue(value) :
    isKeyed(value) ? value.entrySeq() : value
  ).toSetSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set.of"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.</span>of ()](#apidoc.element.immutable.Seq.Set.of)
- description and source-code
```javascript
of = function () {
  return SetSeq(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.Seq.Set.prototype"></a>[module immutable.Seq.Set.prototype](#apidoc.module.immutable.Seq.Set.prototype)

#### <a name="apidoc.element.immutable.Seq.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.Set.prototype.constructor)
- description and source-code
```javascript
function SetIterable(value) {
  return isIterable(value) && !isAssociative(value) ? value : SetSeq(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set.prototype.contains"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>contains (value)](#apidoc.element.immutable.Seq.Set.prototype.contains)
- description and source-code
```javascript
contains = function (value) {
  return this.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>get (value, notSetValue)](#apidoc.element.immutable.Seq.Set.prototype.get)
- description and source-code
```javascript
get = function (value, notSetValue) {
  return this.has(value) ? value : notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Seq.Set.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>has (searchValue)](#apidoc.element.immutable.Seq.Set.prototype.has)
- description and source-code
```javascript
has = function (searchValue) {
  return this.some(function(value ) {return is(value, searchValue)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set.prototype.includes"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>includes (value)](#apidoc.element.immutable.Seq.Set.prototype.includes)
- description and source-code
```javascript
includes = function (value) {
  return this.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set.prototype.keySeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>keySeq ()](#apidoc.element.immutable.Seq.Set.prototype.keySeq)
- description and source-code
```javascript
keySeq = function () {
  return this.valueSeq();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.Set.prototype.toSetSeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.Set.prototype.</span>toSetSeq ()](#apidoc.element.immutable.Seq.Set.prototype.toSetSeq)
- description and source-code
```javascript
toSetSeq = function () {
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Seq.prototype"></a>[module immutable.Seq.prototype](#apidoc.module.immutable.Seq.prototype)

#### <a name="apidoc.element.immutable.Seq.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Seq.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {
  return seqIterate(this, fn, reverse, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Seq.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  return seqIterator(this, type, reverse, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.prototype.cacheResult"></a>[function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>cacheResult ()](#apidoc.element.immutable.Seq.prototype.cacheResult)
- description and source-code
```javascript
cacheResult = function () {
  if (!this._cache && this.__iterateUncached) {
    this._cache = this.entrySeq().toArray();
    this.size = this._cache.length;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>constructor (value)](#apidoc.element.immutable.Seq.prototype.constructor)
- description and source-code
```javascript
function Seq(value) {
  return value === null || value === undefined ? emptySequence() :
    isIterable(value) ? value.toSeq() : seqFromValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Seq.prototype.toSeq"></a>[function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>toSeq ()](#apidoc.element.immutable.Seq.prototype.toSeq)
- description and source-code
```javascript
toSeq = function () {
  return this;
}
```
- example usage
```shell
...

Once the Seq is used, it performs only the work necessary. In this
example, no intermediate arrays are ever created, filter is called three times,
and map is only called twice:

console.log(oddSquares.get(1)); // 9

Any collection can be converted to a lazy Seq with '.toSeq()'.

var seq = Immutable.Map({a:1, b:1, c:1}).toSeq();

Seq allow for the efficient chaining of sequence operations, especially when
converting to a different concrete type (such as to a JS object):

seq.flip().map(key => key.toUpperCase()).flip().toObject();
...
```

#### <a name="apidoc.element.immutable.Seq.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Seq.prototype.</span>toString ()](#apidoc.element.immutable.Seq.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('Seq {', '}');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.immutable.Set"></a>[module immutable.Set](#apidoc.module.immutable.Set)

#### <a name="apidoc.element.immutable.Set.Set"></a>[function <span class="apidocSignatureSpan">immutable.</span>Set (value)](#apidoc.element.immutable.Set.Set)
- description and source-code
```javascript
function Set(value) {
  return value === null || value === undefined ? emptySet() :
    isSet(value) && !isOrdered(value) ? value :
    emptySet().withMutations(function(set ) {
      var iter = SetIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v ) {return set.add(v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.fromKeys"></a>[function <span class="apidocSignatureSpan">immutable.Set.</span>fromKeys (value)](#apidoc.element.immutable.Set.fromKeys)
- description and source-code
```javascript
fromKeys = function (value) {
  return this(KeyedIterable(value).keySeq());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.isSet"></a>[function <span class="apidocSignatureSpan">immutable.Set.</span>isSet (maybeSet)](#apidoc.element.immutable.Set.isSet)
- description and source-code
```javascript
function isSet(maybeSet) {
  return !!(maybeSet && maybeSet[IS_SET_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.of"></a>[function <span class="apidocSignatureSpan">immutable.Set.</span>of ()](#apidoc.element.immutable.Set.of)
- description and source-code
```javascript
of = function () {
  return this(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.Set.prototype"></a>[module immutable.Set.prototype](#apidoc.module.immutable.Set.prototype)

#### <a name="apidoc.element.immutable.Set.prototype.__empty"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__empty ()](#apidoc.element.immutable.Set.prototype.__empty)
- description and source-code
```javascript
function emptySet() {
  return EMPTY_SET || (EMPTY_SET = makeSet(emptyMap()));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.__ensureOwner"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Set.prototype.__ensureOwner)
- description and source-code
```javascript
__ensureOwner = function (ownerID) {
  if (ownerID === this.__ownerID) {
    return this;
  }
  var newMap = this._map.__ensureOwner(ownerID);
  if (!ownerID) {
    this.__ownerID = ownerID;
    this._map = newMap;
    return this;
  }
  return this.__make(newMap, ownerID);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Set.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {var this$0 = this;
  return this._map.__iterate(function(_, k)  {return fn(k, k, this$0)}, reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Set.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  return this._map.map(function(_, k)  {return k}).__iterator(type, reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.__make"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>__make (map, ownerID)](#apidoc.element.immutable.Set.prototype.__make)
- description and source-code
```javascript
function makeSet(map, ownerID) {
  var set = Object.create(SetPrototype);
  set.size = map ? map.size : 0;
  set._map = map;
  set.__ownerID = ownerID;
  return set;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.add"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>add (value)](#apidoc.element.immutable.Set.prototype.add)
- description and source-code
```javascript
add = function (value) {
  return updateSet(this, this._map.set(value, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.asImmutable"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>asImmutable ()](#apidoc.element.immutable.Set.prototype.asImmutable)
- description and source-code
```javascript
asImmutable = function () {
  return this.__ensureOwner();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.asMutable"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>asMutable ()](#apidoc.element.immutable.Set.prototype.asMutable)
- description and source-code
```javascript
asMutable = function () {
  return this.__ownerID ? this : this.__ensureOwner(new OwnerID());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.clear"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>clear ()](#apidoc.element.immutable.Set.prototype.clear)
- description and source-code
```javascript
clear = function () {
  return updateSet(this, this._map.clear());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>constructor (value)](#apidoc.element.immutable.Set.prototype.constructor)
- description and source-code
```javascript
function Set(value) {
  return value === null || value === undefined ? emptySet() :
    isSet(value) && !isOrdered(value) ? value :
    emptySet().withMutations(function(set ) {
      var iter = SetIterable(value);
      assertNotInfinite(iter.size);
      iter.forEach(function(v ) {return set.add(v)});
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.delete"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>delete (value)](#apidoc.element.immutable.Set.prototype.delete)
- description and source-code
```javascript
delete = function (value) {
  return updateSet(this, this._map.remove(value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.has"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>has (value)](#apidoc.element.immutable.Set.prototype.has)
- description and source-code
```javascript
has = function (value) {
  return this._map.has(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.intersect"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>intersect ()](#apidoc.element.immutable.Set.prototype.intersect)
- description and source-code
```javascript
intersect = function () {var iters = SLICE$0.call(arguments, 0);
  if (iters.length === 0) {
    return this;
  }
  iters = iters.map(function(iter ) {return SetIterable(iter)});
  var originalSet = this;
  return this.withMutations(function(set ) {
    originalSet.forEach(function(value ) {
      if (!iters.every(function(iter ) {return iter.includes(value)})) {
        set.remove(value);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.merge"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>merge ()](#apidoc.element.immutable.Set.prototype.merge)
- description and source-code
```javascript
merge = function () {
  return this.union.apply(this, arguments);
}
```
- example usage
```shell
...
accepts plain JavaScript Arrays and Objects anywhere a method expects an
'Iterable' with no performance penalty.

'''javascript
var map1 = Immutable.Map({a:1, b:2, c:3, d:4});
var map2 = Immutable.Map({c:10, a:20, t:30});
var obj = {d:100, o:200, g:300};
var map3 = map1.merge(map2, obj);
// Map { a: 20, b: 2, c: 10, d: 100, t: 30, o: 200, g: 300 }
'''

This is possible because 'immutable' can treat any JavaScript Array or Object
as an Iterable. You can take advantage of this in order to get sophisticated
collection methods on JavaScript Objects, which otherwise have a very sparse
native API. Because Seq evaluates lazily and does not cache intermediate
...
```

#### <a name="apidoc.element.immutable.Set.prototype.mergeDeep"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>mergeDeep ()](#apidoc.element.immutable.Set.prototype.mergeDeep)
- description and source-code
```javascript
mergeDeep = function () {
  return this.union.apply(this, arguments);
}
```
- example usage
```shell
...
'''

A few power-tools allow for reading and operating on nested data. The
most useful are 'mergeDeep', 'getIn', 'setIn', and 'updateIn', found on 'List',
'Map' and 'OrderedMap'.

'''javascript
var nested2 = nested.mergeDeep({a:{b:{d:6}}});
// Map { a: Map { b: Map { c: List [ 3, 4, 5 ], d: 6 } } }
'''

'''javascript
nested2.getIn(['a', 'b', 'd']); // 6

var nested3 = nested2.updateIn(['a', 'b', 'd'], value => value + 1);
...
```

#### <a name="apidoc.element.immutable.Set.prototype.mergeDeepWith"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>mergeDeepWith (merger)](#apidoc.element.immutable.Set.prototype.mergeDeepWith)
- description and source-code
```javascript
mergeDeepWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return this.union.apply(this, iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.mergeWith"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>mergeWith (merger)](#apidoc.element.immutable.Set.prototype.mergeWith)
- description and source-code
```javascript
mergeWith = function (merger) {var iters = SLICE$0.call(arguments, 1);
  return this.union.apply(this, iters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.remove"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>remove (value)](#apidoc.element.immutable.Set.prototype.remove)
- description and source-code
```javascript
remove = function (value) {
  return updateSet(this, this._map.remove(value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.sort"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>sort (comparator)](#apidoc.element.immutable.Set.prototype.sort)
- description and source-code
```javascript
sort = function (comparator) {
  // Late binding
  return OrderedSet(sortFactory(this, comparator));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>sortBy (mapper, comparator)](#apidoc.element.immutable.Set.prototype.sortBy)
- description and source-code
```javascript
sortBy = function (mapper, comparator) {
  // Late binding
  return OrderedSet(sortFactory(this, comparator, mapper));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.subtract"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>subtract ()](#apidoc.element.immutable.Set.prototype.subtract)
- description and source-code
```javascript
subtract = function () {var iters = SLICE$0.call(arguments, 0);
  if (iters.length === 0) {
    return this;
  }
  iters = iters.map(function(iter ) {return SetIterable(iter)});
  var originalSet = this;
  return this.withMutations(function(set ) {
    originalSet.forEach(function(value ) {
      if (iters.some(function(iter ) {return iter.includes(value)})) {
        set.remove(value);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>toString ()](#apidoc.element.immutable.Set.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('Set {', '}');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.union"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>union ()](#apidoc.element.immutable.Set.prototype.union)
- description and source-code
```javascript
union = function () {var iters = SLICE$0.call(arguments, 0);
  iters = iters.filter(function(x ) {return x.size !== 0});
  if (iters.length === 0) {
    return this;
  }
  if (this.size === 0 && !this.__ownerID && iters.length === 1) {
    return this.constructor(iters[0]);
  }
  return this.withMutations(function(set ) {
    for (var ii = 0; ii < iters.length; ii++) {
      SetIterable(iters[ii]).forEach(function(value ) {return set.add(value)});
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.wasAltered"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>wasAltered ()](#apidoc.element.immutable.Set.prototype.wasAltered)
- description and source-code
```javascript
wasAltered = function () {
  return this._map.wasAltered();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Set.prototype.withMutations"></a>[function <span class="apidocSignatureSpan">immutable.Set.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Set.prototype.withMutations)
- description and source-code
```javascript
withMutations = function (fn) {
  var mutable = this.asMutable();
  fn(mutable);
  return mutable.wasAltered() ? mutable.__ensureOwner(this.__ownerID) : this;
}
```
- example usage
```shell
...
exactly how  'Immutable' applies complex mutations itself.

As an example, building 'list2' results in the creation of 1, not 3, new
immutable Lists.

'''javascript
var list1 = Immutable.List.of(1,2,3);
var list2 = list1.withMutations(function (list) {
  list.push(4).push(5).push(6);
});
assert(list1.size === 3);
assert(list2.size === 6);
'''

Note: 'immutable' also provides 'asMutable' and 'asImmutable', but only
...
```



# <a name="apidoc.module.immutable.Stack"></a>[module immutable.Stack](#apidoc.module.immutable.Stack)

#### <a name="apidoc.element.immutable.Stack.Stack"></a>[function <span class="apidocSignatureSpan">immutable.</span>Stack (value)](#apidoc.element.immutable.Stack.Stack)
- description and source-code
```javascript
function Stack(value) {
  return value === null || value === undefined ? emptyStack() :
    isStack(value) ? value :
    emptyStack().unshiftAll(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.isStack"></a>[function <span class="apidocSignatureSpan">immutable.Stack.</span>isStack (maybeStack)](#apidoc.element.immutable.Stack.isStack)
- description and source-code
```javascript
function isStack(maybeStack) {
  return !!(maybeStack && maybeStack[IS_STACK_SENTINEL]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.of"></a>[function <span class="apidocSignatureSpan">immutable.Stack.</span>of ()](#apidoc.element.immutable.Stack.of)
- description and source-code
```javascript
of = function () {
  return this(arguments);
}
```
- example usage
```shell
...

The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
...
```



# <a name="apidoc.module.immutable.Stack.prototype"></a>[module immutable.Stack.prototype](#apidoc.module.immutable.Stack.prototype)

#### <a name="apidoc.element.immutable.Stack.prototype.__ensureOwner"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>__ensureOwner (ownerID)](#apidoc.element.immutable.Stack.prototype.__ensureOwner)
- description and source-code
```javascript
__ensureOwner = function (ownerID) {
  if (ownerID === this.__ownerID) {
    return this;
  }
  if (!ownerID) {
    this.__ownerID = ownerID;
    this.__altered = false;
    return this;
  }
  return makeStack(this.size, this._head, ownerID, this.__hash);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.__iterate"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>__iterate (fn, reverse)](#apidoc.element.immutable.Stack.prototype.__iterate)
- description and source-code
```javascript
__iterate = function (fn, reverse) {
  if (reverse) {
    return this.reverse().__iterate(fn);
  }
  var iterations = 0;
  var node = this._head;
  while (node) {
    if (fn(node.value, iterations++, this) === false) {
      break;
    }
    node = node.next;
  }
  return iterations;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.__iterator"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>__iterator (type, reverse)](#apidoc.element.immutable.Stack.prototype.__iterator)
- description and source-code
```javascript
__iterator = function (type, reverse) {
  if (reverse) {
    return this.reverse().__iterator(type);
  }
  var iterations = 0;
  var node = this._head;
  return new Iterator(function()  {
    if (node) {
      var value = node.value;
      node = node.next;
      return iteratorValue(type, iterations++, value);
    }
    return iteratorDone();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.asImmutable"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>asImmutable ()](#apidoc.element.immutable.Stack.prototype.asImmutable)
- description and source-code
```javascript
asImmutable = function () {
  return this.__ensureOwner();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.asMutable"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>asMutable ()](#apidoc.element.immutable.Stack.prototype.asMutable)
- description and source-code
```javascript
asMutable = function () {
  return this.__ownerID ? this : this.__ensureOwner(new OwnerID());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.clear"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>clear ()](#apidoc.element.immutable.Stack.prototype.clear)
- description and source-code
```javascript
clear = function () {
  if (this.size === 0) {
    return this;
  }
  if (this.__ownerID) {
    this.size = 0;
    this._head = undefined;
    this.__hash = undefined;
    this.__altered = true;
    return this;
  }
  return emptyStack();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.constructor"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>constructor (value)](#apidoc.element.immutable.Stack.prototype.constructor)
- description and source-code
```javascript
function Stack(value) {
  return value === null || value === undefined ? emptyStack() :
    isStack(value) ? value :
    emptyStack().unshiftAll(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.get"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>get (index, notSetValue)](#apidoc.element.immutable.Stack.prototype.get)
- description and source-code
```javascript
get = function (index, notSetValue) {
  var head = this._head;
  index = wrapIndex(this, index);
  while (head && index--) {
    head = head.next;
  }
  return head ? head.value : notSetValue;
}
```
- example usage
```shell
...

Then require it into any module.

'''javascript
var Immutable = require('immutable');
var map1 = Immutable.Map({a:1, b:2, c:3});
var map2 = map1.set('b', 50);
map1.get('b'); // 2
map2.get('b'); // 50
'''

### Browser

To use 'immutable' from a browser, download [dist/immutable.min.js](https://github.com/facebook/immutable-js/blob/master/dist/immutable
.min.js)
or use a CDN such as [CDNJS](https://cdnjs.com/libraries/immutable)
...
```

#### <a name="apidoc.element.immutable.Stack.prototype.peek"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>peek ()](#apidoc.element.immutable.Stack.prototype.peek)
- description and source-code
```javascript
peek = function () {
  return this._head && this._head.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.pop"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>pop ()](#apidoc.element.immutable.Stack.prototype.pop)
- description and source-code
```javascript
pop = function () {
  return this.slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.push"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>push ()](#apidoc.element.immutable.Stack.prototype.push)
- description and source-code
```javascript
push = function () {
  if (arguments.length === 0) {
    return this;
  }
  var newSize = this.size + arguments.length;
  var head = this._head;
  for (var ii = arguments.length - 1; ii >= 0; ii--) {
    head = {
      value: arguments[ii],
      next: head
    };
  }
  if (this.__ownerID) {
    this.size = newSize;
    this._head = head;
    this.__hash = undefined;
    this.__altered = true;
    return this;
  }
  return makeStack(newSize, head);
}
```
- example usage
```shell
...
The difference for the immutable collections is that methods which would mutate
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
assert(list4.get(0) === 1);
...
```

#### <a name="apidoc.element.immutable.Stack.prototype.pushAll"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>pushAll (iter)](#apidoc.element.immutable.Stack.prototype.pushAll)
- description and source-code
```javascript
pushAll = function (iter) {
  iter = IndexedIterable(iter);
  if (iter.size === 0) {
    return this;
  }
  assertNotInfinite(iter.size);
  var newSize = this.size;
  var head = this._head;
  iter.reverse().forEach(function(value ) {
    newSize++;
    head = {
      value: value,
      next: head
    };
  });
  if (this.__ownerID) {
    this.size = newSize;
    this._head = head;
    this.__hash = undefined;
    this.__altered = true;
    return this;
  }
  return makeStack(newSize, head);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.shift"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>shift ()](#apidoc.element.immutable.Stack.prototype.shift)
- description and source-code
```javascript
shift = function () {
  return this.pop.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.slice"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>slice (begin, end)](#apidoc.element.immutable.Stack.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  if (wholeSlice(begin, end, this.size)) {
    return this;
  }
  var resolvedBegin = resolveBegin(begin, this.size);
  var resolvedEnd = resolveEnd(end, this.size);
  if (resolvedEnd !== this.size) {
    // super.slice(begin, end);
    return IndexedCollection.prototype.slice.call(this, begin, end);
  }
  var newSize = this.size - resolvedBegin;
  var head = this._head;
  while (resolvedBegin--) {
    head = head.next;
  }
  if (this.__ownerID) {
    this.size = newSize;
    this._head = head;
    this.__hash = undefined;
    this.__altered = true;
    return this;
  }
  return makeStack(newSize, head);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.toString"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>toString ()](#apidoc.element.immutable.Stack.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.__toString('Stack [', ']');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.unshift"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>unshift ()](#apidoc.element.immutable.Stack.prototype.unshift)
- description and source-code
```javascript
unshift = function () {
  return this.push.apply(this, arguments);
}
```
- example usage
```shell
...
the collection, like 'push', 'set', 'unshift' or 'splice' instead return a new
immutable collection. Methods which return new arrays like 'slice' or 'concat'
instead return new immutable collections.

'''javascript
var list1 = Immutable.List.of(1, 2);
var list2 = list1.push(3, 4, 5);
var list3 = list2.unshift(0);
var list4 = list1.concat(list2, list3);
assert(list1.size === 2);
assert(list2.size === 5);
assert(list3.size === 6);
assert(list4.size === 13);
assert(list4.get(0) === 1);
'''
...
```

#### <a name="apidoc.element.immutable.Stack.prototype.unshiftAll"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>unshiftAll (iter)](#apidoc.element.immutable.Stack.prototype.unshiftAll)
- description and source-code
```javascript
unshiftAll = function (iter) {
  return this.pushAll(iter);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.wasAltered"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>wasAltered ()](#apidoc.element.immutable.Stack.prototype.wasAltered)
- description and source-code
```javascript
wasAltered = function () {
  return this.__altered;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.immutable.Stack.prototype.withMutations"></a>[function <span class="apidocSignatureSpan">immutable.Stack.prototype.</span>withMutations (fn)](#apidoc.element.immutable.Stack.prototype.withMutations)
- description and source-code
```javascript
withMutations = function (fn) {
  var mutable = this.asMutable();
  fn(mutable);
  return mutable.wasAltered() ? mutable.__ensureOwner(this.__ownerID) : this;
}
```
- example usage
```shell
...
exactly how  'Immutable' applies complex mutations itself.

As an example, building 'list2' results in the creation of 1, not 3, new
immutable Lists.

'''javascript
var list1 = Immutable.List.of(1,2,3);
var list2 = list1.withMutations(function (list) {
  list.push(4).push(5).push(6);
});
assert(list1.size === 3);
assert(list2.size === 6);
'''

Note: 'immutable' also provides 'asMutable' and 'asImmutable', but only
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
