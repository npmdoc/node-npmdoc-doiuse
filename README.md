# api documentation for  [doiuse (v2.6.0)](https://github.com/anandthakker/doiuse)  [![npm package](https://img.shields.io/npm/v/npmdoc-doiuse.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-doiuse) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-doiuse.svg)](https://travis-ci.org/npmdoc/node-npmdoc-doiuse)
#### Lint CSS for browser support against caniuse database.

[![NPM](https://nodei.co/npm/doiuse.png?downloads=true)](https://www.npmjs.com/package/doiuse)

[![apidoc](https://npmdoc.github.io/node-npmdoc-doiuse/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-doiuse_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-doiuse/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-doiuse/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-doiuse/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Anand Thakker"
    },
    "bin": {
        "doiuse": "./cli.js"
    },
    "bugs": {
        "url": "https://github.com/anandthakker/doiuse/issues"
    },
    "dependencies": {
        "browserslist": "^1.1.1",
        "caniuse-db": "^1.0.30000187",
        "css-rule-stream": "^1.1.0",
        "duplexer2": "0.0.2",
        "jsonfilter": "^1.1.2",
        "ldjson-stream": "^1.2.1",
        "lodash": "^4.0.0",
        "multimatch": "^2.0.0",
        "postcss": "^5.0.8",
        "source-map": "^0.4.2",
        "through2": "^0.6.3",
        "yargs": "^3.5.4"
    },
    "description": "Lint CSS for browser support against caniuse database.",
    "devDependencies": {
        "babel": "^5.2.13",
        "mock-fs": "^3.12.1",
        "postcss-import": "^7.1.3",
        "standard": "^8.1.0",
        "tape": "^4.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1892d10b61a9a356addbf2b614933e81f8bb3834",
        "tarball": "https://registry.npmjs.org/doiuse/-/doiuse-2.6.0.tgz"
    },
    "gitHead": "25175cf97974246a856892a17df4f672c94eabde",
    "homepage": "https://github.com/anandthakker/doiuse",
    "keywords": [
        "lint",
        "css",
        "browser",
        "support"
    ],
    "license": "MIT",
    "main": "lib/doiuse.js",
    "maintainers": [
        {
            "name": "anandthakker",
            "email": "vestibule@anandthakker.net"
        }
    ],
    "name": "doiuse",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/anandthakker/doiuse.git"
    },
    "scripts": {
        "babel": "babel -d lib/ src/",
        "prepublish": "npm run babel",
        "pretest": "npm run babel",
        "test": "standard && tape test/*.js"
    },
    "standard": {
        "ignore": [
            "data/*.js"
        ]
    },
    "version": "2.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module doiuse](#apidoc.module.doiuse)
1.  object <span class="apidocSignatureSpan">doiuse.</span>default
1.  object <span class="apidocSignatureSpan">doiuse.</span>util

#### [module doiuse.util](#apidoc.module.doiuse.util)
1.  [function <span class="apidocSignatureSpan">doiuse.util.</span>formatBrowserName (browserKey, versions)](#apidoc.element.doiuse.util.formatBrowserName)



# <a name="apidoc.module.doiuse"></a>[module doiuse](#apidoc.module.doiuse)



# <a name="apidoc.module.doiuse.util"></a>[module doiuse.util](#apidoc.module.doiuse.util)

#### <a name="apidoc.element.doiuse.util.formatBrowserName"></a>[function <span class="apidocSignatureSpan">doiuse.util.</span>formatBrowserName (browserKey, versions)](#apidoc.element.doiuse.util.formatBrowserName)
- description and source-code
```javascript
function formatBrowserName(browserKey, versions) {
  var browserName = (agents[browserKey] || {}).browser;
  if (!versions) {
    return browserName;
  }
  return browserName + ' (' + versions.join(',') + ')';
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
