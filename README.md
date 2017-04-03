# api documentation for  [electron-builder (v16.6.1)](https://github.com/electron-userland/electron-builder)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-builder)
#### A complete solution to package and build a ready for distribution Electron app for MacOS, Windows and Linux with “auto update” support out of the box

[![NPM](https://nodei.co/npm/electron-builder.png?downloads=true)](https://www.npmjs.com/package/electron-builder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-builder/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-electron-builder_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-builder/build..beta..travis-ci.org/apidoc.html)

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
        "electron-builder-core": "16.6.0",
        "electron-builder-http": "16.6.0",
        "electron-builder-util": "16.6.0",
        "electron-download-tf": "4.1.1",
        "electron-macos-sign": "~1.6.0",
        "electron-publish": "16.6.0",
        "fs-extra-p": "^4.1.0",
        "hosted-git-info": "^2.4.1",
        "is-ci": "^1.0.10",
        "isbinaryfile": "^3.0.2",
        "js-yaml": "^3.8.2",
        "minimatch": "^3.0.3",
        "node-forge": "^0.7.1",
        "normalize-package-data": "^2.3.6",
        "parse-color": "^1.0.0",
        "plist": "^2.0.1",
        "sanitize-filename": "^1.6.1",
        "semver": "^5.3.0",
        "update-notifier": "^2.1.0",
        "uuid-1345": "^0.99.6",
        "yargs": "^7.0.2"
    },
    "description": "A complete solution to package and build a ready for distribution Electron app for MacOS, Windows and Linux with “auto update” support out of the box",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "d1605809c0662998cff5c25602bd8811a3ae4e5c",
        "tarball": "https://registry.npmjs.org/electron-builder/-/electron-builder-16.6.1.tgz"
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
            "name": "develar",
            "email": "develar@gmail.com"
        },
        {
            "name": "stefanjudis",
            "email": "stefanjudis@gmail.com"
        }
    ],
    "name": "electron-builder",
    "optionalDependencies": {},
    "publishConfig": {
        "tag": "next"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/electron-userland/electron-builder.git"
    },
    "scripts": {},
    "typings": "./out/electron-builder.d.ts",
    "version": "16.6.1"
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
1.  object <span class="apidocSignatureSpan">electron-builder.</span>asar
1.  object <span class="apidocSignatureSpan">electron-builder.</span>asarUtil
1.  object <span class="apidocSignatureSpan">electron-builder.</span>builder
1.  object <span class="apidocSignatureSpan">electron-builder.</span>codeSign
1.  object <span class="apidocSignatureSpan">electron-builder.</span>fileMatcher
1.  object <span class="apidocSignatureSpan">electron-builder.</span>fileTransformer
1.  object <span class="apidocSignatureSpan">electron-builder.</span>linuxPackager
1.  object <span class="apidocSignatureSpan">electron-builder.</span>macPackager
1.  object <span class="apidocSignatureSpan">electron-builder.</span>packager
1.  object <span class="apidocSignatureSpan">electron-builder.</span>platformPackager
1.  object <span class="apidocSignatureSpan">electron-builder.</span>readInstalled
1.  object <span class="apidocSignatureSpan">electron-builder.</span>repositoryInfo
1.  object <span class="apidocSignatureSpan">electron-builder.</span>winPackager
1.  object <span class="apidocSignatureSpan">electron-builder.</span>windowsCodeSign
1.  object <span class="apidocSignatureSpan">electron-builder.</span>yarn
1.  string <span class="apidocSignatureSpan">electron-builder.</span>DIR_TARGET

