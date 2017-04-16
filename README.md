# api documentation for  [electron-builder (v17.0.0)](https://github.com/electron-userland/electron-builder)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-builder)
#### A complete solution to package and build a ready for distribution Electron app for MacOS, Windows and Linux with “auto update” support out of the box

[![NPM](https://nodei.co/npm/electron-builder.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-builder)

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
        "shasum": "402ff5b8a31ab930d32c7a64fad73f27ea4da7f5",
        "tarball": "https://registry.npmjs.org/electron-builder/-/electron-builder-17.0.0.tgz"
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
    "version": "17.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module electron-builder](#apidoc.module.electron-builder)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>Packager (options, cancellationToken)](#apidoc.element.electron-builder.Packager)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>Platform (name, buildConfigurationKey, nodeName)](#apidoc.element.electron-builder.Platform)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>Target (name)](#apidoc.element.electron-builder.Target)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>archFromString (name)](#apidoc.element.electron-builder.archFromString)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>build (_x)](#apidoc.element.electron-builder.build)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>buildForge (appDir, options)](#apidoc.element.electron-builder.buildForge)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>createTargets (platforms, type, arch)](#apidoc.element.electron-builder.createTargets)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>getArchSuffix (arch)](#apidoc.element.electron-builder.getArchSuffix)
1.  object <span class="apidocSignatureSpan">electron-builder.</span>Arch
1.  object <span class="apidocSignatureSpan">electron-builder.</span>appInfo
1.  string <span class="apidocSignatureSpan">electron-builder.</span>DIR_TARGET

#### [module electron-builder.appInfo](#apidoc.module.electron-builder.appInfo)
1.  [function <span class="apidocSignatureSpan">electron-builder.appInfo.</span>AppInfo (metadata, info, buildVersion)](#apidoc.element.electron-builder.appInfo.AppInfo)



# <a name="apidoc.module.electron-builder"></a>[module electron-builder](#apidoc.module.electron-builder)

#### <a name="apidoc.element.electron-builder.Packager"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>Packager (options, cancellationToken)](#apidoc.element.electron-builder.Packager)
- description and source-code
```javascript
class Packager {
    //noinspection JSUnusedGlobalSymbols
    constructor(options, cancellationToken) {
        this.options = options;
        this.cancellationToken = cancellationToken;
        this.isTwoPackageJsonProjectLayoutUsed = true;
        this.eventEmitter = new (_events || _load_events()).EventEmitter();
        this.tempDirManager = new (_tmp || _load_tmp()).TmpDir();
        this._repositoryInfo = new (_electronBuilderUtil || _load_electronBuilderUtil()).Lazy(() => (0, (_repositoryInfo || _load_repositoryInfo
()).getRepositoryInfo)(this.projectDir, this.metadata, this.devMetadata));
        this.afterPackHandlers = [];
        this.projectDir = options.projectDir == null ? process.cwd() : _path.resolve(options.projectDir);
        this.prepackaged = options.prepackaged == null ? null : _path.resolve(this.projectDir, options.prepackaged);
    }
    get isPrepackedAppAsar() {
        return this._isPrepackedAppAsar;
    }
    get config() {
        return this._config;
    }
    get repositoryInfo() {
        return this._repositoryInfo.value;
    }
    addAfterPackHandler(handler) {
        this.afterPackHandlers.push(handler);
    }
    artifactCreated(handler) {
        addHandler(this.eventEmitter, "artifactCreated", handler);
        return this;
    }
    dispatchArtifactCreated(event) {
        this.eventEmitter.emit("artifactCreated", event);
    }
    build() {
        var _this = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            //noinspection JSDeprecatedSymbols
            const devMetadataFromOptions = _this.options.devMetadata;
            if (devMetadataFromOptions != null) {
                (0, (_log || _load_log()).warn)("devMetadata is deprecated, please use config instead");
            }
            let configPath = null;
            let configFromOptions = _this.options.config;
            if (typeof configFromOptions === "string") {
                // it is a path to config file
                configPath = configFromOptions;
                configFromOptions = null;
            }
            if (devMetadataFromOptions != null) {
                if (configFromOptions != null) {
                    throw new Error("devMetadata and config cannot be used in conjunction");
                }
                configFromOptions = devMetadataFromOptions.build;
            }
            const projectDir = _this.projectDir;
            const fileOrPackageConfig = yield configPath == null ? (0, (_readPackageJson || _load_readPackageJson()).loadConfig)(
projectDir) : (0, (_readPackageJson || _load_readPackageJson()).doLoadConfig)(_path.resolve(projectDir, configPath), projectDir);
            const config = (0, (_deepAssign || _load_deepAssign()).deepAssign)({}, fileOrPackageConfig, configFromOptions);
            const extraMetadata = _this.options.extraMetadata;
            if (extraMetadata != null) {
                const extraBuildMetadata = extraMetadata.build;
                if (extraBuildMetadata != null) {
                    (0, (_deepAssign || _load_deepAssign()).deepAssign)(config, extraBuildMetadata);
                    delete extraMetadata.build;
                }
                if (extraMetadata.directories != null) {
                    (0, (_log || _load_log()).warn)('--em.directories is deprecated, please specify as --em.build.directories"');
                    (0, (_deepAssign || _load_deepAssign()).deepAssign)(config, { directories: extraMetadata.directories });
                    delete extraMetadata.directories;
                }
            }
            yield (0, (_readPackageJson || _load_readPackageJson()).validateConfig)(config);
            _this._config = config;
            _this.appDir = yield (0, (_electronBuilderUtil || _load_electronBuilderUtil()).computeDefaultAppDirectory)(projectDir
, (0, (_electronBuilderUtil || _load_electronBuilderUtil()).use)(config.directories, function (it) {
                return it.app;
            }));
            _this.isTwoPackageJsonProjectLayoutUsed = _this.appDir !== projectD ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.Platform"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>Platform (name, buildConfigurationKey, nodeName)](#apidoc.element.electron-builder.Platform)
- description and source-code
```javascript
class Platform {
    constructor(name, buildConfigurationKey, nodeName) {
        this.name = name;
        this.buildConfigurationKey = buildConfigurationKey;
        this.nodeName = nodeName;
    }
    toString() {
        return this.name;
    }
    createTarget(type) {
        for (var _len = arguments.length, archs = Array(_len > 1 ? _len - 1 : 0), _key = 1; _key < _len; _key++) {
            archs[_key - 1] = arguments[_key];
        }

        if (type == null && (archs == null || archs.length === 0)) {
            return new Map([[this, new Map()]]);
        }
        const archToType = new Map();
        if (this === Platform.MAC) {
            archs = [Arch.x64];
        }
        for (const arch of archs == null || archs.length === 0 ? [archFromString(process.arch)] : archs) {
            archToType.set(arch, type == null ? [] : Array.isArray(type) ? type : [type]);
        }
        return new Map([[this, archToType]]);
    }
    static current() {
        return Platform.fromString(process.platform);
    }
    static fromString(name) {
        name = name.toLowerCase();
        switch (name) {
            case Platform.MAC.nodeName:
            case Platform.MAC.name:
                return Platform.MAC;
            case Platform.WINDOWS.nodeName:
            case Platform.WINDOWS.name:
            case Platform.WINDOWS.buildConfigurationKey:
                return Platform.WINDOWS;
            case Platform.LINUX.nodeName:
                return Platform.LINUX;
            default:
                throw new Error('Unknown platform: ${name}');
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.Target"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>Target (name)](#apidoc.element.electron-builder.Target)
- description and source-code
```javascript
class Target {
    constructor(name) {
        let isAsyncSupported = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : true;

        this.name = name;
        this.isAsyncSupported = isAsyncSupported;
    }
    finishBuild() {
        return Promise.resolve();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.archFromString"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>archFromString (name)](#apidoc.element.electron-builder.archFromString)
- description and source-code
```javascript
function archFromString(name) {
    if (name === "x64") {
        return Arch.x64;
    }
    if (name === "ia32") {
        return Arch.ia32;
    }
    if (name === "armv7l") {
        return Arch.armv7l;
    }
    throw new Error('Unsupported arch ${name}');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.build"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>build (_x)](#apidoc.element.electron-builder.build)
- description and source-code
```javascript
function build(_x) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
...
'''js
"use strict"

const builder = require("electron-builder")
const Platform = builder.Platform

// Promise is returned
builder.build({
targets: Platform.MAC.createTarget(),
config: {
 "//": "build options, see https://goo.gl/ZhRfla"
}
})
.then(() => {
  // handle result
...
```

#### <a name="apidoc.element.electron-builder.buildForge"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>buildForge (appDir, options)](#apidoc.element.electron-builder.buildForge)
- description and source-code
```javascript
function buildForge(appDir, options) {
    return (0, (_builder || _load_builder()).build)(Object.assign({
        prepackaged: appDir,
        config: {
            directories: {
                // https://github.com/electron-userland/electron-forge/blob/master/src/makers/generic/zip.js
                output: _path.resolve(appDir, "..", "make")
            }
        }
    }, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.createTargets"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>createTargets (platforms, type, arch)](#apidoc.element.electron-builder.createTargets)
- description and source-code
```javascript
function createTargets(platforms, type, arch) {
    const targets = new Map();
    for (const platform of platforms) {
        const archs = platform === (_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC ? [(_electronBuilderCore ||
_load_electronBuilderCore()).Arch.x64] : arch === "all" ? [(_electronBuilderCore || _load_electronBuilderCore()).Arch.x64, (_electronBuilderCore
 || _load_electronBuilderCore()).Arch.ia32] : [(0, (_electronBuilderCore || _load_electronBuilderCore()).archFromString)(arch ==
null ? process.arch : arch)];
        const archToType = new Map();
        targets.set(platform, archToType);
        for (const arch of archs) {
            archToType.set(arch, type == null ? [] : [type]);
        }
    }
    return targets;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.getArchSuffix"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>getArchSuffix (arch)](#apidoc.element.electron-builder.getArchSuffix)
- description and source-code
```javascript
function getArchSuffix(arch) {
    return arch === Arch.x64 ? "" : '-${Arch[arch]}';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.appInfo"></a>[module electron-builder.appInfo](#apidoc.module.electron-builder.appInfo)

#### <a name="apidoc.element.electron-builder.appInfo.AppInfo"></a>[function <span class="apidocSignatureSpan">electron-builder.appInfo.</span>AppInfo (metadata, info, buildVersion)](#apidoc.element.electron-builder.appInfo.AppInfo)
- description and source-code
```javascript
class AppInfo {
    constructor(metadata, info, buildVersion) {
        this.metadata = metadata;
        this.info = info;
        this.description = (0, (_electronBuilderUtil || _load_electronBuilderUtil()).smarten)(this.metadata.description || "");
        this.version = metadata.version;
        this.buildNumber = this.config.buildVersion || process.env.TRAVIS_BUILD_NUMBER || process.env.APPVEYOR_BUILD_NUMBER || process
.env.CIRCLE_BUILD_NUM || process.env.BUILD_NUMBER;
        if ((0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(buildVersion)) {
            buildVersion = this.version;
            if (!(0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(this.buildNumber)) {
                buildVersion += '.${this.buildNumber}';
            }
            this.buildVersion = buildVersion;
        } else {
            this.buildVersion = buildVersion;
        }
        this.productName = this.config.productName || metadata.productName || metadata.name;
        this.productFilename = (0, (_sanitizeFilename || _load_sanitizeFilename()).default)(this.productName);
    }
    get config() {
        return this.info.config;
    }
    get versionInWeirdWindowsForm() {
        const parsedVersion = new (_semver || _load_semver()).SemVer(this.version);
        return '${parsedVersion.major}.${parsedVersion.minor}.${parsedVersion.patch}.${this.buildNumber || "0"}';
    }
    get companyName() {
        return this.metadata.author.name;
    }
    get id() {
        let appId;
        if (this.config.appId != null) {
            appId = this.config.appId;
        }
        const generateDefaultAppId = () => {
            return 'com.electron.${this.metadata.name.toLowerCase()}';
        };
        if (appId != null && (appId === "your.id" || (0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(
appId))) {
            const incorrectAppId = appId;
            appId = generateDefaultAppId();
            (0, (_log || _load_log()).warn)('Do not use "${incorrectAppId}" as appId, "${appId}" will be used instead');
        }
        return appId == null ? generateDefaultAppId() : appId;
    }
    get name() {
        return this.metadata.name;
    }
    get copyright() {
        const copyright = this.config.copyright;
        if (copyright != null) {
            return copyright;
        }
        return 'Copyright © ${new Date().getFullYear()} ${this.metadata.author.name || this.productName}';
    }
    computePackageUrl() {
        var _this = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            const url = _this.metadata.homepage;
            if (url != null) {
                return url;
            }
            const info = yield _this.info.repositoryInfo;
            return info == null || info.type !== "github" ? null : 'https://${info.domain}/${info.user}/${info.project}';
        })();
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
