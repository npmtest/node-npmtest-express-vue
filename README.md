# npmtest-express-vue

#### basic test coverage for  [express-vue (v3.9.11)](https://github.com/express-vue/express-vue)  [![npm package](https://img.shields.io/npm/v/npmtest-express-vue.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-express-vue) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-express-vue.svg)](https://travis-ci.org/npmtest/node-npmtest-express-vue)

#### Vue rendering engine for Express.js

[![NPM](https://nodei.co/npm/express-vue.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/express-vue)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-express-vue/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-express-vue/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-express-vue/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-express-vue/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-express-vue/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-express-vue/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-express-vue/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-express-vue/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-express-vue/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-express-vue/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-express-vue/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-express-vue/build/test-report.html](https://npmtest.github.io/node-npmtest-express-vue/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-express-vue/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-express-vue/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-express-vue/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-express-vue/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-vue/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-vue/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-express-vue/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-express-vue/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Daniel Cherubini",
        "url": "https://cherubini.casa"
    },
    "ava": {
        "files": [
            "test/*.js"
        ],
        "source": [
            "lib/**/*.js",
            "!dist/**/*"
        ],
        "concurrency": 5,
        "failFast": false,
        "powerAssert": false,
        "require": [
            "babel-register"
        ],
        "babel": "inherit"
    },
    "bugs": {
        "url": "https://github.com/express-vue/express-vue/issues"
    },
    "dependencies": {
        "babel-core": "^6.18.0",
        "babel-preset-es2015": "^6.9.0",
        "html-minifier": "^3.2.3",
        "param-case": "^2.1.0",
        "pug": "^2.0.0-beta11",
        "require-from-string": "^1.2.1",
        "vue": "^2.2.6",
        "vue-server-renderer": "^2.2.6",
        "xss": "^0.3.1"
    },
    "description": "Vue rendering engine for Express.js",
    "devDependencies": {
        "ava": "^0.18.2",
        "babel-eslint": "^7.1.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-flow-strip-types": "^6.22.0",
        "babel-register": "^6.18.0",
        "coveralls": "^2.12.0",
        "del": "^2.2.2",
        "eslint": "^3.11.0",
        "eslint-config-xo-space": "^0.16.0",
        "eslint-plugin-babel": "^4.0.0",
        "express": "^4.14.0",
        "flow-bin": "^0.42.0",
        "gulp": "^3.9.1",
        "gulp-ava": "^0.16.0",
        "gulp-babel": "^6.1.2",
        "gulp-concat": "^2.6.1",
        "gulp-eslint": "^3.0.1",
        "gulp-exclude-gitignore": "^1.1.1",
        "gulp-line-ending-corrector": "^1.0.1",
        "gulp-nsp": "^2.4.2",
        "nyc": "^10.1.2"
    },
    "directories": {},
    "dist": {
        "shasum": "412d98a3b1cdee8e766d875c4b3a987bad045c0e",
        "tarball": "https://registry.npmjs.org/express-vue/-/express-vue-3.9.11.tgz"
    },
    "engines": {
        "node": ">=6.0.0"
    },
    "eslintConfig": {
        "extends": "xo-space",
        "env": {
            "mocha": true
        }
    },
    "files": [
        "dist"
    ],
    "gitHead": "24fdc965691c51fc998ff2fc9bb4250ff5701e5d",
    "homepage": "https://github.com/express-vue/express-vue",
    "keywords": [
        "vue",
        "express",
        "node"
    ],
    "license": "Apache-2.0",
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "danmademe"
        }
    ],
    "name": "express-vue",
    "nyc": {
        "include": [
            "lib/**/*.js"
        ]
    },
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/express-vue/express-vue.git"
    },
    "scripts": {
        "coverage": "nyc report --reporter=text-lcov | coveralls",
        "postversion": "git push && git push --tags",
        "prepublish": "gulp build",
        "preversion": "npm test",
        "test": "gulp test",
        "version": "gulp build && git add -A"
    },
    "typings": "dist/index.d.ts",
    "version": "3.9.11",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
