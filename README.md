# api documentation for  [psd (v3.1.0)](https://github.com/meltingice/psd.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-psd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-psd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-psd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-psd)
#### A general purpose Photoshop file parser.

[![NPM](https://nodei.co/npm/psd.png?downloads=true)](https://www.npmjs.com/package/psd)

[![apidoc](https://npmdoc.github.io/node-npmdoc-psd/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-psd_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-psd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-psd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-psd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/meltingice/psd.js/issues"
    },
    "dependencies": {
        "coffee-script": "~ 1.7.1",
        "coffeescript-module": "~ 0.2.1",
        "iconv-lite": "~ 0.4.4",
        "jspack": "~ 0.0.3",
        "lodash": "~ 2.4",
        "parse-engine-data": "~ 0.1",
        "pngjs": "~ 0.4.0",
        "rsvp": "~ 3.0.6"
    },
    "description": "A general purpose Photoshop file parser.",
    "devDependencies": {
        "browserify": "~ 3.46.0",
        "codo": "~ 2.0.11",
        "coffeeify": "~ 0.6.0",
        "mocha": "~ 1.18.2",
        "rimraf": "~ 2.2.8",
        "should": "~ 3.3.1"
    },
    "directories": {},
    "dist": {
        "shasum": "e84c68b694261bcba4bfb92041cb56d2410e4115",
        "tarball": "https://registry.npmjs.org/psd/-/psd-3.1.0.tgz"
    },
    "gitHead": "825a536da444d52e3b416ed3bba6113c82cbdca1",
    "homepage": "https://github.com/meltingice/psd.js",
    "keywords": [
        "psd",
        "parser",
        "photoshop",
        "adobe",
        "reader"
    ],
    "main": "./index.js",
    "maintainers": [
        {
            "name": "mnutt",
            "email": "michael@nuttnet.net"
        },
        {
            "name": "meltingice",
            "email": "meltingice8917@gmail.com"
        }
    ],
    "name": "psd",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/meltingice/psd.js.git"
    },
    "scripts": {
        "test": "mocha test"
    },
    "version": "3.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module psd](#apidoc.module.psd)
1.  [function <span class="apidocSignatureSpan">psd.</span>Node.Root (psd)](#apidoc.element.psd.Node.Root)
1.  [function <span class="apidocSignatureSpan">psd.</span>aliasFunction (to, from)](#apidoc.element.psd.aliasFunction)
1.  [function <span class="apidocSignatureSpan">psd.</span>aliasProperty (to, from)](#apidoc.element.psd.aliasProperty)
1.  [function <span class="apidocSignatureSpan">psd.</span>delegate ()](#apidoc.element.psd.delegate)
1.  [function <span class="apidocSignatureSpan">psd.</span>extends (obj)](#apidoc.element.psd.extends)
1.  [function <span class="apidocSignatureSpan">psd.</span>fromFile (file)](#apidoc.element.psd.fromFile)
1.  [function <span class="apidocSignatureSpan">psd.</span>included (func)](#apidoc.element.psd.included)
1.  [function <span class="apidocSignatureSpan">psd.</span>includes (obj)](#apidoc.element.psd.includes)
1.  [function <span class="apidocSignatureSpan">psd.</span>open (file)](#apidoc.element.psd.open)
1.  object <span class="apidocSignatureSpan">psd.</span>Node
1.  object <span class="apidocSignatureSpan">psd.</span>Node.Root.prototype
1.  object <span class="apidocSignatureSpan">psd.</span>__super__

#### [module psd.Node](#apidoc.module.psd.Node)
1.  [function <span class="apidocSignatureSpan">psd.Node.</span>Root (psd)](#apidoc.element.psd.Node.Root)

#### [module psd.Node.Root](#apidoc.module.psd.Node.Root)
1.  [function <span class="apidocSignatureSpan">psd.Node.</span>Root (psd)](#apidoc.element.psd.Node.Root.Root)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>aliasFunction (to, from)](#apidoc.element.psd.Node.Root.aliasFunction)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>aliasProperty (to, from)](#apidoc.element.psd.Node.Root.aliasProperty)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>delegate ()](#apidoc.element.psd.Node.Root.delegate)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>extends (obj)](#apidoc.element.psd.Node.Root.extends)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>included (func)](#apidoc.element.psd.Node.Root.included)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>includes (obj)](#apidoc.element.psd.Node.Root.includes)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.</span>layerForPsd (psd)](#apidoc.element.psd.Node.Root.layerForPsd)
1.  object <span class="apidocSignatureSpan">psd.Node.Root.</span>PROPERTIES
1.  object <span class="apidocSignatureSpan">psd.Node.Root.</span>__super__

#### [module psd.Node.Root.prototype](#apidoc.module.psd.Node.Root.prototype)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>buildHeirarchy ()](#apidoc.element.psd.Node.Root.prototype.buildHeirarchy)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>constructor (psd)](#apidoc.element.psd.Node.Root.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>depth ()](#apidoc.element.psd.Node.Root.prototype.depth)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>documentDimensions ()](#apidoc.element.psd.Node.Root.prototype.documentDimensions)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>export ()](#apidoc.element.psd.Node.Root.prototype.export)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>fillOpacity ()](#apidoc.element.psd.Node.Root.prototype.fillOpacity)
1.  [function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>opacity ()](#apidoc.element.psd.Node.Root.prototype.opacity)
1.  string <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>type



# <a name="apidoc.module.psd"></a>[module psd](#apidoc.module.psd)

#### <a name="apidoc.element.psd.Node.Root"></a>[function <span class="apidocSignatureSpan">psd.</span>Node.Root (psd)](#apidoc.element.psd.Node.Root)
- description and source-code
```javascript
function Root(psd) {
  this.psd = psd;
  Root.__super__.constructor.call(this, Root.layerForPsd(this.psd));
  this.buildHeirarchy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.aliasFunction"></a>[function <span class="apidocSignatureSpan">psd.</span>aliasFunction (to, from)](#apidoc.element.psd.aliasFunction)
- description and source-code
```javascript
aliasFunction = function (to, from) {
  return this.prototype[to] = (function(_this) {
    return function() {
      var args;
      args = 1 <= arguments.length ? __slice.call(arguments, 0) : [];
      return _this.prototype[from].apply(_this, args);
    };
  })(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.aliasProperty"></a>[function <span class="apidocSignatureSpan">psd.</span>aliasProperty (to, from)](#apidoc.element.psd.aliasProperty)
- description and source-code
```javascript
aliasProperty = function (to, from) {
  return Object.defineProperty(this.prototype, to, {
    get: function() {
      return this[from];
    },
    set: function(val) {
      return this[from] = val;
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.delegate"></a>[function <span class="apidocSignatureSpan">psd.</span>delegate ()](#apidoc.element.psd.delegate)
- description and source-code
```javascript
delegate = function () {
  var args, source, target, _i, _len, _results;
  args = 1 <= arguments.length ? __slice.call(arguments, 0) : [];
  target = args.pop();
  _results = [];
  for (_i = 0, _len = args.length; _i < _len; _i++) {
    source = args[_i];
    _results.push(this.prototype[source] = target.prototype[source]);
  }
  return _results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.extends"></a>[function <span class="apidocSignatureSpan">psd.</span>extends (obj)](#apidoc.element.psd.extends)
- description and source-code
```javascript
extends = function (obj) {
  var key, value, _ref;
  for (key in obj) {
    value = obj[key];
    if (__indexOf.call(moduleKeywords, key) < 0) {
      this[key] = value;
    }
  }
  if ((_ref = obj.extended) != null) {
    _ref.call(this, this);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.fromFile"></a>[function <span class="apidocSignatureSpan">psd.</span>fromFile (file)](#apidoc.element.psd.fromFile)
- description and source-code
```javascript
fromFile = function (file) {
  return new PSD(fs.readFileSync(file));
}
```
- example usage
```shell
...

PSD.js works almost exactly the same in the browser and NodeJS.

### NodeJS Example

''' js
var PSD = require('psd');
var psd = PSD.fromFile("path/to/file.psd");
psd.parse();

console.log(psd.tree().export());
console.log(psd.tree().childrenAtPath('A/B/C')[0].export());

// You can also use promises syntax for opening and parsing
PSD.open("path/to/file.psd").then(function (psd) {
...
```

#### <a name="apidoc.element.psd.included"></a>[function <span class="apidocSignatureSpan">psd.</span>included (func)](#apidoc.element.psd.included)
- description and source-code
```javascript
included = function (func) {
  return func.call(this, this.prototype);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.includes"></a>[function <span class="apidocSignatureSpan">psd.</span>includes (obj)](#apidoc.element.psd.includes)
- description and source-code
```javascript
includes = function (obj) {
  var key, value, _ref;
  for (key in obj) {
    value = obj[key];
    if (__indexOf.call(moduleKeywords, key) < 0) {
      this.prototype[key] = value;
    }
  }
  if ((_ref = obj.included) != null) {
    _ref.call(this, this);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.open"></a>[function <span class="apidocSignatureSpan">psd.</span>open (file)](#apidoc.element.psd.open)
- description and source-code
```javascript
open = function (file) {
  return new RSVP.Promise(function(resolve, reject) {
    return fs.readFile(file, (function(_this) {
      return function(err, data) {
        var psd;
        if (err) {
          return reject(err);
        }
        psd = new PSD(data);
        psd.parse();
        return resolve(psd);
      };
    })(this));
  });
}
```
- example usage
```shell
...
var psd = PSD.fromFile("path/to/file.psd");
psd.parse();

console.log(psd.tree().export());
console.log(psd.tree().childrenAtPath('A/B/C')[0].export());

// You can also use promises syntax for opening and parsing
PSD.open("path/to/file.psd").then(function (psd) {
  return psd.image.saveAsPng('./output.png');
}).then(function () {
  console.log("Finished!");
});

'''
...
```



# <a name="apidoc.module.psd.Node"></a>[module psd.Node](#apidoc.module.psd.Node)

#### <a name="apidoc.element.psd.Node.Root"></a>[function <span class="apidocSignatureSpan">psd.Node.</span>Root (psd)](#apidoc.element.psd.Node.Root)
- description and source-code
```javascript
function Root(psd) {
  this.psd = psd;
  Root.__super__.constructor.call(this, Root.layerForPsd(this.psd));
  this.buildHeirarchy();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.psd.Node.Root"></a>[module psd.Node.Root](#apidoc.module.psd.Node.Root)

#### <a name="apidoc.element.psd.Node.Root.Root"></a>[function <span class="apidocSignatureSpan">psd.Node.</span>Root (psd)](#apidoc.element.psd.Node.Root.Root)
- description and source-code
```javascript
function Root(psd) {
  this.psd = psd;
  Root.__super__.constructor.call(this, Root.layerForPsd(this.psd));
  this.buildHeirarchy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.aliasFunction"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>aliasFunction (to, from)](#apidoc.element.psd.Node.Root.aliasFunction)
- description and source-code
```javascript
aliasFunction = function (to, from) {
  return this.prototype[to] = (function(_this) {
    return function() {
      var args;
      args = 1 <= arguments.length ? __slice.call(arguments, 0) : [];
      return _this.prototype[from].apply(_this, args);
    };
  })(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.aliasProperty"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>aliasProperty (to, from)](#apidoc.element.psd.Node.Root.aliasProperty)
- description and source-code
```javascript
aliasProperty = function (to, from) {
  return Object.defineProperty(this.prototype, to, {
    get: function() {
      return this[from];
    },
    set: function(val) {
      return this[from] = val;
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.delegate"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>delegate ()](#apidoc.element.psd.Node.Root.delegate)
- description and source-code
```javascript
delegate = function () {
  var args, source, target, _i, _len, _results;
  args = 1 <= arguments.length ? __slice.call(arguments, 0) : [];
  target = args.pop();
  _results = [];
  for (_i = 0, _len = args.length; _i < _len; _i++) {
    source = args[_i];
    _results.push(this.prototype[source] = target.prototype[source]);
  }
  return _results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.extends"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>extends (obj)](#apidoc.element.psd.Node.Root.extends)
- description and source-code
```javascript
extends = function (obj) {
  var key, value, _ref;
  for (key in obj) {
    value = obj[key];
    if (__indexOf.call(moduleKeywords, key) < 0) {
      this[key] = value;
    }
  }
  if ((_ref = obj.extended) != null) {
    _ref.call(this, this);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.included"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>included (func)](#apidoc.element.psd.Node.Root.included)
- description and source-code
```javascript
included = function (func) {
  return func.call(this, this.prototype);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.includes"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>includes (obj)](#apidoc.element.psd.Node.Root.includes)
- description and source-code
```javascript
includes = function (obj) {
  var key, value, _ref;
  for (key in obj) {
    value = obj[key];
    if (__indexOf.call(moduleKeywords, key) < 0) {
      this.prototype[key] = value;
    }
  }
  if ((_ref = obj.included) != null) {
    _ref.call(this, this);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.layerForPsd"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.</span>layerForPsd (psd)](#apidoc.element.psd.Node.Root.layerForPsd)
- description and source-code
```javascript
layerForPsd = function (psd) {
  var layer, prop, _i, _len, _ref;
  layer = {};
  _ref = Node.PROPERTIES;
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    prop = _ref[_i];
    layer[prop] = null;
  }
  layer.top = 0;
  layer.left = 0;
  layer.right = psd.header.width;
  layer.bottom = psd.header.height;
  return layer;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.psd.Node.Root.prototype"></a>[module psd.Node.Root.prototype](#apidoc.module.psd.Node.Root.prototype)

#### <a name="apidoc.element.psd.Node.Root.prototype.buildHeirarchy"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>buildHeirarchy ()](#apidoc.element.psd.Node.Root.prototype.buildHeirarchy)
- description and source-code
```javascript
buildHeirarchy = function () {
  var currentGroup, layer, parent, parseStack, _i, _len, _ref;
  currentGroup = this;
  parseStack = [];
  _ref = this.psd.layers;
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    layer = _ref[_i];
    if (layer.isFolder()) {
      parseStack.push(currentGroup);
      currentGroup = new Group(layer, _.last(parseStack));
    } else if (layer.isFolderEnd()) {
      parent = parseStack.pop();
      parent.children().push(currentGroup);
      currentGroup = parent;
    } else {
      currentGroup.children().push(new Layer(layer, currentGroup));
    }
  }
  return this.updateDimensions();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.prototype.constructor"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>constructor (psd)](#apidoc.element.psd.Node.Root.prototype.constructor)
- description and source-code
```javascript
function Root(psd) {
  this.psd = psd;
  Root.__super__.constructor.call(this, Root.layerForPsd(this.psd));
  this.buildHeirarchy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.prototype.depth"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>depth ()](#apidoc.element.psd.Node.Root.prototype.depth)
- description and source-code
```javascript
depth = function () {
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.prototype.documentDimensions"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>documentDimensions ()](#apidoc.element.psd.Node.Root.prototype.documentDimensions)
- description and source-code
```javascript
documentDimensions = function () {
  return [this.width, this.height];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.prototype.export"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>export ()](#apidoc.element.psd.Node.Root.prototype.export)
- description and source-code
```javascript
export = function () {
  var _ref;
  return {
    children: this._children.map(function(c) {
      return c["export"]();
    }),
    document: {
      width: this.width,
      height: this.height,
      resources: {
        layerComps: ((_ref = this.psd.resources.resource('layerComps')) != null ? _ref["export"]() : void 0) || [],
        guides: [],
        slices: []
      }
    }
  };
}
```
- example usage
```shell
...
### NodeJS Example

''' js
var PSD = require('psd');
var psd = PSD.fromFile("path/to/file.psd");
psd.parse();

console.log(psd.tree().export());
console.log(psd.tree().childrenAtPath('A/B/C')[0].export());

// You can also use promises syntax for opening and parsing
PSD.open("path/to/file.psd").then(function (psd) {
return psd.image.saveAsPng('./output.png');
}).then(function () {
console.log("Finished!");
...
```

#### <a name="apidoc.element.psd.Node.Root.prototype.fillOpacity"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>fillOpacity ()](#apidoc.element.psd.Node.Root.prototype.fillOpacity)
- description and source-code
```javascript
fillOpacity = function () {
  return 255;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.psd.Node.Root.prototype.opacity"></a>[function <span class="apidocSignatureSpan">psd.Node.Root.prototype.</span>opacity ()](#apidoc.element.psd.Node.Root.prototype.opacity)
- description and source-code
```javascript
opacity = function () {
  return 255;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
