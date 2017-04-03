# api documentation for  [forever-monitor (v1.7.1)](https://github.com/nodejitsu/forever-monitor#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-forever-monitor.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-forever-monitor) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-forever-monitor.svg)](https://travis-ci.org/npmdoc/node-npmdoc-forever-monitor)
#### Core forever process monitor

[![NPM](https://nodei.co/npm/forever-monitor.png?downloads=true)](https://www.npmjs.com/package/forever-monitor)

[![apidoc](https://npmdoc.github.io/node-npmdoc-forever-monitor/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-forever-monitor_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-forever-monitor/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-forever-monitor/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-forever-monitor/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/nodejitsu/forever-monitor/issues"
    },
    "contributors": [
        {
            "name": "Charlie Robbins",
            "email": "charlie@nodejitsu.com"
        },
        {
            "name": "Fedor Indutny",
            "email": "fedor.indutny@gmail.com"
        },
        {
            "name": "James Halliday",
            "email": "mail@substack.net"
        },
        {
            "name": "Bradley Meck",
            "email": "bradley@nodejitsu.com"
        },
        {
            "name": "Dominic Tarr",
            "email": "dominic@nodejitsu.com"
        },
        {
            "name": "Maciej Małecki",
            "email": "maciej@nodejitsu.com"
        }
    ],
    "dependencies": {
        "broadway": "~0.3.6",
        "chokidar": "^1.0.1",
        "minimatch": "~3.0.2",
        "ps-tree": "0.0.x",
        "utile": "~0.2.1"
    },
    "description": "Core forever process monitor",
    "devDependencies": {
        "optimist": "~0.6.1",
        "vows": "~0.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5d820f4a3a78db2d81ae2671f158b9e86a091bb8",
        "tarball": "https://registry.npmjs.org/forever-monitor/-/forever-monitor-1.7.1.tgz"
    },
    "engines": {
        "node": ">= 0.8.x"
    },
    "gitHead": "7d1c4631d831a017b7ae9430585f8b7324f66162",
    "homepage": "https://github.com/nodejitsu/forever-monitor#readme",
    "keywords": [
        "fault tolerant",
        "sysadmin",
        "tools"
    ],
    "license": "MIT",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        }
    ],
    "name": "forever-monitor",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/nodejitsu/forever-monitor.git"
    },
    "scripts": {
        "test": "vows test/**/*-test.js --spec -i"
    },
    "version": "1.7.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module forever-monitor](#apidoc.module.forever-monitor)
