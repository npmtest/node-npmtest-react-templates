# npmtest-react-templates

#### basic test coverage for  [react-templates (v0.6.1)](https://github.com/wix/react-templates)  [![npm package](https://img.shields.io/npm/v/npmtest-react-templates.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-templates) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-templates.svg)](https://travis-ci.org/npmtest/node-npmtest-react-templates)

#### Light weight templates for react -> write html get valid react code

[![NPM](https://nodei.co/npm/react-templates.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-templates)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-templates/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-templates/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-templates/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-templates/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-templates/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-templates/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-templates/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-templates/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-templates/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-templates/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-templates/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-templates/build/test-report.html](https://npmtest.github.io/node-npmtest-react-templates/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-templates/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-templates/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-templates/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-templates/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-templates/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-templates/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-templates/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-templates/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Avi Marcus"
    },
    "bin": {
        "rt": "./bin/rt.js"
    },
    "bugs": {
        "url": "https://github.com/wix/react-templates/issues"
    },
    "dependencies": {
        "chalk": "1.1.3",
        "cheerio": "0.22.0",
        "css": "2.2.1",
        "escodegen": "1.8.1",
        "esprima": "3.1.3",
        "glob": "7.1.1",
        "lodash": "4.17.4",
        "normalize-html-whitespace": "0.2.0",
        "optionator": "0.8.2",
        "text-table": "0.2.0"
    },
    "description": "Light weight templates for react -> write html get valid react code",
    "devDependencies": {
        "babel-cli": "6.18.0",
        "babel-core": "6.21.0",
        "babel-loader": "6.2.10",
        "babel-preset-es2015": "6.18.0",
        "brace": "0.9.1",
        "brfs": "1.4.3",
        "coveralls": "2.11.15",
        "eslint": "3.12.2",
        "eslint-config-wix-editor": "0.2.3",
        "eslint-plugin-lodash": "2.2.5",
        "eslint-plugin-react": "6.8.0",
        "eslint-plugin-wix-editor": "1.1.1",
        "grunt": "1.0.1",
        "grunt-babel": "6.0.0",
        "grunt-browserify": "5.0.0",
        "grunt-contrib-requirejs": "1.0.0",
        "grunt-contrib-uglify": "2.0.0",
        "grunt-contrib-watch": "1.0.0",
        "grunt-eslint": "19.0.0",
        "grunt-tape": "0.1.0",
        "istanbul": "0.4.5",
        "json-loader": "0.5.4",
        "react": "15.3.2",
        "react-dom": "15.3.2",
        "react-native": "0.39.2",
        "tape": "4.6.3",
        "webpack": "1.14.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a91bfb97cf85847ed5252d00623436e4135cc166",
        "tarball": "https://registry.npmjs.org/react-templates/-/react-templates-0.6.1.tgz"
    },
    "gitHead": "696aa2b4be448649361f8e27e7456c6c04dfa3df",
    "homepage": "https://github.com/wix/react-templates",
    "keywords": [
        "templates",
        "react-templates",
        "react",
        "reactjs",
        "react.js",
        "react-component",
        "react component"
    ],
    "license": "MIT",
    "main": "./dist/cli.js",
    "maintainers": [
        {
            "name": "danyshaanan"
        },
        {
            "name": "ganimomer"
        },
        {
            "name": "idok"
        }
    ],
    "name": "react-templates",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/wix/react-templates.git"
    },
    "scripts": {
        "all": "npm run lint && npm run test",
        "babel": "rm -rf dist && babel src/ --out-dir dist",
        "build": "npm run lint && npm run test",
        "buildwp": "webpack --config webpack-production.config.js --progress --profile --colors",
        "lint": "eslint .",
        "major": "npm version major -m\"update version to %s\" && git push && git push --tags",
        "minor": "npm version minor -m\"update version to %s\" && git push && git push --tags",
        "patch": "npm version patch -m\"update version to %s\" && git push && git push --tags",
        "prepublish": "npm run babel",
        "test": "babel-node test/src/test.js",
        "test-cov": "istanbul cover test/src/test.js -- --require test/support/env --reporter dot --check-leaks test/ test/acceptance/"
    },
    "version": "0.6.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
