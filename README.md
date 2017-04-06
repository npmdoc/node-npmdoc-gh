# api documentation for  [gh (v1.12.8)](http://nodegh.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-gh.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gh) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gh.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gh)
#### GitHub command line tools.

[![NPM](https://nodei.co/npm/gh.png?downloads=true)](https://www.npmjs.com/package/gh)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gh/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gh_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gh/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gh/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gh/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Eduardo Lundgren",
        "email": "eduardolundgren@gmail.com",
        "url": "http://eduardo.io"
    },
    "bin": {
        "gh": "bin/gh.js"
    },
    "bugs": {
        "url": "https://github.com/node-gh/gh/issues"
    },
    "contributors": [
        {
            "name": "Zeno Rocha",
            "email": "zno.rocha@gmail.com",
            "url": "http://zenorocha.com"
        }
    ],
    "dependencies": {
        "async": "^1.5.0",
        "babel-polyfill": "^6.0.16",
        "colors": "^1.1.2",
        "github": "^0.2.4",
        "handlebars": "^4.0.4",
        "inquirer": "^0.11.0",
        "insight": "^0.7.0",
        "lodash": "^3.10.1",
        "moment": "^2.13.0",
        "nopt": "^3.0.4",
        "open": "^0.0.5",
        "request": "^2.65.0",
        "truncate": "^2.0.0",
        "update-notifier": "^0.5.0",
        "userhome": "^1.0.0",
        "which": "^1.2.0",
        "wordwrap": "^1.0.0"
    },
    "description": "GitHub command line tools.",
    "devDependencies": {
        "babel": "^5.8",
        "gulp": "^3.9.0",
        "gulp-complexity": "^0.3.2",
        "gulp-istanbul": "^0.10.2",
        "gulp-jscs": "^3.0.2",
        "gulp-jshint": "^1.12.0",
        "gulp-mocha": "^2.1.3",
        "jshint-stylish": "^2.0.1",
        "plato": "^1.5.0",
        "rewire": "^2.3.4",
        "run-sequence": "^1.1.4"
    },
    "directories": {},
    "dist": {
        "shasum": "115e64a2748a0fedef57b1a68f1c5175980a86c2",
        "tarball": "https://registry.npmjs.org/gh/-/gh-1.12.8.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "10205cc07abbccc6c18ccf5c976da3a5ac0913f7",
    "homepage": "http://nodegh.io",
    "keywords": [
        "git",
        "github",
        "external",
        "commands",
        "helpers"
    ],
    "license": "BSD-3-Clause",
    "maintainers": [
        {
            "name": "eduardolundgren",
            "email": "eduardolundgren@gmail.com"
        },
        {
            "name": "zenorocha",
            "email": "zno.rocha@gmail.com"
        },
        {
            "name": "henvic",
            "email": "henriquevicente@gmail.com"
        }
    ],
    "name": "gh",
    "optionalDependencies": {},
    "preferGlobal": "true",
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/node-gh/gh.git"
    },
    "scripts": {
        "ci": "gulp ci",
        "postpublish": "sh postpublish.sh",
        "prepublish": "sh prepublish.sh",
        "test": "gulp test"
    },
    "trackingCode": "UA-58265773-2",
    "version": "1.12.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gh](#apidoc.module.gh)
1.  [function <span class="apidocSignatureSpan">gh.</span>cmd_anonymizer (commandDetails, redaction)](#apidoc.element.gh.cmd_anonymizer)
1.  [function <span class="apidocSignatureSpan">gh.</span>rest_api_client (options)](#apidoc.element.gh.rest_api_client)
1.  object <span class="apidocSignatureSpan">gh.</span>base
1.  object <span class="apidocSignatureSpan">gh.</span>cmd
1.  object <span class="apidocSignatureSpan">gh.</span>cmd_anonymizer.prototype
1.  object <span class="apidocSignatureSpan">gh.</span>configs
1.  object <span class="apidocSignatureSpan">gh.</span>exec
1.  object <span class="apidocSignatureSpan">gh.</span>git
1.  object <span class="apidocSignatureSpan">gh.</span>hooks
1.  object <span class="apidocSignatureSpan">gh.</span>logger
1.  object <span class="apidocSignatureSpan">gh.</span>rest_api_client.prototype
1.  object <span class="apidocSignatureSpan">gh.</span>tracker

#### [module gh.base](#apidoc.module.gh.base)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>asyncReadPackages (callback)](#apidoc.element.gh.base.asyncReadPackages)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>checkVersion ()](#apidoc.element.gh.base.checkVersion)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>clone (o)](#apidoc.element.gh.base.clone)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>expandAliases (options)](#apidoc.element.gh.base.expandAliases)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>find (filepath, opt_pattern)](#apidoc.element.gh.base.find)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>getConfig (opt_plugin)](#apidoc.element.gh.base.getConfig)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>getUser ()](#apidoc.element.gh.base.getUser)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>load ()](#apidoc.element.gh.base.load)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>notifyVersion (pkg)](#apidoc.element.gh.base.notifyVersion)
1.  [function <span class="apidocSignatureSpan">gh.base.</span>writeGlobalConfig (jsonPath, value)](#apidoc.element.gh.base.writeGlobalConfig)

#### [module gh.cmd](#apidoc.module.gh.cmd)
1.  [function <span class="apidocSignatureSpan">gh.cmd.</span>run ()](#apidoc.element.gh.cmd.run)
1.  [function <span class="apidocSignatureSpan">gh.cmd.</span>setUp ()](#apidoc.element.gh.cmd.setUp)

#### [module gh.cmd_anonymizer](#apidoc.module.gh.cmd_anonymizer)
1.  [function <span class="apidocSignatureSpan">gh.</span>cmd_anonymizer (commandDetails, redaction)](#apidoc.element.gh.cmd_anonymizer.cmd_anonymizer)

#### [module gh.cmd_anonymizer.prototype](#apidoc.module.gh.cmd_anonymizer.prototype)
1.  [function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>classify (word)](#apidoc.element.gh.cmd_anonymizer.prototype.classify)
1.  [function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>extractArgument (word)](#apidoc.element.gh.cmd_anonymizer.prototype.extractArgument)
1.  [function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>isOptionValue (option, value)](#apidoc.element.gh.cmd_anonymizer.prototype.isOptionValue)
1.  [function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>isValueInOptions (options, value)](#apidoc.element.gh.cmd_anonymizer.prototype.isValueInOptions)
1.  [function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>resolve (cmd)](#apidoc.element.gh.cmd_anonymizer.prototype.resolve)
1.  [function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>resolveToString (cmd)](#apidoc.element.gh.cmd_anonymizer.prototype.resolveToString)

#### [module gh.configs](#apidoc.module.gh.configs)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>addPluginConfig (config, plugin)](#apidoc.element.gh.configs.addPluginConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>createGlobalConfig ()](#apidoc.element.gh.configs.createGlobalConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getConfig (opt_plugin)](#apidoc.element.gh.configs.getConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getGlobalConfig (opt_plugin)](#apidoc.element.gh.configs.getGlobalConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getGlobalConfigPath ()](#apidoc.element.gh.configs.getGlobalConfigPath)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getNodeModulesGlobalPath ()](#apidoc.element.gh.configs.getNodeModulesGlobalPath)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getPlugin (plugin)](#apidoc.element.gh.configs.getPlugin)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getPluginBasename (plugin)](#apidoc.element.gh.configs.getPluginBasename)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getPluginPath (plugin)](#apidoc.element.gh.configs.getPluginPath)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getPlugins ()](#apidoc.element.gh.configs.getPlugins)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getProjectConfigPath ()](#apidoc.element.gh.configs.getProjectConfigPath)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>getUserHomePath ()](#apidoc.element.gh.configs.getUserHomePath)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>isPluginIgnored (plugin)](#apidoc.element.gh.configs.isPluginIgnored)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>removeGlobalConfig (key)](#apidoc.element.gh.configs.removeGlobalConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>saveJsonConfig (path, object)](#apidoc.element.gh.configs.saveJsonConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>writeGlobalConfig (jsonPath, value)](#apidoc.element.gh.configs.writeGlobalConfig)
1.  [function <span class="apidocSignatureSpan">gh.configs.</span>writeGlobalConfigCredentials (user, token)](#apidoc.element.gh.configs.writeGlobalConfigCredentials)
1.  string <span class="apidocSignatureSpan">gh.configs.</span>PLUGINS_PATH_KEY

#### [module gh.exec](#apidoc.module.gh.exec)
1.  [function <span class="apidocSignatureSpan">gh.exec.</span>execSync (cmd, options)](#apidoc.element.gh.exec.execSync)
1.  [function <span class="apidocSignatureSpan">gh.exec.</span>execSyncInteractiveStream (cmd, options)](#apidoc.element.gh.exec.execSyncInteractiveStream)
1.  [function <span class="apidocSignatureSpan">gh.exec.</span>spawnSync (cmd, args, options)](#apidoc.element.gh.exec.spawnSync)
1.  [function <span class="apidocSignatureSpan">gh.exec.</span>spawnSyncStream (cmd, args, options)](#apidoc.element.gh.exec.spawnSyncStream)

#### [module gh.git](#apidoc.module.gh.git)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>_merge (branch, type)](#apidoc.element.gh.git._merge)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>checkout (branch, newBranch)](#apidoc.element.gh.git.checkout)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>clone (url, folder)](#apidoc.element.gh.git.clone)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>countUserAdjacentCommits ()](#apidoc.element.gh.git.countUserAdjacentCommits)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>deleteBranch (branch)](#apidoc.element.gh.git.deleteBranch)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>fetch (repoUrl, headBranch, pullBranch)](#apidoc.element.gh.git.fetch)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>findRoot ()](#apidoc.element.gh.git.findRoot)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getCommitMessage (branch, number)](#apidoc.element.gh.git.getCommitMessage)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getConfig (key)](#apidoc.element.gh.git.getConfig)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getCurrentBranch ()](#apidoc.element.gh.git.getCurrentBranch)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getLastCommitMessage (branch)](#apidoc.element.gh.git.getLastCommitMessage)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getLastCommitSHA ()](#apidoc.element.gh.git.getLastCommitSHA)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getRemoteUrl (remote)](#apidoc.element.gh.git.getRemoteUrl)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getRepo (remote)](#apidoc.element.gh.git.getRepo)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getRepoFromRemoteURL (url)](#apidoc.element.gh.git.getRepoFromRemoteURL)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getUser (remote)](#apidoc.element.gh.git.getUser)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>getUserFromRemoteUrl (url)](#apidoc.element.gh.git.getUserFromRemoteUrl)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>merge (branch)](#apidoc.element.gh.git.merge)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>parseRemoteUrl (url)](#apidoc.element.gh.git.parseRemoteUrl)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>push (remote, branch)](#apidoc.element.gh.git.push)
1.  [function <span class="apidocSignatureSpan">gh.git.</span>rebase (branch)](#apidoc.element.gh.git.rebase)

#### [module gh.hooks](#apidoc.module.gh.hooks)
1.  [function <span class="apidocSignatureSpan">gh.hooks.</span>createContext (scope)](#apidoc.element.gh.hooks.createContext)
1.  [function <span class="apidocSignatureSpan">gh.hooks.</span>getHooksArrayFromPath_ (path, opt_config)](#apidoc.element.gh.hooks.getHooksArrayFromPath_)
1.  [function <span class="apidocSignatureSpan">gh.hooks.</span>getHooksFromPath (path)](#apidoc.element.gh.hooks.getHooksFromPath)
1.  [function <span class="apidocSignatureSpan">gh.hooks.</span>invoke (path, scope, opt_callback)](#apidoc.element.gh.hooks.invoke)
1.  [function <span class="apidocSignatureSpan">gh.hooks.</span>setupPlugins_ (context, setupFn, opt_callback)](#apidoc.element.gh.hooks.setupPlugins_)
1.  [function <span class="apidocSignatureSpan">gh.hooks.</span>wrapCommand_ (cmd, context, when)](#apidoc.element.gh.hooks.wrapCommand_)

#### [module gh.logger](#apidoc.module.gh.logger)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>applyReplacements (output, replaceMap)](#apidoc.element.gh.logger.applyReplacements)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>compileTemplate (source, map)](#apidoc.element.gh.logger.compileTemplate)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>debug ()](#apidoc.element.gh.logger.debug)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>error ()](#apidoc.element.gh.logger.error)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>getDuration (start, opt_end)](#apidoc.element.gh.logger.getDuration)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>getErrorMessage (err)](#apidoc.element.gh.logger.getErrorMessage)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>insane ()](#apidoc.element.gh.logger.insane)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>log ()](#apidoc.element.gh.logger.log)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>logTemplate (source, map)](#apidoc.element.gh.logger.logTemplate)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>logTemplateFile (file, map)](#apidoc.element.gh.logger.logTemplateFile)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>registerHelper (name, callback)](#apidoc.element.gh.logger.registerHelper)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>registerHelpers_ ()](#apidoc.element.gh.logger.registerHelpers_)
1.  [function <span class="apidocSignatureSpan">gh.logger.</span>warn ()](#apidoc.element.gh.logger.warn)
1.  object <span class="apidocSignatureSpan">gh.logger.</span>colors

#### [module gh.rest_api_client](#apidoc.module.gh.rest_api_client)
1.  [function <span class="apidocSignatureSpan">gh.</span>rest_api_client (options)](#apidoc.element.gh.rest_api_client.rest_api_client)

#### [module gh.rest_api_client.prototype](#apidoc.module.gh.rest_api_client.prototype)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>authorize (p)](#apidoc.element.gh.rest_api_client.prototype.authorize)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>delete ()](#apidoc.element.gh.rest_api_client.prototype.delete)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>encode ()](#apidoc.element.gh.rest_api_client.prototype.encode)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>get ()](#apidoc.element.gh.rest_api_client.prototype.get)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>post ()](#apidoc.element.gh.rest_api_client.prototype.post)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>put ()](#apidoc.element.gh.rest_api_client.prototype.put)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>request (method, path, params)](#apidoc.element.gh.rest_api_client.prototype.request)
1.  [function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>url (pathname, query)](#apidoc.element.gh.rest_api_client.prototype.url)
1.  object <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>DEFAULT_CONFIG

#### [module gh.tracker](#apidoc.module.gh.tracker)
1.  [function <span class="apidocSignatureSpan">gh.tracker.</span>resolveCommand (cmd, commandDetails)](#apidoc.element.gh.tracker.resolveCommand)
1.  [function <span class="apidocSignatureSpan">gh.tracker.</span>trackCommand (cmd, commandDetails)](#apidoc.element.gh.tracker.trackCommand)
1.  number <span class="apidocSignatureSpan">gh.tracker.</span>_permissionTimeout
1.  object <span class="apidocSignatureSpan">gh.tracker.</span>_queue
1.  object <span class="apidocSignatureSpan">gh.tracker.</span>config
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>appVersion
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>nodeVersion
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>os
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>packageName
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>packageVersion
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>trackingCode
1.  string <span class="apidocSignatureSpan">gh.tracker.</span>trackingProvider



# <a name="apidoc.module.gh"></a>[module gh](#apidoc.module.gh)

#### <a name="apidoc.element.gh.cmd_anonymizer"></a>[function <span class="apidocSignatureSpan">gh.</span>cmd_anonymizer (commandDetails, redaction)](#apidoc.element.gh.cmd_anonymizer)
- description and source-code
```javascript
function CmdAnonymizer(commandDetails, redaction) {
    this.last = null;
    this.invoked = [];
    this.redaction = redaction;
    this.options = commandDetails.options;
    this.shorthands = commandDetails.shorthands;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.rest_api_client"></a>[function <span class="apidocSignatureSpan">gh.</span>rest_api_client (options)](#apidoc.element.gh.rest_api_client)
- description and source-code
```javascript
function RestApiClient(options) {
    _classCallCheck(this, RestApiClient);

    options = lodash.merge(this.DEFAULT_CONFIG, options);
    this.options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gh.base"></a>[module gh.base](#apidoc.module.gh.base)

#### <a name="apidoc.element.gh.base.asyncReadPackages"></a>[function <span class="apidocSignatureSpan">gh.base.</span>asyncReadPackages (callback)](#apidoc.element.gh.base.asyncReadPackages)
- description and source-code
```javascript
asyncReadPackages = function (callback) {
    function async(err, data) {
        if (err) {
            throw err;
        }

        callback(JSON.parse(data));
    }

    fs.readFile(path.join(__dirname, '..', 'package.json'), async);

    configs.getPlugins().forEach(function (plugin) {
        fs.readFile(path.join(
            configs.getNodeModulesGlobalPath(), plugin, 'package.json'), async);
    });
}
```
- example usage
```shell
...
    tracker.track(track);

    notifier.notify();
}
};

exports.checkVersion = function () {
exports.asyncReadPackages(exports.notifyVersion);
};

exports.expandAliases = function (options) {
var config = configs.getConfig();

if (config.alias) {
    options.fwd = config.alias[options.fwd] || options.fwd;
...
```

#### <a name="apidoc.element.gh.base.checkVersion"></a>[function <span class="apidocSignatureSpan">gh.base.</span>checkVersion ()](#apidoc.element.gh.base.checkVersion)
- description and source-code
```javascript
checkVersion = function () {
    exports.asyncReadPackages(exports.notifyVersion);
}
```
- example usage
```shell
...
operations = [],
options,
parsed = nopt(process.argv),
remain = parsed.argv.remain,
cooked = parsed.argv.cooked;

    operations.push(function (callback) {
base.checkVersion();

if (tracker.optOut !== undefined) {
    callback();
    return;
}

tracker.askPermission(null, function () {
...
```

#### <a name="apidoc.element.gh.base.clone"></a>[function <span class="apidocSignatureSpan">gh.base.</span>clone (o)](#apidoc.element.gh.base.clone)
- description and source-code
```javascript
clone = function (o) {
    return JSON.parse(JSON.stringify(o));
}
```
- example usage
```shell
...

        // Try to retrieve iterative values from iterative option key,
        // e.g. option['number'] === [1,2,3]. If iterative option key is not
        // present, assume [undefined] in order to initialize the loop.
        iterativeValues = options[iterative] || [undefined];

        iterativeValues.forEach(function (value) {
options = base.clone(options);

// Value can be undefined when the command doesn't have a iterative
// option.
options[iterative] = value;

invokePayload(options, Command, cooked, remain);
...
```

#### <a name="apidoc.element.gh.base.expandAliases"></a>[function <span class="apidocSignatureSpan">gh.base.</span>expandAliases (options)](#apidoc.element.gh.base.expandAliases)
- description and source-code
```javascript
expandAliases = function (options) {
    var config = configs.getConfig();

    if (config.alias) {
        options.fwd = config.alias[options.fwd] || options.fwd;
        options.submit = config.alias[options.submit] || options.submit;
        options.user = config.alias[options.user] || options.user;
    }
}
```
- example usage
```shell
...
        options.user = options.remoteUser || options.loggedUser;
    }
}

options.repo = options.repo || git.getRepoFromRemoteURL(remoteUrl);
options.currentBranch = options.currentBranch || git.getCurrentBranch();

base.expandAliases(options);
options.github_host = config.github_host;
options.github_gist_host = config.github_gist_host;

// Try to retrieve iterative values from iterative option key,
// e.g. option['number'] === [1,2,3]. If iterative option key is not
// present, assume [undefined] in order to initialize the loop.
iterativeValues = options[iterative] || [undefined];
...
```

#### <a name="apidoc.element.gh.base.find"></a>[function <span class="apidocSignatureSpan">gh.base.</span>find (filepath, opt_pattern)](#apidoc.element.gh.base.find)
- description and source-code
```javascript
find = function (filepath, opt_pattern) {
    return fs.readdirSync(filepath).filter(function (file) {
        return (opt_pattern || /.*/).test(file);
    });
}
```
- example usage
```shell
...
    commandDir = path.join(__dirname, 'cmds');
    commandPath = path.join(commandDir, name + '.js');

    if (fs.existsSync(commandPath)) {
        Command = require(commandPath).Impl;
    }
    else {
        commandFiles = base.find(commandDir, /\.js$/i);
        commandFiles.every(function (file) {
commandPath = path.join(commandDir, file);
Command = require(commandPath).Impl;

if (Command.DETAILS.alias === name) {
    return false;
}
...
```

#### <a name="apidoc.element.gh.base.getConfig"></a>[function <span class="apidocSignatureSpan">gh.base.</span>getConfig (opt_plugin)](#apidoc.element.gh.base.getConfig)
- description and source-code
```javascript
getConfig = function (opt_plugin) {
    var config = cache[opt_plugin];

    if (!config) {
        config = getConfig(opt_plugin);
        cache[opt_plugin] = config;
    }

    var protocol = config.api.protocol + '://',
        is_enterprise = (config.api.host !== 'api.github.com');

    if (config.github_host === undefined) {
        config.github_host = protocol + (is_enterprise ? config.api.host : 'github.com') + '/';
    }
    if (config.github_gist_host === undefined) {
        config.github_gist_host = protocol + (is_enterprise ? config.api.host + '/gist' : 'gist.github.com') + '/';
    }

    return config;
}
```
- example usage
```shell
...
exports.clone = function (o) {
return JSON.parse(JSON.stringify(o));
};

// -- Utils --------------------------------------------------------------------

exports.load = function () {
var config = configs.getConfig();

exports.github = new Github({
    debug: false,
    host: config.api.host,
    protocol: config.api.protocol,
    version: config.api.version,
    pathPrefix: config.api.pathPrefix
...
```

#### <a name="apidoc.element.gh.base.getUser"></a>[function <span class="apidocSignatureSpan">gh.base.</span>getUser ()](#apidoc.element.gh.base.getUser)
- description and source-code
```javascript
getUser = function () {
    return configs.getConfig().github_user;
}
```
- example usage
```shell
...
    async.series(operations, function () {
var iterativeValues,
    remoteUrl = git.getRemoteUrl(options.remote);

options.isTTY = {};
options.isTTY.in = Boolean(process.stdin.isTTY);
options.isTTY.out = Boolean(process.stdout.isTTY);
options.loggedUser = base.getUser();
options.remoteUser = git.getUserFromRemoteUrl(remoteUrl);

if (!options.user) {
    if (options.repo || options.all) {
        options.user = options.loggedUser;
    }
    else {
...
```

#### <a name="apidoc.element.gh.base.load"></a>[function <span class="apidocSignatureSpan">gh.base.</span>load ()](#apidoc.element.gh.base.load)
- description and source-code
```javascript
load = function () {
    var config = configs.getConfig();

    exports.github = new Github({
        debug: false,
        host: config.api.host,
        protocol: config.api.protocol,
        version: config.api.version,
        pathPrefix: config.api.pathPrefix
    });
}
```
- example usage
```shell
...
};

exports.run = function () {
if (!fs.existsSync(configs.getUserHomePath())) {
    configs.createGlobalConfig();
}

base.load();
configs.getConfig();

// If configs.PLUGINS_PATH_KEY is undefined, try to cache it before proceeding.
if (configs.getConfig()[configs.PLUGINS_PATH_KEY] === undefined) {
    configs.getNodeModulesGlobalPath();
}
...
```

#### <a name="apidoc.element.gh.base.notifyVersion"></a>[function <span class="apidocSignatureSpan">gh.base.</span>notifyVersion (pkg)](#apidoc.element.gh.base.notifyVersion)
- description and source-code
```javascript
notifyVersion = function (pkg) {
    var notifier = updateNotifier({pkg: pkg}),
        update,
        track = 'notify/';

    if (notifier.update) {
        update = notifier.update;

        track += update.name + '/' + update.latest + '/from/' + update.current;

        tracker.track(track);

        notifier.notify();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.base.writeGlobalConfig"></a>[function <span class="apidocSignatureSpan">gh.base.</span>writeGlobalConfig (jsonPath, value)](#apidoc.element.gh.base.writeGlobalConfig)
- description and source-code
```javascript
writeGlobalConfig = function (jsonPath, value) {
    var config = exports.getGlobalConfig(),
        i,
        output,
        path,
        pathLen;

    path = jsonPath.split('.');
    output = config;

    for (i = 0, pathLen = path.length; i < pathLen; i++) {
        output[path[i]] = config[path[i]] || (i + 1 === pathLen ? value : {});
        output = output[path[i]];
    }

    exports.saveJsonConfig(exports.getUserHomePath(), config);
    cache = {};
}
```
- example usage
```shell
...
    path = exports.getConfig()[PLUGINS_PATH_KEY];

if (path === undefined) {
    result = exec.spawnSync('npm', ['root', '-g']);

    if (result.stdout) {
        path = result.stdout;
        exports.writeGlobalConfig(PLUGINS_PATH_KEY, path);
    }
    else {
        logger.warn('Can\'t resolve plugins directory path.');
    }
}

return path;
...
```



# <a name="apidoc.module.gh.cmd"></a>[module gh.cmd](#apidoc.module.gh.cmd)

#### <a name="apidoc.element.gh.cmd.run"></a>[function <span class="apidocSignatureSpan">gh.cmd.</span>run ()](#apidoc.element.gh.cmd.run)
- description and source-code
```javascript
run = function () {
    if (!fs.existsSync(configs.getUserHomePath())) {
        configs.createGlobalConfig();
    }

    base.load();
    configs.getConfig();

    // If configs.PLUGINS_PATH_KEY is undefined, try to cache it before proceeding.
    if (configs.getConfig()[configs.PLUGINS_PATH_KEY] === undefined) {
        configs.getNodeModulesGlobalPath();
    }

    try {
        process.env.GH_PATH = path.join(__dirname, '../');

        this.setUp();
    } catch (e) {
        tracker.track('error');
        console.error(e.stack || e);
    }

}
```
- example usage
```shell
...

            // Value can be undefined when the command doesn't have a iterative
            // option.
            options[iterative] = value;

            invokePayload(options, Command, cooked, remain);

            new Command(options).run();

            tracker.trackCommand(options.argv.original, Command.DETAILS);
        });
    });
};

exports.run = function () {
...
```

#### <a name="apidoc.element.gh.cmd.setUp"></a>[function <span class="apidocSignatureSpan">gh.cmd.</span>setUp ()](#apidoc.element.gh.cmd.setUp)
- description and source-code
```javascript
setUp = function () {
    var Command,
        iterative,
        operations = [],
        options,
        parsed = nopt(process.argv),
        remain = parsed.argv.remain,
        cooked = parsed.argv.cooked;

    operations.push(function (callback) {
        base.checkVersion();

        if (tracker.optOut !== undefined) {
            callback();
            return;
        }

        tracker.askPermission(null, function () {
            callback();
        });
    });

    operations.push(function (callback) {
        var module = remain[0];

        if (cooked[0] === '--version' || cooked[0] === '-v') {
            module = 'version';
        }
        else if (!remain.length ||
            (cooked.indexOf('-h') >= 0) ||
            (cooked.indexOf('--help') >= 0)) {
            module = 'help';
        }

        Command = loadCommand(module);

        if (!Command) {
            tracker.trackCommand(remain);
            logger.error('Command not found');
            return;
        }

        options = nopt(
            Command.DETAILS.options,
            Command.DETAILS.shorthands, process.argv, 2);

        iterative = Command.DETAILS.iterative;

        cooked = options.argv.cooked;
        remain = options.argv.remain;

        options.number = options.number || [remain[1]];
        options.remote = options.remote || config.default_remote;

        if (module === 'help') {
            callback();
        }
        else {
            User.login(callback);
        }
    });

    async.series(operations, function () {
        var iterativeValues,
            remoteUrl = git.getRemoteUrl(options.remote);

        options.isTTY = {};
        options.isTTY.in = Boolean(process.stdin.isTTY);
        options.isTTY.out = Boolean(process.stdout.isTTY);
        options.loggedUser = base.getUser();
        options.remoteUser = git.getUserFromRemoteUrl(remoteUrl);

        if (!options.user) {
            if (options.repo || options.all) {
                options.user = options.loggedUser;
            }
            else {
                options.user = options.remoteUser || options.loggedUser;
            }
        }

        options.repo = options.repo || git.getRepoFromRemoteURL(remoteUrl);
        options.currentBranch = options.currentBranch || git.getCurrentBranch();

        base.expandAliases(options);
        options.github_host = config.github_host;
        options.github_gist_host = config.github_gist_host;

        // Try to retrieve iterative values from iterative option key,
        // e.g. option['number'] === [1,2,3]. If iterative option key is not
        // present, assume [undefined] in order to initialize the loop.
        iterativeValues = options[iterative] || [undefined];

        iterativeValues.forEach(function (value) {
            options = base.clone(options);

            // Value can be undefined when the command doesn't have a iterative
            // option.
            options[iterative] = value;

            invokePayload(options, Command, cooked, remain);

            new Command(options).run();

            tracker.trackCommand(options.argv.original, Command.DETAILS);
        });
    });
}
```
- example usage
```shell
...
    if (configs.getConfig()[configs.PLUGINS_PATH_KEY] === undefined) {
        configs.getNodeModulesGlobalPath();
    }

    try {
        process.env.GH_PATH = path.join(__dirname, '../');

        this.setUp();
    } catch (e) {
        tracker.track('error');
        console.error(e.stack || e);
    }

};
...
```



# <a name="apidoc.module.gh.cmd_anonymizer"></a>[module gh.cmd_anonymizer](#apidoc.module.gh.cmd_anonymizer)

#### <a name="apidoc.element.gh.cmd_anonymizer.cmd_anonymizer"></a>[function <span class="apidocSignatureSpan">gh.</span>cmd_anonymizer (commandDetails, redaction)](#apidoc.element.gh.cmd_anonymizer.cmd_anonymizer)
- description and source-code
```javascript
function CmdAnonymizer(commandDetails, redaction) {
    this.last = null;
    this.invoked = [];
    this.redaction = redaction;
    this.options = commandDetails.options;
    this.shorthands = commandDetails.shorthands;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gh.cmd_anonymizer.prototype"></a>[module gh.cmd_anonymizer.prototype](#apidoc.module.gh.cmd_anonymizer.prototype)

#### <a name="apidoc.element.gh.cmd_anonymizer.prototype.classify"></a>[function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>classify (word)](#apidoc.element.gh.cmd_anonymizer.prototype.classify)
- description and source-code
```javascript
classify = function (word) {
    var arg = this.extractArgument(word),
        whitelist = ['verbose', 'no-hooks'];

    if (whitelist.indexOf(arg) === 0) {
        this.invoked.push(word);
        this.last = arg;
        return;
    }

    if (this.shorthands && this.shorthands[arg]) {
        this.invoked.push(word);
        this.last = this.shorthands[arg];
        return;
    }

    if (this.options && this.options[arg]) {
        this.invoked.push(word);
        this.last = arg;
        return;
    }

    if (this.options && this.isValueInOptions(this.last, word)) {
        this.invoked.push(word);
        this.last = undefined;
        return;
    }

    if (this.options && this.options[this.last] instanceof Array &&
        this.options[this.last].indexOf(word) !== -1) {
        this.invoked.push(word);
        this.last = undefined;
        return;
    }

    this.invoked.push(this.redaction);
    this.last = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.cmd_anonymizer.prototype.extractArgument"></a>[function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>extractArgument (word)](#apidoc.element.gh.cmd_anonymizer.prototype.extractArgument)
- description and source-code
```javascript
extractArgument = function (word) {
    return word.replace(/-{0,2}/, '');
}
```
- example usage
```shell
...

CmdAnonymizer.prototype.isValueInOptions = function (options, value) {
if (!(options instanceof Array)) {
    return this.isOptionValue(options, value);
}

return options.some(function (each) {
    return this.isOptionValue(this.extractArgument(each), value);
}, this);
};

CmdAnonymizer.prototype.classify = function (word) {
var arg = this.extractArgument(word),
    whitelist = ['verbose', 'no-hooks'];
...
```

#### <a name="apidoc.element.gh.cmd_anonymizer.prototype.isOptionValue"></a>[function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>isOptionValue (option, value)](#apidoc.element.gh.cmd_anonymizer.prototype.isOptionValue)
- description and source-code
```javascript
isOptionValue = function (option, value) {
    var choice = this.options[option],
        booleans = ['true', 'false'];

    return ((choice instanceof Array && choice.indexOf(value) !== -1) ||
        (choice === Boolean && booleans.indexOf(value.toLowerCase()) !== -1) ||
        (typeof choice === 'string' && choice === value));
}
```
- example usage
```shell
...
    return ((choice instanceof Array && choice.indexOf(value) !== -1) ||
        (choice === Boolean && booleans.indexOf(value.toLowerCase()) !== -1) ||
        (typeof choice === 'string' && choice === value));
};

CmdAnonymizer.prototype.isValueInOptions = function (options, value) {
    if (!(options instanceof Array)) {
        return this.isOptionValue(options, value);
    }

    return options.some(function (each) {
        return this.isOptionValue(this.extractArgument(each), value);
    }, this);
};
...
```

#### <a name="apidoc.element.gh.cmd_anonymizer.prototype.isValueInOptions"></a>[function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>isValueInOptions (options, value)](#apidoc.element.gh.cmd_anonymizer.prototype.isValueInOptions)
- description and source-code
```javascript
isValueInOptions = function (options, value) {
    if (!(options instanceof Array)) {
        return this.isOptionValue(options, value);
    }

    return options.some(function (each) {
        return this.isOptionValue(this.extractArgument(each), value);
    }, this);
}
```
- example usage
```shell
...

if (this.options && this.options[arg]) {
    this.invoked.push(word);
    this.last = arg;
    return;
}

if (this.options && this.isValueInOptions(this.last, word)) {
    this.invoked.push(word);
    this.last = undefined;
    return;
}

if (this.options && this.options[this.last] instanceof Array &&
    this.options[this.last].indexOf(word) !== -1) {
...
```

#### <a name="apidoc.element.gh.cmd_anonymizer.prototype.resolve"></a>[function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>resolve (cmd)](#apidoc.element.gh.cmd_anonymizer.prototype.resolve)
- description and source-code
```javascript
resolve = function (cmd) {
    // quasi-strict white list approach (best-effort)

    this.invoked.push(cmd.shift());

    cmd.forEach(this.classify, this);

    return this.invoked;
}
```
- example usage
```shell
...

    cmd.forEach(this.classify, this);

    return this.invoked;
};

CmdAnonymizer.prototype.resolveToString = function (cmd) {
    return this.resolve(cmd).join(' ');
};

module.exports = CmdAnonymizer;
...
```

#### <a name="apidoc.element.gh.cmd_anonymizer.prototype.resolveToString"></a>[function <span class="apidocSignatureSpan">gh.cmd_anonymizer.prototype.</span>resolveToString (cmd)](#apidoc.element.gh.cmd_anonymizer.prototype.resolveToString)
- description and source-code
```javascript
resolveToString = function (cmd) {
    return this.resolve(cmd).join(' ');
}
```
- example usage
```shell
...

    if (!commandDetails) {
        return cmd.join(' ').replace(/\w+/g, redaction);
    }

    cmdAnonymizer = new CmdAnonymizer(commandDetails, redaction);

    return cmdAnonymizer.resolveToString(cmd);
};

tracker.trackCommand = function (cmd, commandDetails) {
    var tracking = pkg.name + ' ' + this.resolveCommand(cmd, commandDetails);

    this.track(tracking.replace(/ /g, '%20'));
};
...
```



# <a name="apidoc.module.gh.configs"></a>[module gh.configs](#apidoc.module.gh.configs)

#### <a name="apidoc.element.gh.configs.addPluginConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>addPluginConfig (config, plugin)](#apidoc.element.gh.configs.addPluginConfig)
- description and source-code
```javascript
addPluginConfig = function (config, plugin) {
    var pluginConfig,
        userConfig;

    try {
        // Always use the plugin name without prefix. To be safe removing "gh-"
        // prefix from passed plugin.
        plugin = exports.getPluginBasename(plugin || process.env.NODEGH_PLUGIN);

        pluginConfig = require(path.join(
            exports.getNodeModulesGlobalPath(), 'gh-' + plugin, 'gh-plugin.json'));

        // Merge default plugin configuration with the user's.
        userConfig = config.plugins[plugin] || {};

        Object.keys(userConfig).forEach(function (key) {
            pluginConfig[key] = userConfig[key];
        });

        config.plugins[plugin] = pluginConfig;
    }
    catch (e) {
        if (e.code !== 'MODULE_NOT_FOUND') {
            throw e;
        }
    }
}
```
- example usage
```shell
...

    Object.keys(userConfig).forEach(function (key) {
        config[key] = userConfig[key];
    });

    if (opt_plugin) {
        exports.getPlugins().forEach(function (plugin) {
            exports.addPluginConfig(config, plugin);
        });
    }

    return config;
};

exports.getGlobalConfigPath = function () {
...
```

#### <a name="apidoc.element.gh.configs.createGlobalConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>createGlobalConfig ()](#apidoc.element.gh.configs.createGlobalConfig)
- description and source-code
```javascript
createGlobalConfig = function () {
    exports.saveJsonConfig(exports.getUserHomePath(),
        JSON.parse(fs.readFileSync(exports.getGlobalConfigPath()))
    );
    cache = {};
}
```
- example usage
```shell
...
        tracker.trackCommand(options.argv.original, Command.DETAILS);
    });
});
};

exports.run = function () {
if (!fs.existsSync(configs.getUserHomePath())) {
    configs.createGlobalConfig();
}

base.load();
configs.getConfig();

// If configs.PLUGINS_PATH_KEY is undefined, try to cache it before proceeding.
if (configs.getConfig()[configs.PLUGINS_PATH_KEY] === undefined) {
...
```

#### <a name="apidoc.element.gh.configs.getConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getConfig (opt_plugin)](#apidoc.element.gh.configs.getConfig)
- description and source-code
```javascript
getConfig = function (opt_plugin) {
    var config = cache[opt_plugin];

    if (!config) {
        config = getConfig(opt_plugin);
        cache[opt_plugin] = config;
    }

    var protocol = config.api.protocol + '://',
        is_enterprise = (config.api.host !== 'api.github.com');

    if (config.github_host === undefined) {
        config.github_host = protocol + (is_enterprise ? config.api.host : 'github.com') + '/';
    }
    if (config.github_gist_host === undefined) {
        config.github_gist_host = protocol + (is_enterprise ? config.api.host + '/gist' : 'gist.github.com') + '/';
    }

    return config;
}
```
- example usage
```shell
...
exports.clone = function (o) {
return JSON.parse(JSON.stringify(o));
};

// -- Utils --------------------------------------------------------------------

exports.load = function () {
var config = configs.getConfig();

exports.github = new Github({
    debug: false,
    host: config.api.host,
    protocol: config.api.protocol,
    version: config.api.version,
    pathPrefix: config.api.pathPrefix
...
```

#### <a name="apidoc.element.gh.configs.getGlobalConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getGlobalConfig (opt_plugin)](#apidoc.element.gh.configs.getGlobalConfig)
- description and source-code
```javascript
getGlobalConfig = function (opt_plugin) {
    var config,
        configPath,
        userConfig;

    configPath = exports.getUserHomePath();

    if (!fs.existsSync(configPath)) {
        exports.createGlobalConfig();
    }

    config = JSON.parse(fs.readFileSync(exports.getGlobalConfigPath()));
    userConfig = JSON.parse(fs.readFileSync(configPath));

    Object.keys(userConfig).forEach(function (key) {
        config[key] = userConfig[key];
    });

    if (opt_plugin) {
        exports.getPlugins().forEach(function (plugin) {
            exports.addPluginConfig(config, plugin);
        });
    }

    return config;
}
```
- example usage
```shell
...
};

exports.getUserHomePath = function () {
    return userhome('.gh.json');
};

function getConfig(opt_plugin) {
    var globalConfig = exports.getGlobalConfig(opt_plugin),
projectConfig,
result = {};

    try {
projectConfig = JSON.parse(fs.readFileSync(exports.getProjectConfigPath()));

Object.keys(globalConfig).forEach(function (key) {
...
```

#### <a name="apidoc.element.gh.configs.getGlobalConfigPath"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getGlobalConfigPath ()](#apidoc.element.gh.configs.getGlobalConfigPath)
- description and source-code
```javascript
getGlobalConfigPath = function () {
    return path.join(__dirname, '../', 'default.gh.json');
}
```
- example usage
```shell
...

configPath = exports.getUserHomePath();

if (!fs.existsSync(configPath)) {
    exports.createGlobalConfig();
}

config = JSON.parse(fs.readFileSync(exports.getGlobalConfigPath()));
userConfig = JSON.parse(fs.readFileSync(configPath));

Object.keys(userConfig).forEach(function (key) {
    config[key] = userConfig[key];
});

if (opt_plugin) {
...
```

#### <a name="apidoc.element.gh.configs.getNodeModulesGlobalPath"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getNodeModulesGlobalPath ()](#apidoc.element.gh.configs.getNodeModulesGlobalPath)
- description and source-code
```javascript
getNodeModulesGlobalPath = function () {
    var result,
        path = exports.getConfig()[PLUGINS_PATH_KEY];

    if (path === undefined) {
        result = exec.spawnSync('npm', ['root', '-g']);

        if (result.stdout) {
            path = result.stdout;
            exports.writeGlobalConfig(PLUGINS_PATH_KEY, path);
        }
        else {
            logger.warn('Can\'t resolve plugins directory path.');
        }
    }

    return path;
}
```
- example usage
```shell
...
    callback(JSON.parse(data));
}

fs.readFile(path.join(__dirname, '..', 'package.json'), async);

configs.getPlugins().forEach(function (plugin) {
    fs.readFile(path.join(
        configs.getNodeModulesGlobalPath(), plugin, 'package.json'), async);
});
};

exports.notifyVersion = function (pkg) {
var notifier = updateNotifier({pkg: pkg}),
    update,
    track = 'notify/';
...
```

#### <a name="apidoc.element.gh.configs.getPlugin"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getPlugin (plugin)](#apidoc.element.gh.configs.getPlugin)
- description and source-code
```javascript
getPlugin = function (plugin) {
    plugin = exports.getPluginBasename(plugin);

    return require(exports.getPluginPath('gh-' + plugin));
}
```
- example usage
```shell
...
function loadCommand(name) {
    var Command = findCommand(name),
plugin;

    // If command was not found, check if it is registered as a plugin.
    if (!Command) {
try {
    plugin = configs.getPlugin(name);
}
catch(e) {
    return null;
}

Command = plugin.Impl;
...
```

#### <a name="apidoc.element.gh.configs.getPluginBasename"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getPluginBasename (plugin)](#apidoc.element.gh.configs.getPluginBasename)
- description and source-code
```javascript
getPluginBasename = function (plugin) {
    return plugin && plugin.replace('gh-', '');
}
```
- example usage
```shell
...
exports.addPluginConfig = function (config, plugin) {
    var pluginConfig,
userConfig;

    try {
// Always use the plugin name without prefix. To be safe removing "gh-"
// prefix from passed plugin.
plugin = exports.getPluginBasename(plugin || process.env.NODEGH_PLUGIN);

pluginConfig = require(path.join(
    exports.getNodeModulesGlobalPath(), 'gh-' + plugin, 'gh-plugin.json'));

// Merge default plugin configuration with the user's.
userConfig = config.plugins[plugin] || {};
...
```

#### <a name="apidoc.element.gh.configs.getPluginPath"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getPluginPath (plugin)](#apidoc.element.gh.configs.getPluginPath)
- description and source-code
```javascript
getPluginPath = function (plugin) {
    return fs.realpathSync(which.sync(plugin));
}
```
- example usage
```shell
...

    return plugins;
};

exports.getPlugin = function (plugin) {
    plugin = exports.getPluginBasename(plugin);

    return require(exports.getPluginPath('gh-' + plugin));
};

exports.getPluginPath = function (plugin) {
    return fs.realpathSync(which.sync(plugin));
};

exports.getPluginBasename = function (plugin) {
...
```

#### <a name="apidoc.element.gh.configs.getPlugins"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getPlugins ()](#apidoc.element.gh.configs.getPlugins)
- description and source-code
```javascript
getPlugins = function () {
    if (!plugins) {
        plugins = getPlugins();
    }

    return plugins;
}
```
- example usage
```shell
...
    }

    callback(JSON.parse(data));
}

fs.readFile(path.join(__dirname, '..', 'package.json'), async);

configs.getPlugins().forEach(function (plugin) {
    fs.readFile(path.join(
        configs.getNodeModulesGlobalPath(), plugin, 'package.json'), async);
});
};

exports.notifyVersion = function (pkg) {
var notifier = updateNotifier({pkg: pkg}),
...
```

#### <a name="apidoc.element.gh.configs.getProjectConfigPath"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getProjectConfigPath ()](#apidoc.element.gh.configs.getProjectConfigPath)
- description and source-code
```javascript
getProjectConfigPath = function () {
    return path.join(process.cwd(), '.gh.json');
}
```
- example usage
```shell
...

function getConfig(opt_plugin) {
    var globalConfig = exports.getGlobalConfig(opt_plugin),
projectConfig,
result = {};

    try {
projectConfig = JSON.parse(fs.readFileSync(exports.getProjectConfigPath()));

Object.keys(globalConfig).forEach(function (key) {
    result[key] = globalConfig[key];
});

Object.keys(projectConfig).forEach(function (key) {
    result[key] = projectConfig[key];
...
```

#### <a name="apidoc.element.gh.configs.getUserHomePath"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>getUserHomePath ()](#apidoc.element.gh.configs.getUserHomePath)
- description and source-code
```javascript
getUserHomePath = function () {
    return userhome('.gh.json');
}
```
- example usage
```shell
...

        tracker.trackCommand(options.argv.original, Command.DETAILS);
    });
});
};

exports.run = function () {
if (!fs.existsSync(configs.getUserHomePath())) {
    configs.createGlobalConfig();
}

base.load();
configs.getConfig();

// If configs.PLUGINS_PATH_KEY is undefined, try to cache it before proceeding.
...
```

#### <a name="apidoc.element.gh.configs.isPluginIgnored"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>isPluginIgnored (plugin)](#apidoc.element.gh.configs.isPluginIgnored)
- description and source-code
```javascript
isPluginIgnored = function (plugin) {
    if (exports.getConfig().ignored_plugins.indexOf(exports.getPluginBasename(plugin)) > -1) {
        return true;
    }

    return false;
}
```
- example usage
```shell
...
    // Second, search all installed plugins and load the hooks for each into
    // core hooks array.
    plugins.forEach(function (plugin) {
var pluginConfig;

plugin = configs.getPluginBasename(plugin);

if (config.plugins && !configs.isPluginIgnored(plugin)) {
    pluginConfig = config.plugins[plugin];

    if (pluginConfig) {
        pluginHooks = pluginHooks.concat(
            exports.getHooksArrayFromPath_(path, pluginConfig));
    }
}
...
```

#### <a name="apidoc.element.gh.configs.removeGlobalConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>removeGlobalConfig (key)](#apidoc.element.gh.configs.removeGlobalConfig)
- description and source-code
```javascript
removeGlobalConfig = function (key) {
    var config = exports.getGlobalConfig();

    delete config[key];

    exports.saveJsonConfig(exports.getUserHomePath(), config);
    cache = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.configs.saveJsonConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>saveJsonConfig (path, object)](#apidoc.element.gh.configs.saveJsonConfig)
- description and source-code
```javascript
saveJsonConfig = function (path, object) {
    var options = {
        mode: parseInt('0600', 8)
    };

    fs.writeFileSync(path, JSON.stringify(object, null, 4), options);
}
```
- example usage
```shell
...
};

exports.removeGlobalConfig = function (key) {
var config = exports.getGlobalConfig();

delete config[key];

exports.saveJsonConfig(exports.getUserHomePath(), config);
cache = {};
};

exports.createGlobalConfig = function () {
exports.saveJsonConfig(exports.getUserHomePath(),
    JSON.parse(fs.readFileSync(exports.getGlobalConfigPath()))
);
...
```

#### <a name="apidoc.element.gh.configs.writeGlobalConfig"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>writeGlobalConfig (jsonPath, value)](#apidoc.element.gh.configs.writeGlobalConfig)
- description and source-code
```javascript
writeGlobalConfig = function (jsonPath, value) {
    var config = exports.getGlobalConfig(),
        i,
        output,
        path,
        pathLen;

    path = jsonPath.split('.');
    output = config;

    for (i = 0, pathLen = path.length; i < pathLen; i++) {
        output[path[i]] = config[path[i]] || (i + 1 === pathLen ? value : {});
        output = output[path[i]];
    }

    exports.saveJsonConfig(exports.getUserHomePath(), config);
    cache = {};
}
```
- example usage
```shell
...
    path = exports.getConfig()[PLUGINS_PATH_KEY];

if (path === undefined) {
    result = exec.spawnSync('npm', ['root', '-g']);

    if (result.stdout) {
        path = result.stdout;
        exports.writeGlobalConfig(PLUGINS_PATH_KEY, path);
    }
    else {
        logger.warn('Can\'t resolve plugins directory path.');
    }
}

return path;
...
```

#### <a name="apidoc.element.gh.configs.writeGlobalConfigCredentials"></a>[function <span class="apidocSignatureSpan">gh.configs.</span>writeGlobalConfigCredentials (user, token)](#apidoc.element.gh.configs.writeGlobalConfigCredentials)
- description and source-code
```javascript
writeGlobalConfigCredentials = function (user, token) {
    var configPath = exports.getUserHomePath();

    exports.writeGlobalConfig('github_user', user);
    exports.writeGlobalConfig('github_token', token);
    logger.log('Writing GH config data: ' + configPath);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gh.exec"></a>[module gh.exec](#apidoc.module.gh.exec)

#### <a name="apidoc.element.gh.exec.execSync"></a>[function <span class="apidocSignatureSpan">gh.exec.</span>execSync (cmd, options)](#apidoc.element.gh.exec.execSync)
- description and source-code
```javascript
execSync = function (cmd, options) {
    if (!options) {
        options = {};
    }

    logger.debug('execSync: ' + cmd);

    options.stdio = ['pipe', process.stdout, process.stderr];

    return child_process.execSync(cmd, options);
}
```
- example usage
```shell
...
    options = {};
}

logger.debug('execSync: ' + cmd);

options.stdio = ['pipe', process.stdout, process.stderr];

return child_process.execSync(cmd, options);
};

exports.execSyncInteractiveStream = function (cmd, options) {
if (!options) {
    options = {};
}
...
```

#### <a name="apidoc.element.gh.exec.execSyncInteractiveStream"></a>[function <span class="apidocSignatureSpan">gh.exec.</span>execSyncInteractiveStream (cmd, options)](#apidoc.element.gh.exec.execSyncInteractiveStream)
- description and source-code
```javascript
execSyncInteractiveStream = function (cmd, options) {
    if (!options) {
        options = {};
    }

    logger.debug('execSyncInteractiveStream: ' + cmd);

    options.stdio = 'inherit';

    return child_process.execSync(cmd, options);
}
```
- example usage
```shell
...
    callback && callback();
    return;
}

logger.log(logger.colors.cyan('[hook]'), truncate(raw.trim(), 120));

try {
    exec.execSyncInteractiveStream(raw, {cwd: process.cwd()});
} catch(e) {
    logger.debug('[' + when + ' hook failure]');
} finally {
    logger.debug(logger.colors.cyan('[end of ' + when + ' hook]'));
}

callback && callback();
...
```

#### <a name="apidoc.element.gh.exec.spawnSync"></a>[function <span class="apidocSignatureSpan">gh.exec.</span>spawnSync (cmd, args, options)](#apidoc.element.gh.exec.spawnSync)
- description and source-code
```javascript
spawnSync = function (cmd, args, options) {
    var exec;

    logger.debug('spawnSync: ' + cmd + ' ' + args.join(' '));

    exec = child_process.spawnSync(cmd, args, options);

    if (exec.error && exec.error.code === 'ENOENT' && process.platform === 'win32') {
        logger.debug('Invoking patched sapwnSync due to Windows\' libuv bug');
        exec = child_process.spawnSync(cmd + '.cmd', args, options);
    }

    return {
        stdout: exec.stdout.toString().trim(),
        stderr: exec.stderr.toString().trim(),
        status: exec.status
    };
}
```
- example usage
```shell
...
// -- Config -------------------------------------------------------------------

exports.getNodeModulesGlobalPath = function () {
    var result,
path = exports.getConfig()[PLUGINS_PATH_KEY];

    if (path === undefined) {
result = exec.spawnSync('npm', ['root', '-g']);

if (result.stdout) {
    path = result.stdout;
    exports.writeGlobalConfig(PLUGINS_PATH_KEY, path);
}
else {
    logger.warn('Can\'t resolve plugins directory path.');
...
```

#### <a name="apidoc.element.gh.exec.spawnSyncStream"></a>[function <span class="apidocSignatureSpan">gh.exec.</span>spawnSyncStream (cmd, args, options)](#apidoc.element.gh.exec.spawnSyncStream)
- description and source-code
```javascript
spawnSyncStream = function (cmd, args, options) {
    var proc,
        err;

    if (!options) {
        options = {};
    }

    options.stdio = ['pipe', process.stdout, process.stderr];

    logger.debug('spawnSyncStream: ' + cmd + ' ' + args.join(' '));

    proc = child_process.spawnSync(cmd, args, options);

    if (proc.status !== 0) {
        err = new Error();
        err.code = proc.status;
        err.message = 'Child process terminated with error code ' + err.code;

        throw err;
    }

    return proc;
}
```
- example usage
```shell
...
exports.checkout = function (branch, newBranch) {
var args = ['checkout', branch];

if (newBranch) {
    args.push('-B', newBranch);
}

return exec.spawnSyncStream(git_command, args);
};

exports.clone = function (url, folder) {
var args = ['clone', url];

if (folder) {
    args.push(folder);
...
```



# <a name="apidoc.module.gh.git"></a>[module gh.git](#apidoc.module.gh.git)

#### <a name="apidoc.element.gh.git._merge"></a>[function <span class="apidocSignatureSpan">gh.git.</span>_merge (branch, type)](#apidoc.element.gh.git._merge)
- description and source-code
```javascript
_merge = function (branch, type) {
    var res;

    try {
        res = exec.spawnSyncStream(git_command, [type, branch]);
    } catch(err) {
        if (err.code && err.code !== 0) {
            exec.spawnSyncStream(git_command, [type, '--abort']);
            throw err;
        }
    }
}
```
- example usage
```shell
...
            exec.spawnSyncStream(git_command, [type, '--abort']);
            throw err;
        }
    }
};

exports.merge = function (branch) {
    return this._merge(branch, 'merge');
};

exports.rebase = function (branch) {
    return this._merge(branch, 'rebase');
};

exports.push = function (remote, branch) {
...
```

#### <a name="apidoc.element.gh.git.checkout"></a>[function <span class="apidocSignatureSpan">gh.git.</span>checkout (branch, newBranch)](#apidoc.element.gh.git.checkout)
- description and source-code
```javascript
checkout = function (branch, newBranch) {
    var args = ['checkout', branch];

    if (newBranch) {
        args.push('-B', newBranch);
    }

    return exec.spawnSyncStream(git_command, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.clone"></a>[function <span class="apidocSignatureSpan">gh.git.</span>clone (url, folder)](#apidoc.element.gh.git.clone)
- description and source-code
```javascript
clone = function (url, folder) {
    var args = ['clone', url];

    if (folder) {
        args.push(folder);
    }

    return exec.spawnSyncStream(git_command, args);
}
```
- example usage
```shell
...

        // Try to retrieve iterative values from iterative option key,
        // e.g. option['number'] === [1,2,3]. If iterative option key is not
        // present, assume [undefined] in order to initialize the loop.
        iterativeValues = options[iterative] || [undefined];

        iterativeValues.forEach(function (value) {
options = base.clone(options);

// Value can be undefined when the command doesn't have a iterative
// option.
options[iterative] = value;

invokePayload(options, Command, cooked, remain);
...
```

#### <a name="apidoc.element.gh.git.countUserAdjacentCommits"></a>[function <span class="apidocSignatureSpan">gh.git.</span>countUserAdjacentCommits ()](#apidoc.element.gh.git.countUserAdjacentCommits)
- description and source-code
```javascript
countUserAdjacentCommits = function () {
    var git,
        params,
        commits = 0,
        user = exports.getConfig('user.name'),
        author;

    do {
        params = ['log', '-1', '--skip=' + commits, '--pretty=%an'];
        git = exec.spawnSync(git_command, params);

        if (git.status !== 0) {
            logger.error(git.stderr);
        }

        author = git.stdout;

        commits += 1;
    } while (author === user);

    commits -= 1;

    return commits;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.deleteBranch"></a>[function <span class="apidocSignatureSpan">gh.git.</span>deleteBranch (branch)](#apidoc.element.gh.git.deleteBranch)
- description and source-code
```javascript
deleteBranch = function (branch) {
    var git = exec.spawnSync(git_command, ['branch', '-d', branch]);

    if (git.status !== 0) {
        logger.debug(git.stderr);
    }

    return git.stdout;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.fetch"></a>[function <span class="apidocSignatureSpan">gh.git.</span>fetch (repoUrl, headBranch, pullBranch)](#apidoc.element.gh.git.fetch)
- description and source-code
```javascript
fetch = function (repoUrl, headBranch, pullBranch) {
    var args = ['fetch', repoUrl, headBranch + ':' + pullBranch, '--no-tags'];

    return exec.spawnSyncStream(git_command, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.findRoot"></a>[function <span class="apidocSignatureSpan">gh.git.</span>findRoot ()](#apidoc.element.gh.git.findRoot)
- description and source-code
```javascript
findRoot = function () {
    return exec.spawnSync(git_command, ['rev-parse', '--show-toplevel']).stdout;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.getCommitMessage"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getCommitMessage (branch, number)](#apidoc.element.gh.git.getCommitMessage)
- description and source-code
```javascript
getCommitMessage = function (branch, number) {
    var git,
        params = ['log'];

    if (!number) {
        number = 1;
    }

    params.push('-' + number, '--first-parent', '--no-merges', '--pretty=%s');

    if (branch) {
        params.push(branch);
    }

    params.push('--');

    git = exec.spawnSync(git_command, params);

    if (git.status !== 0) {
        logger.debug('Can\'t get commit message.');
        return;
    }

    return git.stdout;
}
```
- example usage
```shell
...
    return;
}

return git.stdout;
};

exports.getLastCommitMessage = function (branch) {
return exports.getCommitMessage(branch, 1);
};

exports.getLastCommitSHA = function () {
var git = exec.spawnSync(git_command, ['rev-parse', '--short', 'HEAD']);

if (git.status !== 0) {
    throw new Error('Can\'t retrieve last commit.');
...
```

#### <a name="apidoc.element.gh.git.getConfig"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getConfig (key)](#apidoc.element.gh.git.getConfig)
- description and source-code
```javascript
getConfig = function (key) {
    var git = exec.spawnSync(git_command, ['config', '--get', key]);

    if (git.status !== 0) {
        throw new Error('No git config found for ' + key + '\n');
    }

    return git.stdout;
}
```
- example usage
```shell
...
exports.clone = function (o) {
return JSON.parse(JSON.stringify(o));
};

// -- Utils --------------------------------------------------------------------

exports.load = function () {
var config = configs.getConfig();

exports.github = new Github({
    debug: false,
    host: config.api.host,
    protocol: config.api.protocol,
    version: config.api.version,
    pathPrefix: config.api.pathPrefix
...
```

#### <a name="apidoc.element.gh.git.getCurrentBranch"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getCurrentBranch ()](#apidoc.element.gh.git.getCurrentBranch)
- description and source-code
```javascript
getCurrentBranch = function () {
    var git = exec.spawnSync(git_command, ['symbolic-ref', '--short', 'HEAD']);

    if (git.status !== 0) {
        logger.debug('Can\'t get current branch.');
        return;
    }

    return git.stdout;
}
```
- example usage
```shell
...
    }
    else {
        options.user = options.remoteUser || options.loggedUser;
    }
}

options.repo = options.repo || git.getRepoFromRemoteURL(remoteUrl);
options.currentBranch = options.currentBranch || git.getCurrentBranch();

base.expandAliases(options);
options.github_host = config.github_host;
options.github_gist_host = config.github_gist_host;

// Try to retrieve iterative values from iterative option key,
// e.g. option['number'] === [1,2,3]. If iterative option key is not
...
```

#### <a name="apidoc.element.gh.git.getLastCommitMessage"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getLastCommitMessage (branch)](#apidoc.element.gh.git.getLastCommitMessage)
- description and source-code
```javascript
getLastCommitMessage = function (branch) {
    return exports.getCommitMessage(branch, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.getLastCommitSHA"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getLastCommitSHA ()](#apidoc.element.gh.git.getLastCommitSHA)
- description and source-code
```javascript
getLastCommitSHA = function () {
    var git = exec.spawnSync(git_command, ['rev-parse', '--short', 'HEAD']);

    if (git.status !== 0) {
        throw new Error('Can\'t retrieve last commit.');
    }

    return git.stdout;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.getRemoteUrl"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getRemoteUrl (remote)](#apidoc.element.gh.git.getRemoteUrl)
- description and source-code
```javascript
getRemoteUrl = function (remote) {
    try {
        return exports.getConfig('remote.' + remote + '.url');
    }
    catch(e) {
        logger.debug('Can\'t get remote URL.');
        return;
    }
}
```
- example usage
```shell
...
else {
    User.login(callback);
}
    });

    async.series(operations, function () {
var iterativeValues,
    remoteUrl = git.getRemoteUrl(options.remote);

options.isTTY = {};
options.isTTY.in = Boolean(process.stdin.isTTY);
options.isTTY.out = Boolean(process.stdout.isTTY);
options.loggedUser = base.getUser();
options.remoteUser = git.getUserFromRemoteUrl(remoteUrl);
...
```

#### <a name="apidoc.element.gh.git.getRepo"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getRepo (remote)](#apidoc.element.gh.git.getRepo)
- description and source-code
```javascript
getRepo = function (remote) {
    return exports.getRepoFromRemoteURL(exports.getRemoteUrl(remote));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.git.getRepoFromRemoteURL"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getRepoFromRemoteURL (url)](#apidoc.element.gh.git.getRepoFromRemoteURL)
- description and source-code
```javascript
getRepoFromRemoteURL = function (url) {
    var parsed = exports.parseRemoteUrl(url);

    return parsed && parsed[1];
}
```
- example usage
```shell
...
        options.user = options.loggedUser;
    }
    else {
        options.user = options.remoteUser || options.loggedUser;
    }
}

options.repo = options.repo || git.getRepoFromRemoteURL(remoteUrl);
options.currentBranch = options.currentBranch || git.getCurrentBranch();

base.expandAliases(options);
options.github_host = config.github_host;
options.github_gist_host = config.github_gist_host;

// Try to retrieve iterative values from iterative option key,
...
```

#### <a name="apidoc.element.gh.git.getUser"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getUser (remote)](#apidoc.element.gh.git.getUser)
- description and source-code
```javascript
getUser = function (remote) {
    return exports.getUserFromRemoteUrl(exports.getRemoteUrl(remote));
}
```
- example usage
```shell
...
    async.series(operations, function () {
var iterativeValues,
    remoteUrl = git.getRemoteUrl(options.remote);

options.isTTY = {};
options.isTTY.in = Boolean(process.stdin.isTTY);
options.isTTY.out = Boolean(process.stdout.isTTY);
options.loggedUser = base.getUser();
options.remoteUser = git.getUserFromRemoteUrl(remoteUrl);

if (!options.user) {
    if (options.repo || options.all) {
        options.user = options.loggedUser;
    }
    else {
...
```

#### <a name="apidoc.element.gh.git.getUserFromRemoteUrl"></a>[function <span class="apidocSignatureSpan">gh.git.</span>getUserFromRemoteUrl (url)](#apidoc.element.gh.git.getUserFromRemoteUrl)
- description and source-code
```javascript
getUserFromRemoteUrl = function (url) {
    var parsed = exports.parseRemoteUrl(url);

    return parsed && parsed[0];
}
```
- example usage
```shell
...
var iterativeValues,
    remoteUrl = git.getRemoteUrl(options.remote);

options.isTTY = {};
options.isTTY.in = Boolean(process.stdin.isTTY);
options.isTTY.out = Boolean(process.stdout.isTTY);
options.loggedUser = base.getUser();
options.remoteUser = git.getUserFromRemoteUrl(remoteUrl);

if (!options.user) {
    if (options.repo || options.all) {
        options.user = options.loggedUser;
    }
    else {
        options.user = options.remoteUser || options.loggedUser;
...
```

#### <a name="apidoc.element.gh.git.merge"></a>[function <span class="apidocSignatureSpan">gh.git.</span>merge (branch)](#apidoc.element.gh.git.merge)
- description and source-code
```javascript
merge = function (branch) {
    return this._merge(branch, 'merge');
}
```
- example usage
```shell
...
var lodash = require('lodash');
var logger = require('./logger');

var RestApiClient = (function () {
function RestApiClient(options) {
    _classCallCheck(this, RestApiClient);

    options = lodash.merge(this.DEFAULT_CONFIG, options);
    this.options = options;
}

RestApiClient.prototype.encode = function encode() {
    return encodeURIComponent.apply(this, arguments);
};
...
```

#### <a name="apidoc.element.gh.git.parseRemoteUrl"></a>[function <span class="apidocSignatureSpan">gh.git.</span>parseRemoteUrl (url)](#apidoc.element.gh.git.parseRemoteUrl)
- description and source-code
```javascript
parseRemoteUrl = function (url) {
    var parsed = /[\/:]([\w-]+)\/(.*?)(?:\.git)?$/.exec(url);

    if (parsed) {
        parsed.shift();
    }

    return parsed;
}
```
- example usage
```shell
...
catch(e) {
    logger.debug('Can\'t get remote URL.');
    return;
}
};

exports.getRepoFromRemoteURL = function (url) {
var parsed = exports.parseRemoteUrl(url);

return parsed && parsed[1];
};

exports.getUserFromRemoteUrl = function (url) {
var parsed = exports.parseRemoteUrl(url);
...
```

#### <a name="apidoc.element.gh.git.push"></a>[function <span class="apidocSignatureSpan">gh.git.</span>push (remote, branch)](#apidoc.element.gh.git.push)
- description and source-code
```javascript
push = function (remote, branch) {
    var args = ['push', remote];

    if (branch) {
        args.push(branch);
    }

    return exec.spawnSyncStream(git_command, args);
}
```
- example usage
```shell
...
};

CmdAnonymizer.prototype.classify = function (word) {
var arg = this.extractArgument(word),
    whitelist = ['verbose', 'no-hooks'];

if (whitelist.indexOf(arg) === 0) {
    this.invoked.push(word);
    this.last = arg;
    return;
}

if (this.shorthands && this.shorthands[arg]) {
    this.invoked.push(word);
    this.last = this.shorthands[arg];
...
```

#### <a name="apidoc.element.gh.git.rebase"></a>[function <span class="apidocSignatureSpan">gh.git.</span>rebase (branch)](#apidoc.element.gh.git.rebase)
- description and source-code
```javascript
rebase = function (branch) {
    return this._merge(branch, 'rebase');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gh.hooks"></a>[module gh.hooks](#apidoc.module.gh.hooks)

#### <a name="apidoc.element.gh.hooks.createContext"></a>[function <span class="apidocSignatureSpan">gh.hooks.</span>createContext (scope)](#apidoc.element.gh.hooks.createContext)
- description and source-code
```javascript
createContext = function (scope) {
    return {
        options: scope.options,
        signature: config.signature
    };
}
```
- example usage
```shell
...
    context;

if (options.hooks === false || process.env.NODEGH_HOOK_IS_LOCKED) {
    opt_callback && opt_callback();
    return;
}

context = exports.createContext(scope);

beforeOperations = [

    function (callback) {
        exports.setupPlugins_(context, 'setupBeforeHooks', callback);
    }
];
...
```

#### <a name="apidoc.element.gh.hooks.getHooksArrayFromPath_"></a>[function <span class="apidocSignatureSpan">gh.hooks.</span>getHooksArrayFromPath_ (path, opt_config)](#apidoc.element.gh.hooks.getHooksArrayFromPath_)
- description and source-code
```javascript
getHooksArrayFromPath_ = function (path, opt_config) {
    var keys = path.split('.'),
        key = keys.shift(),
        hooks;

    opt_config = opt_config || config;

    hooks = opt_config.hooks || {};

    while (hooks[key]) {
        hooks = hooks[key];
        key = keys.shift();
    }

    return Array.isArray(hooks) ? hooks : [];
}
```
- example usage
```shell
...

exports.getHooksFromPath = function (path) {
    var hooks,
plugins = configs.getPlugins(),
pluginHooks = [];

    // First, load all core hooks for the specified path.
    hooks = exports.getHooksArrayFromPath_(path);

    // Second, search all installed plugins and load the hooks for each into
    // core hooks array.
    plugins.forEach(function (plugin) {
var pluginConfig;

plugin = configs.getPluginBasename(plugin);
...
```

#### <a name="apidoc.element.gh.hooks.getHooksFromPath"></a>[function <span class="apidocSignatureSpan">gh.hooks.</span>getHooksFromPath (path)](#apidoc.element.gh.hooks.getHooksFromPath)
- description and source-code
```javascript
getHooksFromPath = function (path) {
    var hooks,
        plugins = configs.getPlugins(),
        pluginHooks = [];

    // First, load all core hooks for the specified path.
    hooks = exports.getHooksArrayFromPath_(path);

    // Second, search all installed plugins and load the hooks for each into
    // core hooks array.
    plugins.forEach(function (plugin) {
        var pluginConfig;

        plugin = configs.getPluginBasename(plugin);

        if (config.plugins && !configs.isPluginIgnored(plugin)) {
            pluginConfig = config.plugins[plugin];

            if (pluginConfig) {
                pluginHooks = pluginHooks.concat(
                    exports.getHooksArrayFromPath_(path, pluginConfig));
            }
        }
    });

    return hooks.concat(pluginHooks);
}
```
- example usage
```shell
...
    }
});

return hooks.concat(pluginHooks);
};

exports.invoke = function (path, scope, opt_callback) {
var after = exports.getHooksFromPath(path + '.after'),
    before = exports.getHooksFromPath(path + '.before'),
    beforeOperations,
    afterOperations,
    options = scope.options,
    context;

if (options.hooks === false || process.env.NODEGH_HOOK_IS_LOCKED) {
...
```

#### <a name="apidoc.element.gh.hooks.invoke"></a>[function <span class="apidocSignatureSpan">gh.hooks.</span>invoke (path, scope, opt_callback)](#apidoc.element.gh.hooks.invoke)
- description and source-code
```javascript
invoke = function (path, scope, opt_callback) {
    var after = exports.getHooksFromPath(path + '.after'),
        before = exports.getHooksFromPath(path + '.before'),
        beforeOperations,
        afterOperations,
        options = scope.options,
        context;

    if (options.hooks === false || process.env.NODEGH_HOOK_IS_LOCKED) {
        opt_callback && opt_callback();
        return;
    }

    context = exports.createContext(scope);

    beforeOperations = [

        function (callback) {
            exports.setupPlugins_(context, 'setupBeforeHooks', callback);
        }
    ];

    before.forEach(function (cmd) {
        beforeOperations.push(exports.wrapCommand_(cmd, context, 'before'));
    });

    afterOperations = [

        function (callback) {
            exports.setupPlugins_(context, 'setupAfterHooks', callback);
        }
    ];

    after.forEach(function (cmd) {
        afterOperations.push(exports.wrapCommand_(cmd, context, 'after'));
    });

    afterOperations.push(function (callback) {
        process.env.NODEGH_HOOK_IS_LOCKED = false;
        callback();
    });

    process.env.NODEGH_HOOK_IS_LOCKED = true;

    async.series(beforeOperations, function () {
        opt_callback && opt_callback(function () {
            async.series(afterOperations);
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.hooks.setupPlugins_"></a>[function <span class="apidocSignatureSpan">gh.hooks.</span>setupPlugins_ (context, setupFn, opt_callback)](#apidoc.element.gh.hooks.setupPlugins_)
- description and source-code
```javascript
setupPlugins_ = function (context, setupFn, opt_callback) {
    var plugins = configs.getPlugins(),
        operations = [];

    plugins.forEach(function (plugin) {
        try {
            plugin = configs.getPlugin(plugin);
        }
        catch(e) {
            logger.warn('Can\'t get ' + plugin + ' plugin.');
        }

        if (plugin && plugin[setupFn]) {
            operations.push(function (callback) {
                plugin[setupFn](context, callback);
            });
        }
    });

    async.series(operations, function () {
        opt_callback && opt_callback();
    });
}
```
- example usage
```shell
...
}

context = exports.createContext(scope);

beforeOperations = [

    function (callback) {
        exports.setupPlugins_(context, 'setupBeforeHooks', callback);
    }
];

before.forEach(function (cmd) {
    beforeOperations.push(exports.wrapCommand_(cmd, context, 'before'));
});
...
```

#### <a name="apidoc.element.gh.hooks.wrapCommand_"></a>[function <span class="apidocSignatureSpan">gh.hooks.</span>wrapCommand_ (cmd, context, when)](#apidoc.element.gh.hooks.wrapCommand_)
- description and source-code
```javascript
wrapCommand_ = function (cmd, context, when) {
    return function (callback) {
        var raw = logger.compileTemplate(cmd, context);

        if (!raw) {
            callback && callback();
            return;
        }

        logger.log(logger.colors.cyan('[hook]'), truncate(raw.trim(), 120));

        try {
            exec.execSyncInteractiveStream(raw, {cwd: process.cwd()});
        } catch(e) {
            logger.debug('[' + when + ' hook failure]');
        } finally {
            logger.debug(logger.colors.cyan('[end of ' + when + ' hook]'));
        }

        callback && callback();
    };
}
```
- example usage
```shell
...

function (callback) {
    exports.setupPlugins_(context, 'setupBeforeHooks', callback);
}
    ];

    before.forEach(function (cmd) {
beforeOperations.push(exports.wrapCommand_(cmd, context, 'before'));
    });

    afterOperations = [

function (callback) {
    exports.setupPlugins_(context, 'setupAfterHooks', callback);
}
...
```



# <a name="apidoc.module.gh.logger"></a>[module gh.logger](#apidoc.module.gh.logger)

#### <a name="apidoc.element.gh.logger.applyReplacements"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>applyReplacements (output, replaceMap)](#apidoc.element.gh.logger.applyReplacements)
- description and source-code
```javascript
applyReplacements = function (output, replaceMap) {
    var regexPattern;

    for (regexPattern in replaceMap) {
        if (replaceMap.hasOwnProperty(regexPattern)) {
            output = output.replace(
                new RegExp(regexPattern, 'g'), replaceMap[regexPattern]);
        }
    }

    return output;
}
```
- example usage
```shell
...
    // Normalize git error
    return err.message.replace('Command failed: fatal: ', '').trim();
};

logger.compileTemplate = function (source, map) {
    var template = handlebars.compile(source);

    return logger.applyReplacements(template(map));
};

logger.logTemplate = function (source, map) {
    console.log(logger.compileTemplate(source, map || {}));
};

logger.logTemplateFile = function (file, map) {
...
```

#### <a name="apidoc.element.gh.logger.compileTemplate"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>compileTemplate (source, map)](#apidoc.element.gh.logger.compileTemplate)
- description and source-code
```javascript
compileTemplate = function (source, map) {
    var template = handlebars.compile(source);

    return logger.applyReplacements(template(map));
}
```
- example usage
```shell
...
    async.series(operations, function () {
opt_callback && opt_callback();
    });
};

exports.wrapCommand_ = function (cmd, context, when) {
    return function (callback) {
var raw = logger.compileTemplate(cmd, context);

if (!raw) {
    callback && callback();
    return;
}

logger.log(logger.colors.cyan('[hook]'), truncate(raw.trim(), 120));
...
```

#### <a name="apidoc.element.gh.logger.debug"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>debug ()](#apidoc.element.gh.logger.debug)
- description and source-code
```javascript
debug = function () {
    if (!process.env.GH_VERBOSE) {
        return;
    }

    if (typeof arguments[0] === 'string') {
        arguments[0] = 'DEBUG: ' + arguments[0];
        console.log.apply(this, arguments);
        return;
    }

    console.log('DEBUG:');
    console.log.apply(this, arguments);
}
```
- example usage
```shell
...
    Object.keys(projectConfig).forEach(function (key) {
        result[key] = projectConfig[key];
    });

    return result;
}
catch (e) {
    logger.debug(e.message);

    if (e.code !== 'MODULE_NOT_FOUND' && e.code !== 'ENOENT') {
        throw e;
    }

    return globalConfig;
}
...
```

#### <a name="apidoc.element.gh.logger.error"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>error ()](#apidoc.element.gh.logger.error)
- description and source-code
```javascript
error = function () {
    if (typeof arguments[0] === 'string') {
        arguments[0] = 'fatal: ' + arguments[0];
    }

    console.error.apply(this, arguments);
    process.exit(1);
}
```
- example usage
```shell
...
    module = 'help';
}

Command = loadCommand(module);

if (!Command) {
    tracker.trackCommand(remain);
    logger.error('Command not found');
    return;
}

options = nopt(
    Command.DETAILS.options,
    Command.DETAILS.shorthands, process.argv, 2);
...
```

#### <a name="apidoc.element.gh.logger.getDuration"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>getDuration (start, opt_end)](#apidoc.element.gh.logger.getDuration)
- description and source-code
```javascript
getDuration = function (start, opt_end) {
    if (opt_end === undefined) {
        opt_end = Date.now();
    }

    return moment.duration(moment(start).diff(opt_end)).humanize(true);
}
```
- example usage
```shell
...

logger.registerHelper = function (name, callback) {
handlebars.registerHelper(name, callback);
};

logger.registerHelpers_ = function () {
handlebars.registerHelper('date', function (date) {
    return logger.getDuration(date);
});

handlebars.registerHelper('compareLink', function () {
    return this.options.github_host + this.options.user + '/' + this.options.repo +
        '/compare/' + this.options.pullHeadSHA + '...' + this.options.currentSHA;
});
...
```

#### <a name="apidoc.element.gh.logger.getErrorMessage"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>getErrorMessage (err)](#apidoc.element.gh.logger.getErrorMessage)
- description and source-code
```javascript
getErrorMessage = function (err) {
    var msg;

    // General normalizer
    if (!err) {
        return 'No error message.';
    }

    if (err.errors) {
        return err.errors;
    }

    // Normalize github api error
    if (!err.message) {
        return err;
    }

    try {
        msg = JSON.parse(err.message);
    } catch(e) {
        return err.message;
    }

    if (typeof msg === 'string') {
        return msg;
    }

    if (msg.errors && msg.errors[0] && msg.errors[0].message) {
        return msg.errors[0].message;
    }

    if (msg.message) {
        return msg.message;
    }

    // Normalize git error
    return err.message.replace('Command failed: fatal: ', '').trim();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.logger.insane"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>insane ()](#apidoc.element.gh.logger.insane)
- description and source-code
```javascript
insane = function () {
    if (!process.env.GH_VERBOSE_INSANE) {
        return;
    }

    console.log.apply(this, arguments);
}
```
- example usage
```shell
...
        this.authorize(p);

        var id = Math.floor(Math.random() * 10000000);
        var begin = new Date().getTime();

        return new Promise(function (resolve, reject) {
            logger.debug('New request #' + id + ' started at ' + begin + ':\n' + method + ' ' + p.uri);
            logger.insane(p);
            _request(p, function (error, response) {
var end = new Date().getTime();
logger.debug('End of request #' + id + ' at ' + end + ' (' + (end - begin) + 'ms)' + ' with status code: ' + (response && response
.statusCode));

if (response) {
    logger.insane('Response headers:');
    logger.insane(response.headers);
...
```

#### <a name="apidoc.element.gh.logger.log"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>log ()](#apidoc.element.gh.logger.log)
- description and source-code
```javascript
log = function () {
    console.log.apply(this, arguments);
}
```
- example usage
```shell
...
};

exports.writeGlobalConfigCredentials = function (user, token) {
var configPath = exports.getUserHomePath();

exports.writeGlobalConfig('github_user', user);
exports.writeGlobalConfig('github_token', token);
logger.log('Writing GH config data: ' + configPath);
};

// -- Plugins ------------------------------------------------------------------

exports.addPluginConfig = function (config, plugin) {
var pluginConfig,
    userConfig;
...
```

#### <a name="apidoc.element.gh.logger.logTemplate"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>logTemplate (source, map)](#apidoc.element.gh.logger.logTemplate)
- description and source-code
```javascript
logTemplate = function (source, map) {
    console.log(logger.compileTemplate(source, map || {}));
}
```
- example usage
```shell
...

    if (!fs.existsSync(templatePath)) {
        templatePath = path.join(__dirname, 'cmds/templates', file);
    }

    source = fs.readFileSync(templatePath).toString();

    logger.logTemplate(stripHandlebarsNewLine(source), map);
};

logger.registerHelper = function (name, callback) {
    handlebars.registerHelper(name, callback);
};

logger.registerHelpers_ = function () {
...
```

#### <a name="apidoc.element.gh.logger.logTemplateFile"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>logTemplateFile (file, map)](#apidoc.element.gh.logger.logTemplateFile)
- description and source-code
```javascript
logTemplateFile = function (file, map) {
    var templatePath,
        source;

    templatePath = path.join(file);

    if (!fs.existsSync(templatePath)) {
        templatePath = path.join(__dirname, 'cmds/templates', file);
    }

    source = fs.readFileSync(templatePath).toString();

    logger.logTemplate(stripHandlebarsNewLine(source), map);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.logger.registerHelper"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>registerHelper (name, callback)](#apidoc.element.gh.logger.registerHelper)
- description and source-code
```javascript
registerHelper = function (name, callback) {
    handlebars.registerHelper(name, callback);
}
```
- example usage
```shell
...

source = fs.readFileSync(templatePath).toString();

logger.logTemplate(stripHandlebarsNewLine(source), map);
};

logger.registerHelper = function (name, callback) {
handlebars.registerHelper(name, callback);
};

logger.registerHelpers_ = function () {
handlebars.registerHelper('date', function (date) {
    return logger.getDuration(date);
});
...
```

#### <a name="apidoc.element.gh.logger.registerHelpers_"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>registerHelpers_ ()](#apidoc.element.gh.logger.registerHelpers_)
- description and source-code
```javascript
registerHelpers_ = function () {
    handlebars.registerHelper('date', function (date) {
        return logger.getDuration(date);
    });

    handlebars.registerHelper('compareLink', function () {
        return this.options.github_host + this.options.user + '/' + this.options.repo +
            '/compare/' + this.options.pullHeadSHA + '...' + this.options.currentSHA;
    });

    handlebars.registerHelper('forwardedLink', function () {
        return this.options.github_host + this.options.fwd + '/' + this.options.repo + '/pull/' +
            this.options.forwardedPull;
    });

    handlebars.registerHelper('link', function () {
        return this.options.github_host + this.options.user + '/' + this.options.repo + '/pull/' +
            this.options.number;
    });

    handlebars.registerHelper('submittedLink', function () {
        return this.options.github_host + this.options.submit + '/' + this.options.repo + '/pull/' +
            this.options.submittedPull;
    });

    handlebars.registerHelper('issueLink', function () {
        return this.options.github_host + this.options.user + '/' + this.options.repo + '/issues/' +
            this.options.number;
    });

    handlebars.registerHelper('gistLink', function () {
        return this.options.github_gist_host + this.options.loggedUser + '/' + this.options.id;
    });

    handlebars.registerHelper('repoLink', function () {
        return this.options.github_host + this.options.user + '/' + this.options.repo;
    });

    handlebars.registerHelper('wordwrap', function (text, padding, stripNewLines) {
        var gutter = '';

        if (stripNewLines !== false) {
            text = text.replace(/[\r\n\s\t]+/g, ' ');
        }

        text = wrap(text).split('\n');

        if (padding > 0) {
            gutter = (new Array(padding)).join(' ');
        }

        return text.join('\n' + gutter);
    });
}
```
- example usage
```shell
...
            gutter = (new Array(padding)).join(' ');
        }

        return text.join('\n' + gutter);
    });
};

logger.registerHelpers_();

logger.colors = colors;
module.exports = logger;
...
```

#### <a name="apidoc.element.gh.logger.warn"></a>[function <span class="apidocSignatureSpan">gh.logger.</span>warn ()](#apidoc.element.gh.logger.warn)
- description and source-code
```javascript
warn = function () {
    arguments[0] = 'warning: ' + arguments[0];
    console.error.apply(this, arguments);
}
```
- example usage
```shell
...
        result = exec.spawnSync('npm', ['root', '-g']);

        if (result.stdout) {
            path = result.stdout;
            exports.writeGlobalConfig(PLUGINS_PATH_KEY, path);
        }
        else {
            logger.warn('Can\'t resolve plugins directory path.');
        }
    }

    return path;
};

exports.getUserHomePath = function () {
...
```



# <a name="apidoc.module.gh.rest_api_client"></a>[module gh.rest_api_client](#apidoc.module.gh.rest_api_client)

#### <a name="apidoc.element.gh.rest_api_client.rest_api_client"></a>[function <span class="apidocSignatureSpan">gh.</span>rest_api_client (options)](#apidoc.element.gh.rest_api_client.rest_api_client)
- description and source-code
```javascript
function RestApiClient(options) {
    _classCallCheck(this, RestApiClient);

    options = lodash.merge(this.DEFAULT_CONFIG, options);
    this.options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gh.rest_api_client.prototype"></a>[module gh.rest_api_client.prototype](#apidoc.module.gh.rest_api_client.prototype)

#### <a name="apidoc.element.gh.rest_api_client.prototype.authorize"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>authorize (p)](#apidoc.element.gh.rest_api_client.prototype.authorize)
- description and source-code
```javascript
function authorize(p) {
    var options = this.options;

    if (p.oauth) {
        p.oauth = options.oauth;
        return;
    }

    if (typeof options.user === 'string') {
        p.auth = {
            'user': options.user,
            'pass': options.password
        };
    }
}
```
- example usage
```shell
...
    followAllRedirects: true
};

if (params) {
    p = lodash.merge(p, params);
}

this.authorize(p);

var id = Math.floor(Math.random() * 10000000);
var begin = new Date().getTime();

return new Promise(function (resolve, reject) {
    logger.debug('New request #' + id + ' started at ' + begin + ':\n' + method + ' ' + p.uri);
    logger.insane(p);
...
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.delete"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>delete ()](#apidoc.element.gh.rest_api_client.prototype.delete)
- description and source-code
```javascript
function _delete() {
    return this.request('DELETE', arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.encode"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>encode ()](#apidoc.element.gh.rest_api_client.prototype.encode)
- description and source-code
```javascript
function encode() {
    return encodeURIComponent.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.get"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>get ()](#apidoc.element.gh.rest_api_client.prototype.get)
- description and source-code
```javascript
function get() {
    return this.request('GET', arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.post"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>post ()](#apidoc.element.gh.rest_api_client.prototype.post)
- description and source-code
```javascript
function post() {
    return this.request('POST', arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.put"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>put ()](#apidoc.element.gh.rest_api_client.prototype.put)
- description and source-code
```javascript
function put() {
    return this.request('PUT', arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.request"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>request (method, path, params)](#apidoc.element.gh.rest_api_client.prototype.request)
- description and source-code
```javascript
function request(method, path, params) {
    if (typeof path === 'object') {
        var args = Array.from(path);
        args.unshift(method);
        return this.request.apply(this, args);
    }

    var options = this.options;

    var p = {
        strictSSL: options.strictSSL,
        method: method,
        uri: this.url(path),
        json: true,
        followAllRedirects: true
    };

    if (params) {
        p = lodash.merge(p, params);
    }

    this.authorize(p);

    var id = Math.floor(Math.random() * 10000000);
    var begin = new Date().getTime();

    return new Promise(function (resolve, reject) {
        logger.debug('New request #' + id + ' started at ' + begin + ':\n' + method + ' ' + p.uri);
        logger.insane(p);
        _request(p, function (error, response) {
            var end = new Date().getTime();
            logger.debug('End of request #' + id + ' at ' + end + ' (' + (end - begin) + 'ms)' + ' with status code: ' + (response
 && response.statusCode));

            if (response) {
                logger.insane('Response headers:');
                logger.insane(response.headers);
                logger.debug('Response body');
                logger.debug(response.body);
            }

            if (error) {
                reject(error);
                return;
            }

            if (response.statusCode < 200 || response.statusCode > 399) {
                reject({
                    error: response.statusCode + ' ' + http.STATUS_CODES[response.statusCode],
                    code: response.statusCode,
                    msg: http.STATUS_CODES[response.statusCode],
                    response: response
                });
                return;
            }

            resolve(response);
        });
    });
}
```
- example usage
```shell
...

            resolve(response);
        });
    });
};

RestApiClient.prototype.get = function get() {
    return this.request('GET', arguments);
};

RestApiClient.prototype.post = function post() {
    return this.request('POST', arguments);
};

RestApiClient.prototype.put = function put() {
...
```

#### <a name="apidoc.element.gh.rest_api_client.prototype.url"></a>[function <span class="apidocSignatureSpan">gh.rest_api_client.prototype.</span>url (pathname, query)](#apidoc.element.gh.rest_api_client.prototype.url)
- description and source-code
```javascript
function url(pathname, query) {
    var options = this.options;
    var uri = _url.format({
        protocol: options.protocol,
        hostname: options.host,
        port: options.port,
        pathname: options.base + pathname,
        query: query
    });

    return decodeURIComponent(uri);
}
```
- example usage
```shell
...
}

var options = this.options;

var p = {
    strictSSL: options.strictSSL,
    method: method,
    uri: this.url(path),
    json: true,
    followAllRedirects: true
};

if (params) {
    p = lodash.merge(p, params);
}
...
```



# <a name="apidoc.module.gh.tracker"></a>[module gh.tracker](#apidoc.module.gh.tracker)

#### <a name="apidoc.element.gh.tracker.resolveCommand"></a>[function <span class="apidocSignatureSpan">gh.tracker.</span>resolveCommand (cmd, commandDetails)](#apidoc.element.gh.tracker.resolveCommand)
- description and source-code
```javascript
resolveCommand = function (cmd, commandDetails) {
    var cmdAnonymizer;

    if (!commandDetails) {
        return cmd.join(' ').replace(/\w+/g, redaction);
    }

    cmdAnonymizer = new CmdAnonymizer(commandDetails, redaction);

    return cmdAnonymizer.resolveToString(cmd);
}
```
- example usage
```shell
...

    cmdAnonymizer = new CmdAnonymizer(commandDetails, redaction);

    return cmdAnonymizer.resolveToString(cmd);
};

tracker.trackCommand = function (cmd, commandDetails) {
    var tracking = pkg.name + ' ' + this.resolveCommand(cmd, commandDetails);

    this.track(tracking.replace(/ /g, '%20'));
};

module.exports = tracker;
...
```

#### <a name="apidoc.element.gh.tracker.trackCommand"></a>[function <span class="apidocSignatureSpan">gh.tracker.</span>trackCommand (cmd, commandDetails)](#apidoc.element.gh.tracker.trackCommand)
- description and source-code
```javascript
trackCommand = function (cmd, commandDetails) {
    var tracking = pkg.name + ' ' + this.resolveCommand(cmd, commandDetails);

    this.track(tracking.replace(/ /g, '%20'));
}
```
- example usage
```shell
...
    (cooked.indexOf('--help') >= 0)) {
    module = 'help';
}

Command = loadCommand(module);

if (!Command) {
    tracker.trackCommand(remain);
    logger.error('Command not found');
    return;
}

options = nopt(
    Command.DETAILS.options,
    Command.DETAILS.shorthands, process.argv, 2);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