#### [module electron-builder.appInfo](#apidoc.module.electron-builder.appInfo)
1.  [function <span class="apidocSignatureSpan">electron-builder.appInfo.</span>AppInfo (metadata, info, buildVersion)](#apidoc.element.electron-builder.appInfo.AppInfo)

#### [module electron-builder.asar](#apidoc.module.electron-builder.asar)
1.  [function <span class="apidocSignatureSpan">electron-builder.asar.</span>AsarFilesystem (src)](#apidoc.element.electron-builder.asar.AsarFilesystem)
1.  [function <span class="apidocSignatureSpan">electron-builder.asar.</span>Node {{signature}}](#apidoc.element.electron-builder.asar.Node)
1.  [function <span class="apidocSignatureSpan">electron-builder.asar.</span>readAsar (_x5)](#apidoc.element.electron-builder.asar.readAsar)
1.  [function <span class="apidocSignatureSpan">electron-builder.asar.</span>readAsarJson (_x6, _x7)](#apidoc.element.electron-builder.asar.readAsarJson)

#### [module electron-builder.asarUtil](#apidoc.module.electron-builder.asarUtil)
1.  [function <span class="apidocSignatureSpan">electron-builder.asarUtil.</span>AsarPackager (src, destination, options, unpackPattern, transformer)](#apidoc.element.electron-builder.asarUtil.AsarPackager)
1.  [function <span class="apidocSignatureSpan">electron-builder.asarUtil.</span>checkFileInArchive (_x2, _x3, _x4)](#apidoc.element.electron-builder.asarUtil.checkFileInArchive)

#### [module electron-builder.builder](#apidoc.module.electron-builder.builder)
1.  [function <span class="apidocSignatureSpan">electron-builder.builder.</span>build (_x)](#apidoc.element.electron-builder.builder.build)
1.  [function <span class="apidocSignatureSpan">electron-builder.builder.</span>createTargets (platforms, type, arch)](#apidoc.element.electron-builder.builder.createTargets)
1.  [function <span class="apidocSignatureSpan">electron-builder.builder.</span>normalizeOptions (args)](#apidoc.element.electron-builder.builder.normalizeOptions)

#### [module electron-builder.codeSign](#apidoc.module.electron-builder.codeSign)
1.  [function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>createKeychain (_x3, _x4, _x5, _x6, _x7)](#apidoc.element.electron-builder.codeSign.createKeychain)
1.  [function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>downloadCertificate (_x, _x2)](#apidoc.element.electron-builder.codeSign.downloadCertificate)
1.  [function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>findIdentity (certType, qualifier, keychain)](#apidoc.element.electron-builder.codeSign.findIdentity)
1.  [function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>sign (path, name, keychain)](#apidoc.element.electron-builder.codeSign.sign)
1.  object <span class="apidocSignatureSpan">electron-builder.codeSign.</span>appleCertificatePrefixes
1.  object <span class="apidocSignatureSpan">electron-builder.codeSign.</span>findIdentityRawResult

#### [module electron-builder.fileMatcher](#apidoc.module.electron-builder.fileMatcher)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>FileMatcher (from, to, macroExpander, patterns)](#apidoc.element.electron-builder.fileMatcher.FileMatcher)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>copyFiles (patterns)](#apidoc.element.electron-builder.fileMatcher.copyFiles)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>createFileMatcher (info, appDir, resourcesPath, macroExpander, platformSpecificBuildOptions)](#apidoc.element.electron-builder.fileMatcher.createFileMatcher)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>getFileMatchers (config, name, defaultSrc, defaultDest, allowAdvancedMatching, macroExpander, customBuildOptions)](#apidoc.element.electron-builder.fileMatcher.getFileMatchers)

#### [module electron-builder.fileTransformer](#apidoc.module.electron-builder.fileTransformer)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileTransformer.</span>createElectronCompilerHost (projectDir, cacheDir)](#apidoc.element.electron-builder.fileTransformer.createElectronCompilerHost)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileTransformer.</span>createTransformer (_x, _x2)](#apidoc.element.electron-builder.fileTransformer.createTransformer)
1.  [function <span class="apidocSignatureSpan">electron-builder.fileTransformer.</span>isElectronCompileUsed (info)](#apidoc.element.electron-builder.fileTransformer.isElectronCompileUsed)

#### [module electron-builder.linuxPackager](#apidoc.module.electron-builder.linuxPackager)
1.  [function <span class="apidocSignatureSpan">electron-builder.linuxPackager.</span>LinuxPackager (_platformPackager || _load_platformPackager()](#apidoc.element.electron-builder.linuxPackager.LinuxPackager)

#### [module electron-builder.macPackager](#apidoc.module.electron-builder.macPackager)
1.  [function <span class="apidocSignatureSpan">electron-builder.macPackager.</span>default (_platformPackager || _load_platformPackager()](#apidoc.element.electron-builder.macPackager.default)

#### [module electron-builder.packager](#apidoc.module.electron-builder.packager)
1.  [function <span class="apidocSignatureSpan">electron-builder.packager.</span>Packager (options, cancellationToken)](#apidoc.element.electron-builder.packager.Packager)
1.  [function <span class="apidocSignatureSpan">electron-builder.packager.</span>checkWineVersion (_x)](#apidoc.element.electron-builder.packager.checkWineVersion)
1.  [function <span class="apidocSignatureSpan">electron-builder.packager.</span>normalizePlatforms (rawPlatforms)](#apidoc.element.electron-builder.packager.normalizePlatforms)

#### [module electron-builder.platformPackager](#apidoc.module.electron-builder.platformPackager)
1.  [function <span class="apidocSignatureSpan">electron-builder.platformPackager.</span>PlatformPackager (info)](#apidoc.element.electron-builder.platformPackager.PlatformPackager)
1.  [function <span class="apidocSignatureSpan">electron-builder.platformPackager.</span>normalizeExt (ext)](#apidoc.element.electron-builder.platformPackager.normalizeExt)

#### [module electron-builder.readInstalled](#apidoc.module.electron-builder.readInstalled)
1.  [function <span class="apidocSignatureSpan">electron-builder.</span>readInstalled (_x)](#apidoc.element.electron-builder.readInstalled.readInstalled)

#### [module electron-builder.repositoryInfo](#apidoc.module.electron-builder.repositoryInfo)
1.  [function <span class="apidocSignatureSpan">electron-builder.repositoryInfo.</span>getRepositoryInfo (projectDir, metadata, devMetadata)](#apidoc.element.electron-builder.repositoryInfo.getRepositoryInfo)

#### [module electron-builder.winPackager](#apidoc.module.electron-builder.winPackager)
1.  [function <span class="apidocSignatureSpan">electron-builder.winPackager.</span>WinPackager (_platformPackager || _load_platformPackager()](#apidoc.element.electron-builder.winPackager.WinPackager)

#### [module electron-builder.windowsCodeSign](#apidoc.module.electron-builder.windowsCodeSign)
1.  [function <span class="apidocSignatureSpan">electron-builder.windowsCodeSign.</span>getSignVendorPath ()](#apidoc.element.electron-builder.windowsCodeSign.getSignVendorPath)
1.  [function <span class="apidocSignatureSpan">electron-builder.windowsCodeSign.</span>getToolPath ()](#apidoc.element.electron-builder.windowsCodeSign.getToolPath)
1.  [function <span class="apidocSignatureSpan">electron-builder.windowsCodeSign.</span>sign (_x)](#apidoc.element.electron-builder.windowsCodeSign.sign)

#### [module electron-builder.yarn](#apidoc.module.electron-builder.yarn)
1.  [function <span class="apidocSignatureSpan">electron-builder.yarn.</span>getGypEnv (electronVersion, platform, arch, buildFromSource)](#apidoc.element.electron-builder.yarn.getGypEnv)
1.  [function <span class="apidocSignatureSpan">electron-builder.yarn.</span>installOrRebuild (_x, _x2, _x3, _x4, _x5)](#apidoc.element.electron-builder.yarn.installOrRebuild)
1.  [function <span class="apidocSignatureSpan">electron-builder.yarn.</span>rebuild (_x9, _x10)](#apidoc.element.electron-builder.yarn.rebuild)



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
...
if (options.draft === undefined && !(0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(process.env.EP_DRAFT
)) {
    options.draft = process.env.EP_DRAFT.toLowerCase() === "true";
}
if (options.prerelease === undefined && !(0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(process.env.
EP_PRELEASE)) {
    options.prerelease = process.env.EP_PRELEASE.toLowerCase() === "true";
}
const cancellationToken = new (_CancellationToken || _load_CancellationToken()).CancellationToken();
const packager = new (_packager || _load_packager()).Packager(options, cancellationToken);
// because artifact event maybe dispatched several times for different publish providers
const artifactPaths = new Set();
packager.artifactCreated(function (event) {
    if (event.file != null) {
        artifactPaths.add(event.file);
    }
});
...
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
...
    this.codeSigningInfo = (0, (_codeSign || _load_codeSign()).createKeychain)(info.tempDirManager, this.packagerOptions.cscLink
, this.getCscPassword(), this.packagerOptions.cscInstallerLink, this.packagerOptions.cscInstallerKeyPassword);
}
    }
    get defaultTarget() {
return ["zip", "dmg"];
    }
    prepareAppInfo(appInfo) {
return new (_appInfo || _load_appInfo()).AppInfo(appInfo.metadata, this.info, this.platformSpecificBuildOptions.bundleVersion);
    }
    getIconPath() {
var _this = this;

return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
    let iconPath = _this.platformSpecificBuildOptions.icon || _this.config.icon;
    if (iconPath != null && !iconPath.endsWith(".icns")) {
...
```



# <a name="apidoc.module.electron-builder.asar"></a>[module electron-builder.asar](#apidoc.module.electron-builder.asar)

#### <a name="apidoc.element.electron-builder.asar.AsarFilesystem"></a>[function <span class="apidocSignatureSpan">electron-builder.asar.</span>AsarFilesystem (src)](#apidoc.element.electron-builder.asar.AsarFilesystem)
- description and source-code
```javascript
class AsarFilesystem {
    constructor(src) {
        let header = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : new Node();
        let headerSize = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : -1;

        this.src = src;
        this.header = header;
        this.headerSize = headerSize;
        this.offset = UINT64(0);
        if (this.header.files == null) {
            this.header.files = {};
        }
    }
    searchNodeFromDirectory(p) {
        let node = this.header;
        for (const dir of p.split(_path.sep)) {
            if (dir !== ".") {
                node = node.files[dir];
            }
        }
        return node;
    }
    getOrCreateNode(p) {
        p = _path.relative(this.src, p);
        if (p == null || p.length === 0) {
            return this.header;
        }
        const name = _path.basename(p);
        const dirNode = this.searchNodeFromDirectory(_path.dirname(p));
        if (dirNode.files == null) {
            dirNode.files = {};
        }
        let result = dirNode.files[name];
        if (result == null) {
            result = new Node();
            dirNode.files[name] = result;
        }
        return result;
    }
    insertDirectory(p) {
        let unpacked = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : false;

        const node = this.getOrCreateNode(p);
        node.files = {};
        if (unpacked) {
            node.unpacked = unpacked;
        }
        return node.files;
    }
    insertFileNode(node, stat, file) {
        if (node.size > 4294967295) {
            throw new Error('${file}: file size can not be larger than 4.2GB');
        }
        node.offset = this.offset.toString();
        if (process.platform !== "win32" && stat.mode & 0o100) {
            node.executable = true;
        }
        this.offset.add(UINT64(node.size));
    }
    getNode(p) {
        const node = this.searchNodeFromDirectory(_path.dirname(p));
        return node.files[_path.basename(p)];
    }
    getFile(p) {
        let followLinks = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : true;

        const info = this.getNode(p);
        // if followLinks is false we don't resolve symlinks
        return followLinks && info.link != null ? this.getFile(info.link) : info;
    }
    readJson(file) {
        var _this = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            return JSON.parse((yield _this.readFile(file)).toString());
        })();
    }
    readFile(file) {
        var _this2 = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            return yield readFileFromAsar(_this2, file, _this2.getFile(file));
        })();
    }
}
```
- example usage
```shell
...
}
class AsarPackager {
constructor(src, destination, options, unpackPattern, transformer) {
    this.src = src;
    this.options = options;
    this.unpackPattern = unpackPattern;
    this.transformer = transformer;
    this.fs = new (_asar || _load_asar()).AsarFilesystem(this.src);
    this.metadata = new Map();
    this.outFile = _path.join(destination, "app.asar");
}
// sort files to minimize file change (i.e. asar file is not changed dramatically on small change)
pack(filter, isElectronCompile) {
    var _this = this;
...
```

#### <a name="apidoc.element.electron-builder.asar.Node"></a>[function <span class="apidocSignatureSpan">electron-builder.asar.</span>Node {{signature}}](#apidoc.element.electron-builder.asar.Node)
- description and source-code
```javascript
class Node {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.asar.readAsar"></a>[function <span class="apidocSignatureSpan">electron-builder.asar.</span>readAsar (_x5)](#apidoc.element.electron-builder.asar.readAsar)
- description and source-code
```javascript
function readAsar(_x5) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.asar.readAsarJson"></a>[function <span class="apidocSignatureSpan">electron-builder.asar.</span>readAsarJson (_x6, _x7)](#apidoc.element.electron-builder.asar.readAsarJson)
- description and source-code
```javascript
function readAsarJson(_x6, _x7) {
    return _ref2.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.asarUtil"></a>[module electron-builder.asarUtil](#apidoc.module.electron-builder.asarUtil)

#### <a name="apidoc.element.electron-builder.asarUtil.AsarPackager"></a>[function <span class="apidocSignatureSpan">electron-builder.asarUtil.</span>AsarPackager (src, destination, options, unpackPattern, transformer)](#apidoc.element.electron-builder.asarUtil.AsarPackager)
- description and source-code
```javascript
class AsarPackager {
    constructor(src, destination, options, unpackPattern, transformer) {
        this.src = src;
        this.options = options;
        this.unpackPattern = unpackPattern;
        this.transformer = transformer;
        this.fs = new (_asar || _load_asar()).AsarFilesystem(this.src);
        this.metadata = new Map();
        this.outFile = _path.join(destination, "app.asar");
    }
    // sort files to minimize file change (i.e. asar file is not changed dramatically on small change)
    pack(filter, isElectronCompile) {
        var _this = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            const metadata = _this.metadata;
            let files = yield (0, (_fs || _load_fs()).walk)(_this.src, filter, function (file, fileStat) {
                metadata.set(file, fileStat);
                if (fileStat.isSymbolicLink()) {
                    return (0, (_fsExtraP || _load_fsExtraP()).readlink)(file).then(function (linkTarget) {
                        // http://unix.stackexchange.com/questions/105637/is-symlinks-target-relative-to-the-destinations-parent
-directory-and-if-so-wh
                        const resolved = _path.resolve(_path.dirname(file), linkTarget);
                        const link = _path.relative(_this.src, linkTarget);
                        if (link.startsWith("..")) {
                            // outside of project, linked module (https://github.com/electron-userland/electron-builder/issues/675
)
                            return (0, (_fsExtraP || _load_fsExtraP()).stat)(resolved).then(function (targetFileStat) {
                                metadata.set(file, targetFileStat);
                                return targetFileStat;
                            });
                        } else {
                            fileStat.relativeLink = link;
                        }
                        return null;
                    });
                }
                return null;
            });
            // transform before electron-compile to avoid filtering (cache files in any case should be not transformed)
            const transformer = _this.transformer;
            _this.transformedFiles = yield (_bluebirdLst2 || _load_bluebirdLst2()).default.map(files, function (it) {
                return metadata.get(it).isFile() ? transformer(it) : null;
            }, (_fs || _load_fs()).CONCURRENCY);
            if (isElectronCompile) {
                files = yield _this.compileUsingElectronCompile(files);
            }
            yield _this.createPackageFromFiles(_this.options.ordering == null ? files : yield _this.order(files));
        })();
    }
    compileUsingElectronCompile(files) {
        var _this2 = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            (0, (_log || _load_log()).log)("Compiling using electron-compile");
            const metadata = _this2.metadata;
            const cacheDir = _path.join(_this2.src, ".cache");
            // clear and create cache dir
            yield (0, (_fsExtraP || _load_fsExtraP()).emptyDir)(cacheDir);
            const compilerHost = yield (0, (_fileTransformer || _load_fileTransformer()).createElectronCompilerHost)(_this2.src,
cacheDir);
            const nextSlashIndex = _this2.src.length + 1;
            // pre-compute electron-compile to cache dir - we need to process only subdirectories, not direct files of app dir
            yield (_bluebirdLst2 || _load_bluebirdLst2()).default.map(files, function (file) {
                if (file.indexOf("/node_modules/") !== -1 || file.indexOf("/bower_components/") !== -1 || !(file.indexOf("/", nextSlashIndex
) !== -1) // ignore not root files
                || !metadata.get(file).isFile()) {
                    return null;
                }
                return compilerHost.compile(file).then(function (it) {
                    return null;
                });
            }, (_fs || _load_fs()).CONCURRENCY);
            yield compilerHost.saveConfiguration(); ...
```
- example usage
```shell
...
if (_this2.info.isPrepackedAppAsar) {
    promise = (0, (_fs || _load_fs()).copyDir)(appDir, _path.join(resourcesPath), filter, transformer);
} else if (asarOptions == null) {
    promise = (0, (_fs || _load_fs()).copyDir)(appDir, _path.join(resourcesPath, "app"), filter, transformer);
} else {
    const unpackPattern = (0, (_fileMatcher || _load_fileMatcher()).getFileMatchers)(_this2.config, "asarUnpack", appDir, _path.
join(resourcesPath, "app"), false, macroExpander, platformSpecificBuildOptions);
    const fileMatcher = unpackPattern == null ? null : unpackPattern[0];
    promise = new (_asarUtil || _load_asarUtil()).AsarPackager(appDir, resourcesPath, asarOptions, fileMatcher == null ? null :
fileMatcher.createFilter(), transformer).pack(filter, isElectronCompile);
}
//noinspection ES6MissingAwait
const promises = [promise, (0, (_fs || _load_fs()).unlinkIfExists)(_path.join(resourcesPath, "default_app.asar")), (0, (_fs || _load_fs
()).unlinkIfExists)(_path.join(appOutDir, "version")), _this2.postInitApp(appOutDir)];
if (_this2.platform !== (_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC) {
    promises.push((0, (_fsExtraP || _load_fsExtraP()).rename)(_path.join(appOutDir, "LICENSE"), _path.join(appOutDir, "LICENSE.electron
.txt")).catch(function () {}));
}
yield (_bluebirdLst2 || _load_bluebirdLst2()).default.all(promises);
...
```

#### <a name="apidoc.element.electron-builder.asarUtil.checkFileInArchive"></a>[function <span class="apidocSignatureSpan">electron-builder.asarUtil.</span>checkFileInArchive (_x2, _x3, _x4)](#apidoc.element.electron-builder.asarUtil.checkFileInArchive)
- description and source-code
```javascript
function checkFileInArchive(_x2, _x3, _x4) {
    return _ref2.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.builder"></a>[module electron-builder.builder](#apidoc.module.electron-builder.builder)

#### <a name="apidoc.element.electron-builder.builder.build"></a>[function <span class="apidocSignatureSpan">electron-builder.builder.</span>build (_x)](#apidoc.element.electron-builder.builder.build)
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

#### <a name="apidoc.element.electron-builder.builder.createTargets"></a>[function <span class="apidocSignatureSpan">electron-builder.builder.</span>createTargets (platforms, type, arch)](#apidoc.element.electron-builder.builder.createTargets)
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

#### <a name="apidoc.element.electron-builder.builder.normalizeOptions"></a>[function <span class="apidocSignatureSpan">electron-builder.builder.</span>normalizeOptions (args)](#apidoc.element.electron-builder.builder.normalizeOptions)
- description and source-code
```javascript
function normalizeOptions(args) {
    if (args.targets != null) {
        return args;
    }
    let targets = new Map();
    function processTargets(platform, types) {
        function commonArch(currentIfNotSpecified) {
            if (platform === (_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC) {
                return args.x64 || currentIfNotSpecified ? [(_electronBuilderCore || _load_electronBuilderCore()).Arch.x64] : [];
            }
            const result = Array();
            if (args.x64) {
                result.push((_electronBuilderCore || _load_electronBuilderCore()).Arch.x64);
            }
            if (args.armv7l) {
                result.push((_electronBuilderCore || _load_electronBuilderCore()).Arch.armv7l);
            }
            if (args.ia32) {
                result.push((_electronBuilderCore || _load_electronBuilderCore()).Arch.ia32);
            }
            return result.length === 0 && currentIfNotSpecified ? [(0, (_electronBuilderCore || _load_electronBuilderCore()).archFromString
)(process.arch)] : result;
        }
        if (args.platform != null) {
            throw new Error('--platform cannot be used if --${platform.buildConfigurationKey} is passed');
        }
        if (args.arch != null) {
            throw new Error('--arch cannot be used if --${platform.buildConfigurationKey} is passed');
        }
        let archToType = targets.get(platform);
        if (archToType == null) {
            archToType = new Map();
            targets.set(platform, archToType);
        }
        if (types.length === 0) {
            const defaultTargetValue = args.dir ? [(_electronBuilderCore || _load_electronBuilderCore()).DIR_TARGET] : [];
            for (const arch of commonArch(args.dir === true)) {
                archToType.set(arch, defaultTargetValue);
            }
            return;
        }
        for (const type of types) {
            const suffixPos = type.lastIndexOf(":");
            if (suffixPos > 0) {
                (0, (_electronBuilderUtil || _load_electronBuilderUtil()).addValue)(archToType, (0, (_electronBuilderCore || _load_electronBuilderCore
()).archFromString)(type.substring(suffixPos + 1)), type.substring(0, suffixPos));
            } else {
                for (const arch of commonArch(true)) {
                    (0, (_electronBuilderUtil || _load_electronBuilderUtil()).addValue)(archToType, arch, type);
                }
            }
        }
    }
    if (args.mac != null) {
        processTargets((_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC, args.mac);
    }
    if (args.linux != null) {
        processTargets((_electronBuilderCore || _load_electronBuilderCore()).Platform.LINUX, args.linux);
    }
    if (args.win != null) {
        processTargets((_electronBuilderCore || _load_electronBuilderCore()).Platform.WINDOWS, args.win);
    }
    if (targets.size === 0) {
        if (args.platform == null && args.arch == null) {
            processTargets((_electronBuilderCore || _load_electronBuilderCore()).Platform.current(), []);
        } else {
            targets = createTargets((0, (_packager || _load_packager()).normalizePlatforms)(args.platform), args.dir ? (_electronBuilderCore
 || _load_electronBuilderCore()).DIR_TARGET : null, args.arch);
        }
    }
    const result = Object.assign({}, args);
    result.targets = targets;
    delete result.dir;
    delete result.mac;
    delete result.linux;
    delete result.win;
    delete result.platform;
    delete result.arch;
    const r = result;
    delete r.em;
    delete r.m;
    delete r.o;
    delete r.l;
    delete r.w;
    delete r.windows;
    delete r.macos;
    delete r.$0;
    delete r._;
    delete r.version;
    delete r.help;
    delete result.ia32;
    delete result.x64;
    delete result.armv7l;
    if (result.project != null && result.projectDir == null) {
        result.projectDir = result.project;
    }
    delete result.project;
    return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.codeSign"></a>[module electron-builder.codeSign](#apidoc.module.electron-builder.codeSign)

#### <a name="apidoc.element.electron-builder.codeSign.createKeychain"></a>[function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>createKeychain (_x3, _x4, _x5, _x6, _x7)](#apidoc.element.electron-builder.codeSign.createKeychain)
- description and source-code
```javascript
function createKeychain(_x3, _x4, _x5, _x6, _x7) {
    return _ref3.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.codeSign.downloadCertificate"></a>[function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>downloadCertificate (_x, _x2)](#apidoc.element.electron-builder.codeSign.downloadCertificate)
- description and source-code
```javascript
function downloadCertificate(_x, _x2) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.codeSign.findIdentity"></a>[function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>findIdentity (certType, qualifier, keychain)](#apidoc.element.electron-builder.codeSign.findIdentity)
- description and source-code
```javascript
function findIdentity(certType, qualifier, keychain) {
    let identity = qualifier || process.env.CSC_NAME;
    if ((0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(identity)) {
        if (keychain == null && !(_isCi || _load_isCi()).default && process.env.CSC_IDENTITY_AUTO_DISCOVERY === "false") {
            return (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve(null);
        } else {
            return _findIdentity(certType, null, keychain);
        }
    } else {
        identity = identity.trim();
        for (const prefix of appleCertificatePrefixes) {
            checkPrefix(identity, prefix);
        }
        return _findIdentity(certType, identity, keychain);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.codeSign.sign"></a>[function <span class="apidocSignatureSpan">electron-builder.codeSign.</span>sign (path, name, keychain)](#apidoc.element.electron-builder.codeSign.sign)
- description and source-code
```javascript
function sign(path, name, keychain) {
    const args = ["--deep", "--force", "--sign", name, path];
    if (keychain != null) {
        args.push("--keychain", keychain);
    }
    return (0, (_electronBuilderUtil || _load_electronBuilderUtil()).exec)("codesign", args);
}
```
- example usage
```shell
...
const hasMas = targets.length !== 0 && targets.some(function (it) {
    return it.name === "mas" || it.name === "mas-dev";
});
const prepackaged = _this2.info.prepackaged;
if (!hasMas || targets.length > 1) {
    const appPath = prepackaged == null ? _path.join(_this2.computeAppOutDir(outDir, arch), '${_this2.appInfo.productFilename}.app
') : prepackaged;
    nonMasPromise = (prepackaged ? (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve() : _this2.doPack(outDir, _path.dirname
(appPath), _this2.platform.nodeName, arch, _this2.platformSpecificBuildOptions, targets)).then(function () {
        return _this2.sign(appPath, null, null);
    }).then(function () {
        return _this2.packageInDistributableFormat(appPath, (_electronBuilderCore || _load_electronBuilderCore()).Arch.x64, targets
, postAsyncTasks);
    });
}
for (const target of targets) {
    const targetName = target.name;
    if (!(targetName === "mas" || targetName === "mas-dev")) {
...
```



# <a name="apidoc.module.electron-builder.fileMatcher"></a>[module electron-builder.fileMatcher](#apidoc.module.electron-builder.fileMatcher)

#### <a name="apidoc.element.electron-builder.fileMatcher.FileMatcher"></a>[function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>FileMatcher (from, to, macroExpander, patterns)](#apidoc.element.electron-builder.fileMatcher.FileMatcher)
- description and source-code
```javascript
class FileMatcher {
    constructor(from, to, macroExpander, patterns) {
        this.macroExpander = macroExpander;
        this.from = macroExpander(from);
        this.to = macroExpander(to);
        this.patterns = (0, (_electronBuilderUtil || _load_electronBuilderUtil()).asArray)(patterns).map(it => _path.posix.normalize
(macroExpander(it)));
    }
    addPattern(pattern) {
        this.patterns.push(_path.posix.normalize(this.macroExpander(pattern)));
    }
    addAllPattern() {
        // must be first, see minimatchAll implementation
        this.patterns.unshift("**/*");
    }
    isEmpty() {
        return this.patterns.length === 0;
    }
    containsOnlyIgnore() {
        return !this.isEmpty() && this.patterns.find(it => !it.startsWith("!")) == null;
    }
    computeParsedPatterns(result, fromDir) {
        // https://github.com/electron-userland/electron-builder/issues/733
        const minimatchOptions = { dot: true };
        const relativeFrom = fromDir == null ? null : _path.relative(fromDir, this.from);
        if (this.patterns.length === 0 && relativeFrom != null) {
            // file mappings, from here is a file
            result.push(new (_minimatch || _load_minimatch()).Minimatch(relativeFrom, minimatchOptions));
            return;
        }
        for (let pattern of this.patterns) {
            if (relativeFrom != null) {
                pattern = _path.join(relativeFrom, pattern);
            }
            const parsedPattern = new (_minimatch || _load_minimatch()).Minimatch(pattern, minimatchOptions);
            result.push(parsedPattern);
            if (!(0, (_filter || _load_filter()).hasMagic)(parsedPattern)) {
                // https://github.com/electron-userland/electron-builder/issues/545
                // add **/*
                result.push(new (_minimatch || _load_minimatch()).Minimatch('${pattern}/**/*', minimatchOptions));
            }
        }
    }
    createFilter(ignoreFiles, rawFilter, excludePatterns) {
        const parsedPatterns = [];
        this.computeParsedPatterns(parsedPatterns);
        return (0, (_filter || _load_filter()).createFilter)(this.from, parsedPatterns, ignoreFiles, rawFilter, excludePatterns);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.fileMatcher.copyFiles"></a>[function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>copyFiles (patterns)](#apidoc.element.electron-builder.fileMatcher.copyFiles)
- description and source-code
```javascript
function copyFiles(patterns) {
    if (patterns == null || patterns.length === 0) {
        return (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve();
    }
    return (_bluebirdLst2 || _load_bluebirdLst2()).default.map(patterns, (() => {
        var _ref = (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* (pattern) {
            const fromStat = yield (0, (_fs || _load_fs()).statOrNull)(pattern.from);
            if (fromStat == null) {
                (0, (_log || _load_log()).warn)('File source ${pattern.from} doesn't exist');
                return;
            }
            if (fromStat.isFile()) {
                const toStat = yield (0, (_fs || _load_fs()).statOrNull)(pattern.to);
                // https://github.com/electron-userland/electron-builder/issues/1245
                if (toStat != null && toStat.isDirectory()) {
                    return yield (0, (_fs || _load_fs()).copyFile)(pattern.from, _path.join(pattern.to, _path.basename(pattern.from
)), fromStat);
                }
                yield (0, (_fsExtraP || _load_fsExtraP()).mkdirs)(_path.dirname(pattern.to));
                return yield (0, (_fs || _load_fs()).copyFile)(pattern.from, pattern.to, fromStat);
            }
            if (pattern.isEmpty() || pattern.containsOnlyIgnore()) {
                pattern.addAllPattern();
            }
            return yield (0, (_fs || _load_fs()).copyDir)(pattern.from, pattern.to, pattern.createFilter());
        });

        return function (_x) {
            return _ref.apply(this, arguments);
        };
    })());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.fileMatcher.createFileMatcher"></a>[function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>createFileMatcher (info, appDir, resourcesPath, macroExpander, platformSpecificBuildOptions)](#apidoc.element.electron-builder.fileMatcher.createFileMatcher)
- description and source-code
```javascript
function createFileMatcher(info, appDir, resourcesPath, macroExpander, platformSpecificBuildOptions) {
    const patterns = info.isPrepackedAppAsar ? null : getFileMatchers(info.config, "files", appDir, _path.join(resourcesPath, "app
"), false, macroExpander, platformSpecificBuildOptions);
    const matcher = patterns == null ? new FileMatcher(appDir, _path.join(resourcesPath, "app"), macroExpander) : patterns[0];
    if (matcher.isEmpty() || matcher.containsOnlyIgnore()) {
        matcher.addAllPattern();
    } else {
        matcher.addPattern("package.json");
    }
    matcher.addPattern("!**/node_modules/*/{CHANGELOG.md,ChangeLog,changelog.md,README.md,README,readme.md,readme,test,__tests__
,tests,powered-test,example,examples,*.d.ts}");
    matcher.addPattern("!**/node_modules/.bin");
    matcher.addPattern("!**/*.{o,hprof,orig,pyc,pyo,rbc,swp}");
    matcher.addPattern("!**/._*");
    matcher.addPattern("!*.iml");
    //noinspection SpellCheckingInspection
    matcher.addPattern("!**/{.git,.hg,.svn,CVS,RCS,SCCS," + "__pycache__,.DS_Store,thumbs.db,.gitignore,.gitattributes," + ".editorconfig
,.flowconfig,.jshintrc,.eslintrc," + ".yarn-integrity,.yarn-metadata.json,yarn-error.log,yarn.lock,npm-debug.log," + ".idea," + "
appveyor.yml,.travis.yml,circle.yml," + ".nyc_output}");
    return matcher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.fileMatcher.getFileMatchers"></a>[function <span class="apidocSignatureSpan">electron-builder.fileMatcher.</span>getFileMatchers (config, name, defaultSrc, defaultDest, allowAdvancedMatching, macroExpander, customBuildOptions)](#apidoc.element.electron-builder.fileMatcher.getFileMatchers)
- description and source-code
```javascript
function getFileMatchers(config, name, defaultSrc, defaultDest, allowAdvancedMatching, macroExpander, customBuildOptions) {
    const globalPatterns = config[name];
    const platformSpecificPatterns = customBuildOptions[name];
    const defaultMatcher = new FileMatcher(defaultSrc, defaultDest, macroExpander);
    const fileMatchers = [];
    function addPatterns(patterns) {
        if (patterns == null) {
            return;
        } else if (!Array.isArray(patterns)) {
            if (typeof patterns === "string") {
                defaultMatcher.addPattern(patterns);
                return;
            }
            patterns = [patterns];
        }
        for (const pattern of patterns) {
            if (typeof pattern === "string") {
                // use normalize to transform ./foo to foo
                defaultMatcher.addPattern(pattern);
            } else if (allowAdvancedMatching) {
                const from = pattern.from == null ? defaultSrc : _path.resolve(defaultSrc, pattern.from);
                const to = pattern.to == null ? defaultDest : _path.resolve(defaultDest, pattern.to);
                fileMatchers.push(new FileMatcher(from, to, macroExpander, pattern.filter));
            } else {
                throw new Error('Advanced file copying not supported for "${name}"');
            }
        }
    }
    addPatterns(globalPatterns);
    addPatterns(platformSpecificPatterns);
    if (!defaultMatcher.isEmpty()) {
        // default matcher should be first in the array
        fileMatchers.unshift(defaultMatcher);
    }
    return fileMatchers.length === 0 ? null : fileMatchers;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.fileTransformer"></a>[module electron-builder.fileTransformer](#apidoc.module.electron-builder.fileTransformer)

#### <a name="apidoc.element.electron-builder.fileTransformer.createElectronCompilerHost"></a>[function <span class="apidocSignatureSpan">electron-builder.fileTransformer.</span>createElectronCompilerHost (projectDir, cacheDir)](#apidoc.element.electron-builder.fileTransformer.createElectronCompilerHost)
- description and source-code
```javascript
function createElectronCompilerHost(projectDir, cacheDir) {
    const electronCompilePath = _path.join(projectDir, "node_modules", "electron-compile", "lib");
    return require(_path.join(electronCompilePath, "config-parser")).createCompilerHostFromProjectRoot(projectDir, cacheDir);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.fileTransformer.createTransformer"></a>[function <span class="apidocSignatureSpan">electron-builder.fileTransformer.</span>createTransformer (_x, _x2)](#apidoc.element.electron-builder.fileTransformer.createTransformer)
- description and source-code
```javascript
function createTransformer(_x, _x2) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.fileTransformer.isElectronCompileUsed"></a>[function <span class="apidocSignatureSpan">electron-builder.fileTransformer.</span>isElectronCompileUsed (info)](#apidoc.element.electron-builder.fileTransformer.isElectronCompileUsed)
- description and source-code
```javascript
function isElectronCompileUsed(info) {
    if (info.config.electronCompile != null) {
        return info.config.electronCompile;
    }
    // if in devDependencies - it means that babel is used for precompilation or for some reason user decided to not use electron
-compile for production
    const deps = info.metadata.dependencies;
    return deps != null && "electron-compile" in deps;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.linuxPackager"></a>[module electron-builder.linuxPackager](#apidoc.module.electron-builder.linuxPackager)

#### <a name="apidoc.element.electron-builder.linuxPackager.LinuxPackager"></a>[function <span class="apidocSignatureSpan">electron-builder.linuxPackager.</span>LinuxPackager (_platformPackager || _load_platformPackager()](#apidoc.element.electron-builder.linuxPackager.LinuxPackager)
- description and source-code
```javascript
class LinuxPackager extends (_platformPackager || _load_platformPackager()).PlatformPackager {
    constructor(info) {
        super(info);
        const executableName = this.platformSpecificBuildOptions.executableName;
        this.executableName = (0, (_sanitizeFilename || _load_sanitizeFilename()).default)(executableName == null ? this.appInfo
.name.toLowerCase() : executableName);
    }
    get defaultTarget() {
        return ["appimage"];
    }
    createTargets(targets, mapper, cleanupTasks) {
        let helper;
        const getHelper = () => {
            if (helper == null) {
                helper = new (_LinuxTargetHelper || _load_LinuxTargetHelper()).LinuxTargetHelper(this);
            }
            return helper;
        };
        for (const name of targets) {
            if (name === (_electronBuilderCore || _load_electronBuilderCore()).DIR_TARGET) {
                continue;
            }
            const targetClass = (() => {
                switch (name) {
                    case "appimage":
                        return require("./targets/appImage").default;
                    case "snap":
                        return require("./targets/snap").default;
                    case "deb":
                    case "rpm":
                    case "sh":
                    case "freebsd":
                    case "pacman":
                    case "apk":
                    case "p5p":
                        return require("./targets/fpm").default;
                    default:
                        return null;
                }
            })();
            mapper(name, outDir => targetClass === null ? (0, (_targetFactory || _load_targetFactory()).createCommonTarget)(name
, outDir, this) : new targetClass(name, this, getHelper(), outDir));
        }
    }
    get platform() {
        return (_electronBuilderCore || _load_electronBuilderCore()).Platform.LINUX;
    }
    postInitApp(appOutDir) {
        return (0, (_fsExtraP || _load_fsExtraP()).rename)(_path.join(appOutDir, this.electronDistExecutableName), _path.join(appOutDir
, this.executableName));
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.macPackager"></a>[module electron-builder.macPackager](#apidoc.module.electron-builder.macPackager)

#### <a name="apidoc.element.electron-builder.macPackager.default"></a>[function <span class="apidocSignatureSpan">electron-builder.macPackager.</span>default (_platformPackager || _load_platformPackager()](#apidoc.element.electron-builder.macPackager.default)
- description and source-code
```javascript
class MacPackager extends (_platformPackager || _load_platformPackager()).PlatformPackager {
    constructor(info) {
        super(info);
        if (this.packagerOptions.cscLink == null || process.platform !== "darwin") {
            this.codeSigningInfo = (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve(Object.create(null));
        } else {
            this.codeSigningInfo = (0, (_codeSign || _load_codeSign()).createKeychain)(info.tempDirManager, this.packagerOptions
.cscLink, this.getCscPassword(), this.packagerOptions.cscInstallerLink, this.packagerOptions.cscInstallerKeyPassword);
        }
    }
    get defaultTarget() {
        return ["zip", "dmg"];
    }
    prepareAppInfo(appInfo) {
        return new (_appInfo || _load_appInfo()).AppInfo(appInfo.metadata, this.info, this.platformSpecificBuildOptions.bundleVersion
);
    }
    getIconPath() {
        var _this = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            let iconPath = _this.platformSpecificBuildOptions.icon || _this.config.icon;
            if (iconPath != null && !iconPath.endsWith(".icns")) {
                iconPath += ".icns";
            }
            return iconPath == null ? yield _this.getDefaultIcon("icns") : yield _this.getResource(iconPath);
        })();
    }
    createTargets(targets, mapper, cleanupTasks) {
        for (const name of targets) {
            switch (name) {
                case (_electronBuilderCore || _load_electronBuilderCore()).DIR_TARGET:
                    break;
                case "dmg":
                    mapper("dmg", outDir => new (_dmg || _load_dmg()).DmgTarget(this, outDir));
                    break;
                case "pkg":
                    mapper("pkg", outDir => new (_pkg || _load_pkg()).PkgTarget(this, outDir));
                    break;
                default:
                    mapper(name, outDir => name === "mas" || name === "mas-dev" ? new (_targetFactory || _load_targetFactory()).
NoOpTarget(name) : (0, (_targetFactory || _load_targetFactory()).createCommonTarget)(name, outDir, this));
                    break;
            }
        }
    }
    get platform() {
        return (_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC;
    }
    pack(outDir, arch, targets, postAsyncTasks) {
        var _this2 = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            let nonMasPromise = null;
            const hasMas = targets.length !== 0 && targets.some(function (it) {
                return it.name === "mas" || it.name === "mas-dev";
            });
            const prepackaged = _this2.info.prepackaged;
            if (!hasMas || targets.length > 1) {
                const appPath = prepackaged == null ? _path.join(_this2.computeAppOutDir(outDir, arch), '${_this2.appInfo.productFilename
}.app') : prepackaged;
                nonMasPromise = (prepackaged ? (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve() : _this2.doPack(outDir,
_path.dirname(appPath), _this2.platform.nodeName, arch, _this2.platformSpecificBuildOptions, targets)).then(function () {
                    return _this2.sign(appPath, null, null);
                }).then(function () {
                    return _this2.packageInDistributableFormat(appPath, (_electronBuilderCore || _load_electronBuilderCore()).Arch
.x64, targets, postAsyncTasks);
                });
            }
            for (const target of targets) {
                const targetName = target.name;
                if (!(targetName === "mas" || targetName === "mas-dev")) {
                    continue;
                }
                const masBuildOptions = (0, (_deepAssign || _load_deepAssign()).deepAssign)({}, _this2.platformSpecificBuildOptions
, _this2.config.mas);
                if (targetName === "mas-dev") {
                    (0, (_deepAssign || _load_deepAssign()).deepAssign)(masBuildOptions, _this2.config[targetName]);
                    masBuildOptions.type = "development";
                }
                const target ...
```
- example usage
```shell
...
headerPickle.writeString(JSON.stringify(this.fs.header));
const headerBuf = headerPickle.toBuffer();
const sizePickle = pickle.createEmpty();
sizePickle.writeUInt32(headerBuf.length);
const sizeBuf = sizePickle.toBuffer();
const transformedFiles = this.transformedFiles;
const writeStream = (0, (_fsExtraP || _load_fsExtraP()).createWriteStream)(this.outFile);
return new (_bluebirdLst2 || _load_bluebirdLst2()).default((resolve, reject) => {
    writeStream.on("error", reject);
    writeStream.on("close", resolve);
    writeStream.write(sizeBuf);
    const w = index => {
        let data;
        while (true) {
            if (index >= files.length) {
...
```



# <a name="apidoc.module.electron-builder.packager"></a>[module electron-builder.packager](#apidoc.module.electron-builder.packager)

#### <a name="apidoc.element.electron-builder.packager.Packager"></a>[function <span class="apidocSignatureSpan">electron-builder.packager.</span>Packager (options, cancellationToken)](#apidoc.element.electron-builder.packager.Packager)
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
...
if (options.draft === undefined && !(0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(process.env.EP_DRAFT
)) {
    options.draft = process.env.EP_DRAFT.toLowerCase() === "true";
}
if (options.prerelease === undefined && !(0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(process.env.
EP_PRELEASE)) {
    options.prerelease = process.env.EP_PRELEASE.toLowerCase() === "true";
}
const cancellationToken = new (_CancellationToken || _load_CancellationToken()).CancellationToken();
const packager = new (_packager || _load_packager()).Packager(options, cancellationToken);
// because artifact event maybe dispatched several times for different publish providers
const artifactPaths = new Set();
packager.artifactCreated(function (event) {
    if (event.file != null) {
        artifactPaths.add(event.file);
    }
});
...
```

#### <a name="apidoc.element.electron-builder.packager.checkWineVersion"></a>[function <span class="apidocSignatureSpan">electron-builder.packager.</span>checkWineVersion (_x)](#apidoc.element.electron-builder.packager.checkWineVersion)
- description and source-code
```javascript
function checkWineVersion(_x) {
    return _ref5.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.packager.normalizePlatforms"></a>[function <span class="apidocSignatureSpan">electron-builder.packager.</span>normalizePlatforms (rawPlatforms)](#apidoc.element.electron-builder.packager.normalizePlatforms)
- description and source-code
```javascript
function normalizePlatforms(rawPlatforms) {
    const platforms = rawPlatforms == null || Array.isArray(rawPlatforms) ? rawPlatforms : [rawPlatforms];
    if (platforms == null || platforms.length === 0) {
        return [(_electronBuilderCore || _load_electronBuilderCore()).Platform.fromString(process.platform)];
    } else if (platforms[0] === "all") {
        if (process.platform === (_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC.nodeName) {
            return [(_electronBuilderCore || _load_electronBuilderCore()).Platform.MAC, (_electronBuilderCore || _load_electronBuilderCore
()).Platform.LINUX, (_electronBuilderCore || _load_electronBuilderCore()).Platform.WINDOWS];
        } else if (process.platform === (_electronBuilderCore || _load_electronBuilderCore()).Platform.LINUX.nodeName) {
            // macOS code sign works only on macOS
            return [(_electronBuilderCore || _load_electronBuilderCore()).Platform.LINUX, (_electronBuilderCore || _load_electronBuilderCore
()).Platform.WINDOWS];
        } else {
            return [(_electronBuilderCore || _load_electronBuilderCore()).Platform.WINDOWS];
        }
    } else {
        return platforms.map(it => it instanceof (_electronBuilderCore || _load_electronBuilderCore()).Platform ? it : (_electronBuilderCore
 || _load_electronBuilderCore()).Platform.fromString(it));
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.platformPackager"></a>[module electron-builder.platformPackager](#apidoc.module.electron-builder.platformPackager)

#### <a name="apidoc.element.electron-builder.platformPackager.PlatformPackager"></a>[function <span class="apidocSignatureSpan">electron-builder.platformPackager.</span>PlatformPackager (info)](#apidoc.element.electron-builder.platformPackager.PlatformPackager)
- description and source-code
```javascript
class PlatformPackager {
    constructor(info) {
        this.info = info;
        this._resourceList = new (_electronBuilderUtil || _load_electronBuilderUtil()).Lazy(() => {
            return (0, (_fsExtraP || _load_fsExtraP()).readdir)(this.buildResourcesDir).catch(e => {
                if (e.code !== "ENOENT") {
                    throw e;
                }
                return [];
            });
        });
        this.config = info.config;
        this.platformSpecificBuildOptions = PlatformPackager.normalizePlatformSpecificBuildOptions(this.config[this.platform.buildConfigurationKey
]);
        this.appInfo = this.prepareAppInfo(info.appInfo);
        this.packagerOptions = info.options;
        this.projectDir = info.projectDir;
        this.buildResourcesDir = _path.resolve(this.projectDir, this.relativeBuildResourcesDirname);
    }
    get resourceList() {
        return this._resourceList.value;
    }
    prepareAppInfo(appInfo) {
        return appInfo;
    }
    static normalizePlatformSpecificBuildOptions(options) {
        return options == null ? Object.create(null) : options;
    }
    getCscPassword() {
        const password = this.doGetCscPassword();
        if ((0, (_electronBuilderUtil || _load_electronBuilderUtil()).isEmptyOrSpaces)(password)) {
            (0, (_log || _load_log()).log)("CSC_KEY_PASSWORD is not defined, empty password will be used");
            return "";
        } else {
            return password.trim();
        }
    }
    doGetCscPassword() {
        return this.packagerOptions.cscKeyPassword || process.env.CSC_KEY_PASSWORD;
    }
    get relativeBuildResourcesDirname() {
        return (0, (_electronBuilderUtil || _load_electronBuilderUtil()).use)(this.config.directories, it => it.buildResources) || "
build";
    }
    computeAppOutDir(outDir, arch) {
        return this.info.prepackaged || _path.join(outDir, '${this.platform.buildConfigurationKey}${(0, (_electronBuilderCore ||
_load_electronBuilderCore()).getArchSuffix)(arch)}${this.platform === (_electronBuilderCore || _load_electronBuilderCore()).Platform
.MAC ? "" : "-unpacked"}');
    }
    dispatchArtifactCreated(file, target, arch, safeArtifactName) {
        this.info.dispatchArtifactCreated({
            file, safeArtifactName, target, arch,
            packager: this
        });
    }
    pack(outDir, arch, targets, postAsyncTasks) {
        var _this = this;

        return (0, (_bluebirdLst || _load_bluebirdLst()).coroutine)(function* () {
            const appOutDir = _this.computeAppOutDir(outDir, arch);
            yield _this.doPack(outDir, appOutDir, _this.platform.nodeName, arch, _this.platformSpecificBuildOptions, targets);
            _this.packageInDistributableFormat(appOutDir, arch, targets, postAsyncTasks);
        })();
    }
    packageInDistributableFormat(appOutDir, arch, targets, postAsyncTasks) {
        postAsyncTasks.push((_bluebirdLst2 || _load_bluebirdLst2()).default.map(targets, it => it.isAsyncSupported ? it.build(appOutDir
, arch) : null).then(() => (_bluebirdLst2 || _load_bluebirdLst2()).default.each(targets, it => it.isAsyncSupported ? null : it.build
(appOutDir, arch))));
    }
    getExtraFileMatchers(isResources, appOutDir, macroExpander, customBuildOptions) {
        const base = isResources ? this.getResourcesDir(appOutDir) : this.platform === (_electronBuilderCore || _load_electronBuilderCore
()).Platform.MAC ? _path.join(appOutDir, '${this.appInfo.productFilename}.app', "Contents") : appOutDir;
        return (0, (_fileMatcher || _load_fileMatcher()).getFileMatchers)(this.config, isResources ? "extraResources" : "extraFiles
", this.projectDir, base, true, macroExpander, customBuildOptions);
    }
    get electronDistMacOsAppName() {
        return this.info.muonVersion == null ? "Electron.app" : "Brave.app";
    }
    get electronDistExecutableName() {
        return this.info.muonVersion == null ? "electron" : "brave";
    }
    get electronDistMacOsExecutableName() {
        return this.info.muonVersion == null ? "Electron" : "Brave";
    }
    doPack(outDir, appOutDir, ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.platformPackager.normalizeExt"></a>[function <span class="apidocSignatureSpan">electron-builder.platformPackager.</span>normalizeExt (ext)](#apidoc.element.electron-builder.platformPackager.normalizeExt)
- description and source-code
```javascript
function normalizeExt(ext) {
    return ext.startsWith(".") ? ext.substring(1) : ext;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.readInstalled"></a>[module electron-builder.readInstalled](#apidoc.module.electron-builder.readInstalled)

#### <a name="apidoc.element.electron-builder.readInstalled.readInstalled"></a>[function <span class="apidocSignatureSpan">electron-builder.</span>readInstalled (_x)](#apidoc.element.electron-builder.readInstalled.readInstalled)
- description and source-code
```javascript
function readInstalled(_x) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.repositoryInfo"></a>[module electron-builder.repositoryInfo](#apidoc.module.electron-builder.repositoryInfo)

#### <a name="apidoc.element.electron-builder.repositoryInfo.getRepositoryInfo"></a>[function <span class="apidocSignatureSpan">electron-builder.repositoryInfo.</span>getRepositoryInfo (projectDir, metadata, devMetadata)](#apidoc.element.electron-builder.repositoryInfo.getRepositoryInfo)
- description and source-code
```javascript
function getRepositoryInfo(projectDir, metadata, devMetadata) {
    return _getInfo(projectDir, (devMetadata == null ? null : devMetadata.repository) || (metadata == null ? null : metadata.repository
));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.winPackager"></a>[module electron-builder.winPackager](#apidoc.module.electron-builder.winPackager)

#### <a name="apidoc.element.electron-builder.winPackager.WinPackager"></a>[function <span class="apidocSignatureSpan">electron-builder.winPackager.</span>WinPackager (_platformPackager || _load_platformPackager()](#apidoc.element.electron-builder.winPackager.WinPackager)
- description and source-code
```javascript
class WinPackager extends (_platformPackager || _load_platformPackager()).PlatformPackager {
    constructor(info) {
        var _this;

        _this = super(info);
        this.cscInfo = new (_electronBuilderUtil || _load_electronBuilderUtil()).Lazy(() => {
            const platformSpecificBuildOptions = this.platformSpecificBuildOptions;
            const subjectName = platformSpecificBuildOptions.certificateSubjectName;
            if (subjectName != null) {
                return (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve({ subjectName });
            }
            const certificateSha1 = platformSpecificBuildOptions.certificateSha1;
            if (certificateSha1 != null) {
                return (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve({ certificateSha1 });
            }
            const certificateFile = platformSpecificBuildOptions.certificateFile;
            if (certificateFile != null) {
                const certificatePassword = this.getCscPassword();
                return (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve({
                    file: certificateFile,
                    password: certificatePassword == null ? null : certificatePassword.trim()
                });
            } else {
                const cscLink = process.env.WIN_CSC_LINK || this.packagerOptions.cscLink;
                if (cscLink != null) {
                    return (0, (_codeSign || _load_codeSign()).downloadCertificate)(cscLink, this.info.tempDirManager).then(path
 => {
                        return {
                            file: path,
                            password: this.getCscPassword()
                        };
                    });
                } else {
                    return (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve(null);
                }
            }
        });
        this.computedPublisherName = new (_electronBuilderUtil || _load_electronBuilderUtil()).Lazy((0, (_bluebirdLst || _load_bluebirdLst
()).coroutine)(function* () {
            let publisherName = _this.platformSpecificBuildOptions.publisherName;
            if (publisherName === null) {
                return null;
            }
            const cscInfo = yield _this.cscInfo.value;
            if (cscInfo == null) {
                return null;
            }
            if (publisherName == null && cscInfo.file != null) {
                try {
                    // https://github.com/digitalbazaar/forge/issues/338#issuecomment-164831585
                    const p12Asn1 = (_nodeForge || _load_nodeForge()).asn1.fromDer((yield (0, (_fsExtraP || _load_fsExtraP()).readFile
)(cscInfo.file, "binary")), false);
                    const p12 = (_nodeForge || _load_nodeForge()).pkcs12.pkcs12FromAsn1(p12Asn1, false, cscInfo.password);
                    const bagType = (_nodeForge || _load_nodeForge()).pki.oids.certBag;
                    publisherName = p12.getBags({ bagType: bagType })[bagType][0].cert.subject.getField("CN").value;
                } catch (e) {
                    throw new Error('Cannot extract publisher name from code signing certificate, please file issue. As workaround
, set win.publisherName: ${e.stack || e}');
                }
            }
            return publisherName == null ? null : (0, (_electronBuilderUtil || _load_electronBuilderUtil()).asArray)(publisherName
);
        }));
    }
    get defaultTarget() {
        return ["nsis"];
    }
    doGetCscPassword() {
        return this.platformSpecificBuildOptions.certificatePassword || process.env.WIN_CSC_KEY_PASSWORD || super.doGetCscPassword
();
    }
    createTargets(targets, mapper, cleanupTasks) {
        for (const name of targets) {
            if (name === (_electronBuilderCore || _load_electronBuilderCore()).DIR_TARGET) {
                continue;
            }
            const targetClass = (() => {
                switch (name) {
                    case "nsis":
                    case "portable":
                        return require("./targets/nsis").default;
                    case ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-builder.windowsCodeSign"></a>[module electron-builder.windowsCodeSign](#apidoc.module.electron-builder.windowsCodeSign)

#### <a name="apidoc.element.electron-builder.windowsCodeSign.getSignVendorPath"></a>[function <span class="apidocSignatureSpan">electron-builder.windowsCodeSign.</span>getSignVendorPath ()](#apidoc.element.electron-builder.windowsCodeSign.getSignVendorPath)
- description and source-code
```javascript
function getSignVendorPath() {
    //noinspection SpellCheckingInspection
    return (0, (_binDownload || _load_binDownload()).getBinFromBintray)("winCodeSign", TOOLS_VERSION, "a34a60e74d02b81d0303e498f03c70ce0133f908b671f62ec32896db5cd0a716
");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.windowsCodeSign.getToolPath"></a>[function <span class="apidocSignatureSpan">electron-builder.windowsCodeSign.</span>getToolPath ()](#apidoc.element.electron-builder.windowsCodeSign.getToolPath)
- description and source-code
```javascript
function getToolPath() {
    return _ref3.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.windowsCodeSign.sign"></a>[function <span class="apidocSignatureSpan">electron-builder.windowsCodeSign.</span>sign (_x)](#apidoc.element.electron-builder.windowsCodeSign.sign)
- description and source-code
```javascript
function sign(_x) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
...
const hasMas = targets.length !== 0 && targets.some(function (it) {
    return it.name === "mas" || it.name === "mas-dev";
});
const prepackaged = _this2.info.prepackaged;
if (!hasMas || targets.length > 1) {
    const appPath = prepackaged == null ? _path.join(_this2.computeAppOutDir(outDir, arch), '${_this2.appInfo.productFilename}.app
') : prepackaged;
    nonMasPromise = (prepackaged ? (_bluebirdLst2 || _load_bluebirdLst2()).default.resolve() : _this2.doPack(outDir, _path.dirname
(appPath), _this2.platform.nodeName, arch, _this2.platformSpecificBuildOptions, targets)).then(function () {
        return _this2.sign(appPath, null, null);
    }).then(function () {
        return _this2.packageInDistributableFormat(appPath, (_electronBuilderCore || _load_electronBuilderCore()).Arch.x64, targets
, postAsyncTasks);
    });
}
for (const target of targets) {
    const targetName = target.name;
    if (!(targetName === "mas" || targetName === "mas-dev")) {
...
```



# <a name="apidoc.module.electron-builder.yarn"></a>[module electron-builder.yarn](#apidoc.module.electron-builder.yarn)

#### <a name="apidoc.element.electron-builder.yarn.getGypEnv"></a>[function <span class="apidocSignatureSpan">electron-builder.yarn.</span>getGypEnv (electronVersion, platform, arch, buildFromSource)](#apidoc.element.electron-builder.yarn.getGypEnv)
- description and source-code
```javascript
function getGypEnv(electronVersion, platform, arch, buildFromSource) {
    const gypHome = _path.join((0, (_os || _load_os()).homedir)(), ".electron-gyp");
    return Object.assign({}, process.env, {
        npm_config_disturl: "https://atom.io/download/electron",
        npm_config_target: electronVersion,
        npm_config_runtime: "electron",
        npm_config_arch: arch,
        npm_config_target_arch: arch,
        npm_config_platform: platform,
        npm_config_build_from_source: buildFromSource,
        HOME: gypHome,
        USERPROFILE: gypHome
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.yarn.installOrRebuild"></a>[function <span class="apidocSignatureSpan">electron-builder.yarn.</span>installOrRebuild (_x, _x2, _x3, _x4, _x5)](#apidoc.element.electron-builder.yarn.installOrRebuild)
- description and source-code
```javascript
function installOrRebuild(_x, _x2, _x3, _x4, _x5) {
    return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-builder.yarn.rebuild"></a>[function <span class="apidocSignatureSpan">electron-builder.yarn.</span>rebuild (_x9, _x10)](#apidoc.element.electron-builder.yarn.rebuild)
- description and source-code
```javascript
function rebuild(_x9, _x10) {
    return _ref2.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
