# npmdoc-electron-builder

#### api documentation for  [electron-builder (v17.0.1)](https://github.com/electron-userland/electron-builder)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-builder)

#### A complete solution to package and build a ready for distribution Electron app for MacOS, Windows and Linux with “auto update” support out of the box

[![NPM](https://nodei.co/npm/electron-builder.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-builder)

- [https://npmdoc.github.io/node-npmdoc-electron-builder/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-builder/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-builder/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-builder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-electron-builder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-electron-builder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stefan Judis"
    },
    "bin": {
        "build": "./out/cli/build-cli.js",
        "install-app-deps": "./out/cli/install-app-deps.js",
        "node-gyp-rebuild": "./out/cli/node-gyp-rebuild.js"
    },
    "bugs": {
        "url": "https://github.com/electron-userland/electron-builder/issues"
    },
    "dependencies": {
        "7zip-bin": "^2.0.4",
        "ajv": "^5.0.4-beta.2",
        "ajv-keywords": "^2.0.1-beta.2",
        "bluebird-lst": "^1.0.2",
        "chalk": "^1.1.3",
        "chromium-pickle-js": "^0.2.0",
        "cuint": "^0.2.2",
        "electron-builder-core": "16.8.0",
        "electron-builder-http": "16.6.0",
        "electron-builder-util": "16.8.3",
        "electron-download-tf": "4.2.1",
        "electron-osx-sign": "0.4.4",
        "electron-publish": "16.8.3",
        "fs-extra-p": "^4.1.0",
        "hosted-git-info": "^2.4.2",
        "is-ci": "^1.0.10",
        "isbinaryfile": "^3.0.2",
        "js-yaml": "^3.8.3",
        "minimatch": "^3.0.3",
        "node-forge": "^0.7.1",
        "normalize-package-data": "^2.3.6",
        "parse-color": "^1.0.0",
        "plist": "^2.0.1",
        "sanitize-filename": "^1.6.1",
        "semver": "^5.3.0",
        "update-notifier": "^2.1.0",
        "uuid-1345": "^0.99.6",
        "yargs": "^7.1.0"
    },
    "description": "A complete solution to package and build a ready for distribution Electron app for MacOS, Windows and Linux with “auto update” support out of the box",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "2308ec32edc304aef5b0b21f93941577972fdfb2",
        "tarball": "https://registry.npmjs.org/electron-builder/-/electron-builder-17.0.1.tgz"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "files": [
        "out",
        "templates",
        "vendor",
        "scheme.json",
        "certs/root_certs.keychain"
    ],
    "homepage": "https://github.com/electron-userland/electron-builder",
    "keywords": [
        "electron",
        "builder",
        "build",
        "installer",
        "install",
        "packager",
        "pack",
        "nsis",
        "app",
        "dmg",
        "msi",
        "exe",
        "setup",
        "Windows",
        "OS X",
        "MacOS",
        "Mac",
        "appx"
    ],
    "license": "MIT",
    "main": "out/index.js",
    "maintainers": [
        {
            "name": "develar"
        },
        {
            "name": "stefanjudis"
        }
    ],
    "name": "electron-builder",
    "optionalDependencies": {},
    "publishConfig": {
        "tag": "next"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/electron-userland/electron-builder.git"
    },
    "scripts": {},
    "typings": "./out/electron-builder.d.ts",
    "version": "17.0.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