1.  [function <span class="apidocSignatureSpan">forever-monitor.</span>Monitor (script, options)](#apidoc.element.forever-monitor.Monitor)
1.  [function <span class="apidocSignatureSpan">forever-monitor.</span>Monitor.super_ (options)](#apidoc.element.forever-monitor.Monitor.super_)
1.  [function <span class="apidocSignatureSpan">forever-monitor.</span>checkProcess (pid)](#apidoc.element.forever-monitor.checkProcess)
1.  [function <span class="apidocSignatureSpan">forever-monitor.</span>kill (pid, killTree, signal, callback)](#apidoc.element.forever-monitor.kill)
1.  [function <span class="apidocSignatureSpan">forever-monitor.</span>start (script, options)](#apidoc.element.forever-monitor.start)
1.  object <span class="apidocSignatureSpan">forever-monitor.</span>Monitor.prototype
1.  object <span class="apidocSignatureSpan">forever-monitor.</span>Monitor.super_.prototype
1.  object <span class="apidocSignatureSpan">forever-monitor.</span>Monitor.super_.super_.prototype
1.  string <span class="apidocSignatureSpan">forever-monitor.</span>version

#### [module forever-monitor.Monitor](#apidoc.module.forever-monitor.Monitor)
1.  [function <span class="apidocSignatureSpan">forever-monitor.</span>Monitor (script, options)](#apidoc.element.forever-monitor.Monitor.Monitor)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.</span>parseCommand (command, args)](#apidoc.element.forever-monitor.Monitor.parseCommand)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.</span>super_ (options)](#apidoc.element.forever-monitor.Monitor.super_)

#### [module forever-monitor.Monitor.prototype](#apidoc.module.forever-monitor.Monitor.prototype)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>_getEnv ()](#apidoc.element.forever-monitor.Monitor.prototype._getEnv)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>kill (forceStop)](#apidoc.element.forever-monitor.Monitor.prototype.kill)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>restart ()](#apidoc.element.forever-monitor.Monitor.prototype.restart)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>send (msg)](#apidoc.element.forever-monitor.Monitor.prototype.send)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>start (restart)](#apidoc.element.forever-monitor.Monitor.prototype.start)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>stop ()](#apidoc.element.forever-monitor.Monitor.prototype.stop)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>toString ()](#apidoc.element.forever-monitor.Monitor.prototype.toString)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>trySpawn ()](#apidoc.element.forever-monitor.Monitor.prototype.trySpawn)
1.  object <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>inspect

#### [module forever-monitor.Monitor.super_](#apidoc.module.forever-monitor.Monitor.super_)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.</span>super_ (conf)](#apidoc.element.forever-monitor.Monitor.super_.super_)

#### [module forever-monitor.Monitor.super_.prototype](#apidoc.module.forever-monitor.Monitor.super_.prototype)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>init (options, callback)](#apidoc.element.forever-monitor.Monitor.super_.prototype.init)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>inspect ()](#apidoc.element.forever-monitor.Monitor.super_.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>remove (name)](#apidoc.element.forever-monitor.Monitor.super_.prototype.remove)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>use (plugin, options, callback)](#apidoc.element.forever-monitor.Monitor.super_.prototype.use)

#### [module forever-monitor.Monitor.super_.super_.prototype](#apidoc.module.forever-monitor.Monitor.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>addListener (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>emit ()](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.emit)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>listeners (type)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>listenersAny ()](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.listenersAny)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>many (event, ttl, fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.many)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>off (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.off)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>offAny (fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.offAny)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>on (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>onAny (fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.onAny)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>once (event, fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.once)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>removeAllListeners (type)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>removeListener (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>setMaxListeners (n)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.setMaxListeners)
1.  string <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>delimiter
1.  string <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>event



# <a name="apidoc.module.forever-monitor"></a>[module forever-monitor](#apidoc.module.forever-monitor)

#### <a name="apidoc.element.forever-monitor.Monitor"></a>[function <span class="apidocSignatureSpan">forever-monitor.</span>Monitor (script, options)](#apidoc.element.forever-monitor.Monitor)
- description and source-code
```javascript
Monitor = function (script, options) {
  //
  // Simple bootstrapper for attaching logger
  // and watch plugins by default. Other plugins
  // can be attached through 'monitor.use(plugin, options)'.
  //
  function bootstrap(monitor) {
    plugins.logger.attach.call(monitor, options);
    if (options.watch) {
      plugins.watch.attach.call(monitor, options);
    }
  }

  var execPath = process.execPath,
      self     = this;

  //
  // Setup basic configuration options
  //
  options               = options || {};
  this.silent           = options.silent || false;
  this.killTree         = options.killTree !== false;
  this.uid              = options.uid || utile.randomString(4);
  this.id               = options.id || false;
  this.pidFile          = options.pidFile;
  this.max              = options.max;
  this.killTTL          = options.killTTL;
  this.killSignal       = options.killSignal || 'SIGKILL';
  this.childExists      = false;
  this.checkFile        = options.checkFile !== false;
  this.times            = 0;
  this.warn             = console.error;

  this.logFile          = options.logFile;
  this.outFile          = options.outFile;
  this.errFile          = options.errFile;
  this.append           = options.append;
  this.usePolling       = options.usePolling;
  this.pollingInterval  = options.pollingInterval;

  //
  // Define some safety checks for commands with spaces
  //
  this.parser = options.parser || Monitor.parseCommand;

  //
  // Setup restart timing. These options control how quickly forever restarts
  // a child process as well as when to kill a "spinning" process
  //
  this.minUptime     = typeof options.minUptime !== 'number' ? 0 : options.minUptime;
  this.spinSleepTime = options.spinSleepTime || null;

  //
  // Special case Windows separately to decouple any
  // future changes
  //
  if (process.platform === 'win32') {
    execPath = '"' + execPath + '"';
  }

  if (options.options) {
    console.warn('options.options is deprecated. Use options.args instead.');
  }

  //
  // Setup the command to spawn and the options to pass
  // to that command.
  //
  this.command   = options.command || execPath;
  this.args      = options.args || options.options || [];
  this.spawnWith = options.spawnWith || {};
  this.sourceDir = options.sourceDir;
  this.fork      = options.fork || false;
  this.cwd       = options.cwd || process.cwd();
  this.hideEnv   = options.hideEnv || [];
  this._env      = options.env || {};
  this._hideEnv  = {};

  //
  // Allow for custom stdio configuration of forked processes
  //
  this.stdio = options.stdio || null;

  //
  // Setup watch configuration options
  //
  this.watchIgnoreDotFiles = options.watchIgnoreDotFiles !== false;
  this.watchIgnorePatterns = options.watchIgnorePatterns || [];
  this.watchDirectory      = options.watchDirectory || this.sourceDir;

  //
  // Create a simple mapping of 'this.hideEnv' to an easily indexable
  // object
  //
  this.hideEnv.forEach(function (key) {
    self._hideEnv[key] = true;
  });

  if (Array.isArray(script)) {
    this.command = script[0];
    this.args = script.slice(1);
  }
  else {
    this.args.unshift(script);
  }

  if (this.sourceDir) {
    this.args[0] = path.join(this.sourceDir, this.args[0]);
  }

  //
  // Bootstrap this instance now that options
  // have been set
  //
  broadway.App.call(this, { bootstrapper: { bootstrap: bootstrap } });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_"></a>[function <span class="apidocSignatureSpan">forever-monitor.</span>Monitor.super_ (options)](#apidoc.element.forever-monitor.Monitor.super_)
- description and source-code
```javascript
Monitor.super_ = function (options) {
  //
  // Setup options and 'App' constants.
  //
  options        = options || {};
  this.root      = options.root;
  this.delimiter = options.delimiter || '::';

  //
  // Inherit from 'EventEmitter2'
  //
  events.EventEmitter2.call(this, {
    delimiter: this.delimiter,
    wildcard: true
  });

  //
  // Setup other relevant options such as the plugins
  // for this instance.
  //
  this.options      = options;
  this.env          = options.env || process.env['NODE_ENV'] || 'development'
  this.plugins      = options.plugins || {};
  this.initialized  = false;
  this.bootstrapper = options.bootstrapper || bootstrapper;
  this.initializers = {};
  this.initlist     = [];

  //
  // Bootstrap this instance
  //
  this.bootstrapper.bootstrap(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.checkProcess"></a>[function <span class="apidocSignatureSpan">forever-monitor.</span>checkProcess (pid)](#apidoc.element.forever-monitor.checkProcess)
- description and source-code
```javascript
checkProcess = function (pid) {
  if (!pid) {
    return false;
  }

  try {
    //
    // Trying to kill non-existent process here raises a ESRCH - no such
    // process exception. Also, signal 0 doesn't do no harm to a process - it
    // only checks if sending a signal to a given process is possible.
    //
    process.kill(pid, 0);
    return true;
  }
  catch (err) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.kill"></a>[function <span class="apidocSignatureSpan">forever-monitor.</span>kill (pid, killTree, signal, callback)](#apidoc.element.forever-monitor.kill)
- description and source-code
```javascript
kill = function (pid, killTree, signal, callback) {
  signal   = signal   || 'SIGKILL';
  callback = callback || function () {};

  if (killTree && process.platform !== 'win32') {
    psTree(pid, function (err, children) {
      [pid].concat(
        children.map(function (p) {
          return p.PID;
        })
      ).forEach(function (tpid) {
        try { process.kill(tpid, signal) }
        catch (ex) { }
      });

      callback();
    });
  }
  else {
    try { process.kill(pid, signal) }
    catch (ex) { }
    callback();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.start"></a>[function <span class="apidocSignatureSpan">forever-monitor.</span>start (script, options)](#apidoc.element.forever-monitor.start)
- description and source-code
```javascript
start = function (script, options) {
  if (!options.uid) {
    options.uid = options.uid || utile.randomString(4).replace(/^\-/, '_');
  }

  return new exports.Monitor(script, options).start();
}
```
- example usage
```shell
...
    args: []
  });

  child.on('exit', function () {
    console.log('your-filename.js has exited after 3 restarts');
  });

  child.start();
'''

### Spawning a non-node process
You can spawn non-node processes too. Either set the 'command' key in the
'options' hash or pass in an 'Array' in place of the 'file' argument like this:

''' js
...
```



# <a name="apidoc.module.forever-monitor.Monitor"></a>[module forever-monitor.Monitor](#apidoc.module.forever-monitor.Monitor)

#### <a name="apidoc.element.forever-monitor.Monitor.Monitor"></a>[function <span class="apidocSignatureSpan">forever-monitor.</span>Monitor (script, options)](#apidoc.element.forever-monitor.Monitor.Monitor)
- description and source-code
```javascript
Monitor = function (script, options) {
  //
  // Simple bootstrapper for attaching logger
  // and watch plugins by default. Other plugins
  // can be attached through 'monitor.use(plugin, options)'.
  //
  function bootstrap(monitor) {
    plugins.logger.attach.call(monitor, options);
    if (options.watch) {
      plugins.watch.attach.call(monitor, options);
    }
  }

  var execPath = process.execPath,
      self     = this;

  //
  // Setup basic configuration options
  //
  options               = options || {};
  this.silent           = options.silent || false;
  this.killTree         = options.killTree !== false;
  this.uid              = options.uid || utile.randomString(4);
  this.id               = options.id || false;
  this.pidFile          = options.pidFile;
  this.max              = options.max;
  this.killTTL          = options.killTTL;
  this.killSignal       = options.killSignal || 'SIGKILL';
  this.childExists      = false;
  this.checkFile        = options.checkFile !== false;
  this.times            = 0;
  this.warn             = console.error;

  this.logFile          = options.logFile;
  this.outFile          = options.outFile;
  this.errFile          = options.errFile;
  this.append           = options.append;
  this.usePolling       = options.usePolling;
  this.pollingInterval  = options.pollingInterval;

  //
  // Define some safety checks for commands with spaces
  //
  this.parser = options.parser || Monitor.parseCommand;

  //
  // Setup restart timing. These options control how quickly forever restarts
  // a child process as well as when to kill a "spinning" process
  //
  this.minUptime     = typeof options.minUptime !== 'number' ? 0 : options.minUptime;
  this.spinSleepTime = options.spinSleepTime || null;

  //
  // Special case Windows separately to decouple any
  // future changes
  //
  if (process.platform === 'win32') {
    execPath = '"' + execPath + '"';
  }

  if (options.options) {
    console.warn('options.options is deprecated. Use options.args instead.');
  }

  //
  // Setup the command to spawn and the options to pass
  // to that command.
  //
  this.command   = options.command || execPath;
  this.args      = options.args || options.options || [];
  this.spawnWith = options.spawnWith || {};
  this.sourceDir = options.sourceDir;
  this.fork      = options.fork || false;
  this.cwd       = options.cwd || process.cwd();
  this.hideEnv   = options.hideEnv || [];
  this._env      = options.env || {};
  this._hideEnv  = {};

  //
  // Allow for custom stdio configuration of forked processes
  //
  this.stdio = options.stdio || null;

  //
  // Setup watch configuration options
  //
  this.watchIgnoreDotFiles = options.watchIgnoreDotFiles !== false;
  this.watchIgnorePatterns = options.watchIgnorePatterns || [];
  this.watchDirectory      = options.watchDirectory || this.sourceDir;

  //
  // Create a simple mapping of 'this.hideEnv' to an easily indexable
  // object
  //
  this.hideEnv.forEach(function (key) {
    self._hideEnv[key] = true;
  });

  if (Array.isArray(script)) {
    this.command = script[0];
    this.args = script.slice(1);
  }
  else {
    this.args.unshift(script);
  }

  if (this.sourceDir) {
    this.args[0] = path.join(this.sourceDir, this.args[0]);
  }

  //
  // Bootstrap this instance now that options
  // have been set
  //
  broadway.App.call(this, { bootstrapper: { bootstrap: bootstrap } });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.parseCommand"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.</span>parseCommand (command, args)](#apidoc.element.forever-monitor.Monitor.parseCommand)
- description and source-code
```javascript
parseCommand = function (command, args) {
  var match = command.match(
    process.platform === 'win32' ? safetyChecks.windows : safetyChecks.linux
  );

  //
  // No match means it's a bad command. This is configurable
  // by passing a custom 'parser' function into the 'Monitor'
  // constructor function.
  //
  if (!match) { return false; }

  if (process.platform == 'win32') {
    command = match[1] || match[2];
    if (match[3]) {
      args = match[3].split(' ').concat(args);
    }
  } else {
    command = match[1];
    if (match[2]) {
      args = match[2].split(' ').concat(this.args);
    }
  }

  return {
    command: command,
    args:    args
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.</span>super_ (options)](#apidoc.element.forever-monitor.Monitor.super_)
- description and source-code
```javascript
super_ = function (options) {
  //
  // Setup options and 'App' constants.
  //
  options        = options || {};
  this.root      = options.root;
  this.delimiter = options.delimiter || '::';

  //
  // Inherit from 'EventEmitter2'
  //
  events.EventEmitter2.call(this, {
    delimiter: this.delimiter,
    wildcard: true
  });

  //
  // Setup other relevant options such as the plugins
  // for this instance.
  //
  this.options      = options;
  this.env          = options.env || process.env['NODE_ENV'] || 'development'
  this.plugins      = options.plugins || {};
  this.initialized  = false;
  this.bootstrapper = options.bootstrapper || bootstrapper;
  this.initializers = {};
  this.initlist     = [];

  //
  // Bootstrap this instance
  //
  this.bootstrapper.bootstrap(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever-monitor.Monitor.prototype"></a>[module forever-monitor.Monitor.prototype](#apidoc.module.forever-monitor.Monitor.prototype)

#### <a name="apidoc.element.forever-monitor.Monitor.prototype._getEnv"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>_getEnv ()](#apidoc.element.forever-monitor.Monitor.prototype._getEnv)
- description and source-code
```javascript
_getEnv = function () {
  var self = this,
      merged = {};

  function addKey(key, source) {
    merged[key] = source[key];
  }

  //
  // Mixin the key:value pairs from 'process.env' and the custom
  // environment variables in 'this._env'.
  //
  Object.keys(process.env).forEach(function (key) {
    if (!self._hideEnv[key]) {
      addKey(key, process.env);
    }
  });

  Object.keys(this._env).forEach(function (key) {
    addKey(key, self._env);
  });

  return merged;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.kill"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>kill (forceStop)](#apidoc.element.forever-monitor.Monitor.prototype.kill)
- description and source-code
```javascript
kill = function (forceStop) {
  var child = this.child,
      self = this,
      timer;

  if (!child || (!this.running && !this.forceRestart)) {
    process.nextTick(function () {
      self.emit('error', new Error('Cannot stop process that is not running.'));
    });
  }
  else {
    //
    // Set an instance variable here to indicate this
    // stoppage is forced so that when 'child.on('exit', ..)'
    // fires in 'Monitor.prototype.start' we can short circuit
    // and prevent auto-restart
    //
    if (forceStop) {
      this.forceStop = true;
      //
      // If we have a time before we truly kill forcefully, set up a timer
      //
      if (this.killTTL) {
        timer = setTimeout(function () {
          common.kill(self.child.pid, self.killTree, self.killSignal || 'SIGKILL');
        }, this.killTTL);

        child.once('exit', function () {
          clearTimeout(timer);
        });
      }
    }

    child.once('exit', function () {
      self.emit('stop', self.childData);
      if (self.forceRestart && !self.running) {
        self.start(true);
      }
    });

    common.kill(this.child.pid, this.killTree, this.killSignal);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.restart"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>restart ()](#apidoc.element.forever-monitor.Monitor.prototype.restart)
- description and source-code
```javascript
restart = function () {
  this.times = this.times || 0;
  this.forceRestart = true;

  return !this.running
    ? this.start(true)
    : this.kill(false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.send"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>send (msg)](#apidoc.element.forever-monitor.Monitor.prototype.send)
- description and source-code
```javascript
send = function (msg) {
  var child = this.child,
      self = this;

  if (!child || !this.running) {
    process.nextTick(function () {
      self.emit('error', new Error('Cannot send to process that is not running.'));
    });
  }

  if (child.send) { child.send(msg) }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.start"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>start (restart)](#apidoc.element.forever-monitor.Monitor.prototype.start)
- description and source-code
```javascript
start = function (restart) {
  var self = this,
      child;

  if (this.running && !restart) {
    process.nextTick(function () {
      self.emit('error', new Error('Cannot start process that is already running.'));
    });
    return this;
  }

  child = this.trySpawn();
  if (!child) {
    process.nextTick(function () {
      self.emit('error', new Error('Target script does not exist: ' + self.args[0]));
    });
    return this;
  }

  this.ctime = Date.now();
  this.child = child;
  this.running = true;
  this.isMaster = cluster.isMaster;

  process.nextTick(function () {
    self.emit(restart ? 'restart' : 'start', self, self.data);
  });

  function onMessage(msg) {
    self.emit('message', msg);
  }

  // Re-emit messages from the child process
  this.child.on('message', onMessage);

  child.on('exit', function (code, signal) {
    var spinning = Date.now() - self.ctime < self.minUptime;
    child.removeListener('message', onMessage);
    self.emit('exit:code', code, signal);

    function letChildDie() {
      self.running = false;
      self.forceStop = false;
      self.emit('exit', self, spinning);
    }

    function restartChild() {
      self.forceRestart = false;
      process.nextTick(function () {
        self.start(true);
      });
    }

    self.times++;

    if (self.forceStop || (self.times >= self.max && !self.forceRestart)
      || (spinning && typeof self.spinSleepTime !== 'number') && !self.forceRestart) {
      letChildDie();
    }
    else if (spinning) {
      setTimeout(restartChild, self.spinSleepTime);
    }
    else {
      restartChild();
    }
  });

  return this;
}
```
- example usage
```shell
...
    args: []
  });

  child.on('exit', function () {
    console.log('your-filename.js has exited after 3 restarts');
  });

  child.start();
'''

### Spawning a non-node process
You can spawn non-node processes too. Either set the 'command' key in the
'options' hash or pass in an 'Array' in place of the 'file' argument like this:

''' js
...
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.stop"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>stop ()](#apidoc.element.forever-monitor.Monitor.prototype.stop)
- description and source-code
```javascript
stop = function () {
  return this.kill(true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.toString"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>toString ()](#apidoc.element.forever-monitor.Monitor.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.prototype.trySpawn"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.prototype.</span>trySpawn ()](#apidoc.element.forever-monitor.Monitor.prototype.trySpawn)
- description and source-code
```javascript
trySpawn = function () {
  var run = this.parser(this.command, this.args.slice()),
      stats;

  if (/[^\w]node$/.test(this.command) && this.checkFile && !this.childExists) {
    try {
      stats = fs.statSync(this.args[0]);
      this.childExists = true;
    }
    catch (ex) {
      return false;
    }
  }

  this.spawnWith.cwd = this.spawnWith.cwd || this.cwd;
  this.spawnWith.env = this._getEnv();

  if (process.platform === 'win32') {
    this.spawnWith.detached = true;
  }

  if (this.stdio) {
    this.spawnWith.stdio = this.stdio;
  }

  if (this.fork) {
    if (!this.stdio) {
      this.spawnWith.stdio = [ 'pipe', 'pipe', 'pipe', 'ipc' ];
    }
    return spawn(run.command, run.args, this.spawnWith);
  }

  return spawn(run.command, run.args, this.spawnWith);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever-monitor.Monitor.super_"></a>[module forever-monitor.Monitor.super_](#apidoc.module.forever-monitor.Monitor.super_)

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.</span>super_ (conf)](#apidoc.element.forever-monitor.Monitor.super_.super_)
- description and source-code
```javascript
function EventEmitter(conf) {
  this._events = {};
  this.newListener = false;
  configure.call(this, conf);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever-monitor.Monitor.super_.prototype"></a>[module forever-monitor.Monitor.super_.prototype](#apidoc.module.forever-monitor.Monitor.super_.prototype)

#### <a name="apidoc.element.forever-monitor.Monitor.super_.prototype.init"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>init (options, callback)](#apidoc.element.forever-monitor.Monitor.super_.prototype.init)
- description and source-code
```javascript
init = function (options, callback) {
  if (!callback && typeof options === 'function') {
    callback = options;
    options = {};
  }

  if (this.initialized) {
    return callback();
  }

  var self = this;
  options = options   || {};
  callback = callback || function () {};
  this.env = options.env || this.env;
  this.options = common.mixin({}, this.options, options);

  function onComplete() {
    self.initialized = true;
    self.emit('init');
    callback();
  }

  function ensureFeatures (err) {
    return err
      ? onError(err)
      : features.ensure(this, onComplete);
  }

  function initPlugin(plugin, next) {
    if (typeof self.initializers[plugin] === 'function') {
      return self.initializers[plugin].call(self, function (err) {
        if (err) {
          return next(err);
        }

        self.emit(['plugin', plugin, 'init']);
        self.initializers[plugin] = true;
        next();
      });
    }

    next();
  }

  function initPlugins() {
    async.forEach(self.initlist, initPlugin, ensureFeatures);
  }

  //
  // Emit and respond with any errors that may short
  // circuit the process.
  //
  function onError(err) {
    self.emit(['error', 'init'], err);
    callback(err);
  }

  //
  // Run the bootstrapper, initialize plugins, and
  // ensure features for this instance.
  //
  this.bootstrapper.init(this, initPlugins);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.prototype.inspect"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>inspect ()](#apidoc.element.forever-monitor.Monitor.super_.prototype.inspect)
- description and source-code
```javascript
inspect = function () {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.prototype.remove"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>remove (name)](#apidoc.element.forever-monitor.Monitor.super_.prototype.remove)
- description and source-code
```javascript
remove = function (name) {
  // if this is a plugin object set the name to the plugins name
  if (name.name) {
    name = name.name;
  }

  if (this.plugins[name] && this.plugins[name].detach) {
    this.plugins[name].detach.call(this);
  }

  delete this.plugins[name];
  delete this.options[name];
  delete this.initializers[name];

  var init = this.initlist.indexOf(name);

  if (init !== -1) {
    this.initlist.splice(1, init);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.prototype.use"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.prototype.</span>use (plugin, options, callback)](#apidoc.element.forever-monitor.Monitor.super_.prototype.use)
- description and source-code
```javascript
use = function (plugin, options, callback) {
  options = options || {};

  if (typeof plugin === 'undefined') {
    console.log('Cannot load invalid plugin!');
    return callback && callback(new Error('Invalid plugin'));
  }

  var name = plugin.name,
      self = this;

  // If the plugin doesn't have a name, use itself as an identifier for the plugins hash.
  if (!name) {
    name = common.uuid();
  }

  if (this.plugins[name]) {
    return callback && callback();
  }

  //
  // Setup state on this instance for the specified plugin
  //
  this.plugins[name] = plugin;
  this.options[name] = common.mixin({}, options, this.options[name] || {});

  //
  // Attach the specified plugin to this instance, extending
  // the 'App' with new functionality.
  //
  if (this.plugins[name].attach && options.attach !== false) {
    this.plugins[name].attach.call(this, options);
  }

  //
  // Setup the initializer only if 'options.init' is
  // not false. This allows for some plugins to be lazy-loaded
  //
  if (options.init === false) {
    return callback && callback();
  }

  if (!this.initialized) {
    this.initializers[name] = plugin.init || true;
    this.initlist.push(name);
    return callback && callback();
  }
  else if (plugin.init) {
    plugin.init.call(this, function (err) {
      var args = err
        ? [['plugin', name, 'error'], err]
        : [['plugin', name, 'init']];

      self.emit.apply(self, args);
      return callback && (err ? callback(err) : callback());
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever-monitor.Monitor.super_.super_.prototype"></a>[module forever-monitor.Monitor.super_.super_.prototype](#apidoc.module.forever-monitor.Monitor.super_.super_.prototype)

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>addListener (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (type, listener) {

  if (typeof type === 'function') {
    this.onAny(type);
    return this;
  }

  if (typeof listener !== 'function') {
    throw new Error('on only accepts instances of Function');
  }
  this._events || init.call(this);

  // To avoid recursion in the case that type == "newListeners"! Before
  // adding it to the listeners, first emit "newListeners".
  this.emit('newListener', type, listener);

  if(this.wildcard) {
    growListenerTree.call(this, type, listener);
    return this;
  }

  if (!this._events[type]) {
    // Optimize the case of one listener. Don't need the extra array object.
    this._events[type] = listener;
  }
  else if(typeof this._events[type] === 'function') {
    // Adding the second element, need to change to array.
    this._events[type] = [this._events[type], listener];
  }
  else if (isArray(this._events[type])) {
    // If we've already got an array, just append.
    this._events[type].push(listener);

    // Check for listener leak
    if (!this._events[type].warned) {

      var m = defaultMaxListeners;

      if (typeof this._events.maxListeners !== 'undefined') {
        m = this._events.maxListeners;
      }

      if (m > 0 && this._events[type].length > m) {

        this._events[type].warned = true;
        console.error('(node) warning: possible EventEmitter memory ' +
                      'leak detected. %d listeners added. ' +
                      'Use emitter.setMaxListeners() to increase limit.',
                      this._events[type].length);
        console.trace();
      }
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.emit"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>emit ()](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.emit)
- description and source-code
```javascript
emit = function () {

  this._events || init.call(this);

  var type = arguments[0];

  if (type === 'newListener' && !this.newListener) {
    if (!this._events.newListener) { return false; }
  }

  // Loop through the *_all* functions and invoke them.
  if (this._all) {
    var l = arguments.length;
    var args = new Array(l - 1);
    for (var i = 1; i < l; i++) args[i - 1] = arguments[i];
    for (i = 0, l = this._all.length; i < l; i++) {
      this.event = type;
      this._all[i].apply(this, args);
    }
  }

  // If there is no 'error' event listener then throw.
  if (type === 'error') {

    if (!this._all &&
      !this._events.error &&
      !(this.wildcard && this.listenerTree.error)) {

      if (arguments[1] instanceof Error) {
        throw arguments[1]; // Unhandled 'error' event
      } else {
        throw new Error("Uncaught, unspecified 'error' event.");
      }
      return false;
    }
  }

  var handler;

  if(this.wildcard) {
    handler = [];
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    searchListenerTree.call(this, handler, ns, this.listenerTree, 0);
  }
  else {
    handler = this._events[type];
  }

  if (typeof handler === 'function') {
    this.event = type;
    if (arguments.length === 1) {
      handler.call(this);
    }
    else if (arguments.length > 1)
      switch (arguments.length) {
        case 2:
          handler.call(this, arguments[1]);
          break;
        case 3:
          handler.call(this, arguments[1], arguments[2]);
          break;
        // slower
        default:
          var l = arguments.length;
          var args = new Array(l - 1);
          for (var i = 1; i < l; i++) args[i - 1] = arguments[i];
          handler.apply(this, args);
      }
    return true;
  }
  else if (handler) {
    var l = arguments.length;
    var args = new Array(l - 1);
    for (var i = 1; i < l; i++) args[i - 1] = arguments[i];

    var listeners = handler.slice();
    for (var i = 0, l = listeners.length; i < l; i++) {
      this.event = type;
      listeners[i].apply(this, args);
    }
    return (listeners.length > 0) || !!this._all;
  }
  else {
    return !!this._all;
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.listeners"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>listeners (type)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.listeners)
- description and source-code
```javascript
listeners = function (type) {
  if(this.wildcard) {
    var handlers = [];
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    searchListenerTree.call(this, handlers, ns, this.listenerTree, 0);
    return handlers;
  }

  this._events || init.call(this);

  if (!this._events[type]) this._events[type] = [];
  if (!isArray(this._events[type])) {
    this._events[type] = [this._events[type]];
  }
  return this._events[type];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.listenersAny"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>listenersAny ()](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.listenersAny)
- description and source-code
```javascript
listenersAny = function () {

  if(this._all) {
    return this._all;
  }
  else {
    return [];
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.many"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>many (event, ttl, fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.many)
- description and source-code
```javascript
many = function (event, ttl, fn) {
  var self = this;

  if (typeof fn !== 'function') {
    throw new Error('many only accepts instances of Function');
  }

  function listener() {
    if (--ttl === 0) {
      self.off(event, listener);
    }
    fn.apply(this, arguments);
  }

  listener._origin = fn;

  this.on(event, listener);

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.off"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>off (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.off)
- description and source-code
```javascript
off = function (type, listener) {
  if (typeof listener !== 'function') {
    throw new Error('removeListener only takes instances of Function');
  }

  var handlers,leafs=[];

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);
  }
  else {
    // does not use listeners(), so no side effect of creating _events[type]
    if (!this._events[type]) return this;
    handlers = this._events[type];
    leafs.push({_listeners:handlers});
  }

  for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
    var leaf = leafs[iLeaf];
    handlers = leaf._listeners;
    if (isArray(handlers)) {

      var position = -1;

      for (var i = 0, length = handlers.length; i < length; i++) {
        if (handlers[i] === listener ||
          (handlers[i].listener && handlers[i].listener === listener) ||
          (handlers[i]._origin && handlers[i]._origin === listener)) {
          position = i;
          break;
        }
      }

      if (position < 0) {
        continue;
      }

      if(this.wildcard) {
        leaf._listeners.splice(position, 1);
      }
      else {
        this._events[type].splice(position, 1);
      }

      if (handlers.length === 0) {
        if(this.wildcard) {
          delete leaf._listeners;
        }
        else {
          delete this._events[type];
        }
      }
      return this;
    }
    else if (handlers === listener ||
      (handlers.listener && handlers.listener === listener) ||
      (handlers._origin && handlers._origin === listener)) {
      if(this.wildcard) {
        delete leaf._listeners;
      }
      else {
        delete this._events[type];
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.offAny"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>offAny (fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.offAny)
- description and source-code
```javascript
offAny = function (fn) {
  var i = 0, l = 0, fns;
  if (fn && this._all && this._all.length > 0) {
    fns = this._all;
    for(i = 0, l = fns.length; i < l; i++) {
      if(fn === fns[i]) {
        fns.splice(i, 1);
        return this;
      }
    }
  } else {
    this._all = [];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>on (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (type, listener) {

  if (typeof type === 'function') {
    this.onAny(type);
    return this;
  }

  if (typeof listener !== 'function') {
    throw new Error('on only accepts instances of Function');
  }
  this._events || init.call(this);

  // To avoid recursion in the case that type == "newListeners"! Before
  // adding it to the listeners, first emit "newListeners".
  this.emit('newListener', type, listener);

  if(this.wildcard) {
    growListenerTree.call(this, type, listener);
    return this;
  }

  if (!this._events[type]) {
    // Optimize the case of one listener. Don't need the extra array object.
    this._events[type] = listener;
  }
  else if(typeof this._events[type] === 'function') {
    // Adding the second element, need to change to array.
    this._events[type] = [this._events[type], listener];
  }
  else if (isArray(this._events[type])) {
    // If we've already got an array, just append.
    this._events[type].push(listener);

    // Check for listener leak
    if (!this._events[type].warned) {

      var m = defaultMaxListeners;

      if (typeof this._events.maxListeners !== 'undefined') {
        m = this._events.maxListeners;
      }

      if (m > 0 && this._events[type].length > m) {

        this._events[type].warned = true;
        console.error('(node) warning: possible EventEmitter memory ' +
                      'leak detected. %d listeners added. ' +
                      'Use emitter.setMaxListeners() to increase limit.',
                      this._events[type].length);
        console.trace();
      }
    }
  }
  return this;
}
```
- example usage
```shell
...

  var child = new (forever.Monitor)('your-filename.js', {
    max: 3,
    silent: true,
    args: []
  });

  child.on('exit', function () {
    console.log('your-filename.js has exited after 3 restarts');
  });

  child.start();
'''

### Spawning a non-node process
...
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.onAny"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>onAny (fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.onAny)
- description and source-code
```javascript
onAny = function (fn) {

  if (typeof fn !== 'function') {
    throw new Error('onAny only accepts instances of Function');
  }

  if(!this._all) {
    this._all = [];
  }

  // Add the function to the event listener collection.
  this._all.push(fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.once"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>once (event, fn)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.once)
- description and source-code
```javascript
once = function (event, fn) {
  this.many(event, 1, fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>removeAllListeners (type)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function (type) {
  if (arguments.length === 0) {
    !this._events || init.call(this);
    return this;
  }

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    var leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);

    for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
      var leaf = leafs[iLeaf];
      leaf._listeners = null;
    }
  }
  else {
    if (!this._events[type]) return this;
    this._events[type] = null;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>removeListener (type, listener)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (type, listener) {
  if (typeof listener !== 'function') {
    throw new Error('removeListener only takes instances of Function');
  }

  var handlers,leafs=[];

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);
  }
  else {
    // does not use listeners(), so no side effect of creating _events[type]
    if (!this._events[type]) return this;
    handlers = this._events[type];
    leafs.push({_listeners:handlers});
  }

  for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
    var leaf = leafs[iLeaf];
    handlers = leaf._listeners;
    if (isArray(handlers)) {

      var position = -1;

      for (var i = 0, length = handlers.length; i < length; i++) {
        if (handlers[i] === listener ||
          (handlers[i].listener && handlers[i].listener === listener) ||
          (handlers[i]._origin && handlers[i]._origin === listener)) {
          position = i;
          break;
        }
      }

      if (position < 0) {
        continue;
      }

      if(this.wildcard) {
        leaf._listeners.splice(position, 1);
      }
      else {
        this._events[type].splice(position, 1);
      }

      if (handlers.length === 0) {
        if(this.wildcard) {
          delete leaf._listeners;
        }
        else {
          delete this._events[type];
        }
      }
      return this;
    }
    else if (handlers === listener ||
      (handlers.listener && handlers.listener === listener) ||
      (handlers._origin && handlers._origin === listener)) {
      if(this.wildcard) {
        delete leaf._listeners;
      }
      else {
        delete this._events[type];
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever-monitor.Monitor.super_.super_.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">forever-monitor.Monitor.super_.super_.prototype.</span>setMaxListeners (n)](#apidoc.element.forever-monitor.Monitor.super_.super_.prototype.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function (n) {
  this._events || init.call(this);
  this._events.maxListeners = n;
  if (!this._conf) this._conf = {};
  this._conf.maxListeners = n;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
