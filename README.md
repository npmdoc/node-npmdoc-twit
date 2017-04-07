# api documentation for  [twit (v2.2.5)](https://github.com/ttezel/twit)  [![npm package](https://img.shields.io/npm/v/npmdoc-twit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-twit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-twit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-twit)
#### Twitter API client for node (REST & Streaming)

[![NPM](https://nodei.co/npm/twit.png?downloads=true)](https://www.npmjs.com/package/twit)

[![apidoc](https://npmdoc.github.io/node-npmdoc-twit/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-twit%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-twit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-twit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-twit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tolga Tezel"
    },
    "bugs": {
        "url": "https://github.com/ttezel/twit/issues"
    },
    "dependencies": {
        "bluebird": "^3.1.5",
        "mime": "^1.3.4",
        "request": "^2.68.0"
    },
    "description": "Twitter API client for node (REST & Streaming)",
    "devDependencies": {
        "async": "0.2.9",
        "colors": "0.6.x",
        "commander": "2.6.0",
        "mocha": "2.1.0",
        "rewire": "2.3.4",
        "sinon": "1.15.4"
    },
    "directories": {},
    "dist": {
        "shasum": "241480bab71731162d2a87b27450e4aa3bb5be5f",
        "tarball": "https://registry.npmjs.org/twit/-/twit-2.2.5.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "fa4d346fd564220e5dc41e8866fad3abb74b6479",
    "homepage": "https://github.com/ttezel/twit",
    "keywords": [
        "twitter",
        "api",
        "rest",
        "stream",
        "streaming",
        "oauth"
    ],
    "license": "MIT",
    "main": "./lib/twitter",
    "maintainers": [
        {
            "name": "ttezel",
            "email": "tolgatezel11@gmail.com"
        }
    ],
    "name": "twit",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/ttezel/twit.git"
    },
    "scripts": {
        "test": "mocha tests/* -t 70000 -R spec --bail --globals domain,_events,_maxListeners"
    },
    "version": "2.2.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module twit](#apidoc.module.twit)
1.  [function <span class="apidocSignatureSpan">twit.</span>file_uploader (params, twit)](#apidoc.element.twit.file_uploader)
1.  [function <span class="apidocSignatureSpan">twit.</span>parser ()](#apidoc.element.twit.parser)
1.  [function <span class="apidocSignatureSpan">twit.</span>streaming_api_connection (reqOpts, twitOptions)](#apidoc.element.twit.streaming_api_connection)
1.  object <span class="apidocSignatureSpan">twit.</span>file_uploader.prototype
1.  object <span class="apidocSignatureSpan">twit.</span>helpers
1.  object <span class="apidocSignatureSpan">twit.</span>parser.prototype
1.  object <span class="apidocSignatureSpan">twit.</span>streaming_api_connection.prototype

#### [module twit.file_uploader](#apidoc.module.twit.file_uploader)
1.  [function <span class="apidocSignatureSpan">twit.</span>file_uploader (params, twit)](#apidoc.element.twit.file_uploader.file_uploader)

#### [module twit.file_uploader.prototype](#apidoc.module.twit.file_uploader.prototype)
1.  [function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_appendMedia (media_id_string, chunk_part, segment_index, cb)](#apidoc.element.twit.file_uploader.prototype._appendMedia)
1.  [function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_finalizeMedia (media_id, cb)](#apidoc.element.twit.file_uploader.prototype._finalizeMedia)
1.  [function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_initMedia (cb)](#apidoc.element.twit.file_uploader.prototype._initMedia)
1.  [function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_isUploadComplete ()](#apidoc.element.twit.file_uploader.prototype._isUploadComplete)
1.  [function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>upload (cb)](#apidoc.element.twit.file_uploader.prototype.upload)

#### [module twit.helpers](#apidoc.module.twit.helpers)
1.  [function <span class="apidocSignatureSpan">twit.helpers.</span>attachBodyInfoToError (err, body)](#apidoc.element.twit.helpers.attachBodyInfoToError)
1.  [function <span class="apidocSignatureSpan">twit.helpers.</span>getBearerToken (consumer_key, consumer_secret, cb)](#apidoc.element.twit.helpers.getBearerToken)
1.  [function <span class="apidocSignatureSpan">twit.helpers.</span>makeQueryString (obj)](#apidoc.element.twit.helpers.makeQueryString)
1.  [function <span class="apidocSignatureSpan">twit.helpers.</span>makeTwitError (message)](#apidoc.element.twit.helpers.makeTwitError)
1.  [function <span class="apidocSignatureSpan">twit.helpers.</span>moveParamsIntoPath (params, path)](#apidoc.element.twit.helpers.moveParamsIntoPath)

#### [module twit.parser](#apidoc.module.twit.parser)
1.  [function <span class="apidocSignatureSpan">twit.</span>parser ()](#apidoc.element.twit.parser.parser)
1.  [function <span class="apidocSignatureSpan">twit.parser.</span>super_ ()](#apidoc.element.twit.parser.super_)

#### [module twit.parser.prototype](#apidoc.module.twit.parser.prototype)
1.  [function <span class="apidocSignatureSpan">twit.parser.prototype.</span>parse (chunk)](#apidoc.element.twit.parser.prototype.parse)

#### [module twit.streaming_api_connection](#apidoc.module.twit.streaming_api_connection)
1.  [function <span class="apidocSignatureSpan">twit.</span>streaming_api_connection (reqOpts, twitOptions)](#apidoc.element.twit.streaming_api_connection.streaming_api_connection)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.</span>super_ ()](#apidoc.element.twit.streaming_api_connection.super_)

#### [module twit.streaming_api_connection.prototype](#apidoc.module.twit.streaming_api_connection.prototype)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_handleDisconnect (twitterMsg)](#apidoc.element.twit.streaming_api_connection.prototype._handleDisconnect)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_onClose ()](#apidoc.element.twit.streaming_api_connection.prototype._onClose)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_resetConnection ()](#apidoc.element.twit.streaming_api_connection.prototype._resetConnection)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_resetRetryParams ()](#apidoc.element.twit.streaming_api_connection.prototype._resetRetryParams)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_resetStallAbortTimeout ()](#apidoc.element.twit.streaming_api_connection.prototype._resetStallAbortTimeout)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_scheduleReconnect ()](#apidoc.element.twit.streaming_api_connection.prototype._scheduleReconnect)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_setOauthTimestamp ()](#apidoc.element.twit.streaming_api_connection.prototype._setOauthTimestamp)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_setupParser ()](#apidoc.element.twit.streaming_api_connection.prototype._setupParser)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_startPersistentConnection ()](#apidoc.element.twit.streaming_api_connection.prototype._startPersistentConnection)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_stopStallAbortTimeout ()](#apidoc.element.twit.streaming_api_connection.prototype._stopStallAbortTimeout)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_updateOauthTimestampOffsetFromResponse (resp)](#apidoc.element.twit.streaming_api_connection.prototype._updateOauthTimestampOffsetFromResponse)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>start ()](#apidoc.element.twit.streaming_api_connection.prototype.start)
1.  [function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>stop ()](#apidoc.element.twit.streaming_api_connection.prototype.stop)



# <a name="apidoc.module.twit"></a>[module twit](#apidoc.module.twit)

#### <a name="apidoc.element.twit.file_uploader"></a>[function <span class="apidocSignatureSpan">twit.</span>file_uploader (params, twit)](#apidoc.element.twit.file_uploader)
- description and source-code
```javascript
file_uploader = function (params, twit) {
  assert(params)
  assert(params.file_path, 'Must specify 'file_path' to upload a file. Got: ' + params.file_path + '.')
  var self = this;
  self._file_path = params.file_path;
  self._twit = twit;
  self._isUploading = false;
  self._isFileStreamEnded = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.parser"></a>[function <span class="apidocSignatureSpan">twit.</span>parser ()](#apidoc.element.twit.parser)
- description and source-code
```javascript
parser = function ()  {
  this.message = ''

  EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.streaming_api_connection"></a>[function <span class="apidocSignatureSpan">twit.</span>streaming_api_connection (reqOpts, twitOptions)](#apidoc.element.twit.streaming_api_connection)
- description and source-code
```javascript
streaming_api_connection = function (reqOpts, twitOptions) {
  this.reqOpts = reqOpts
  this.twitOptions = twitOptions
  this._twitter_time_minus_local_time_ms = 0
  EventEmitter.call(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.twit.file_uploader"></a>[module twit.file_uploader](#apidoc.module.twit.file_uploader)

#### <a name="apidoc.element.twit.file_uploader.file_uploader"></a>[function <span class="apidocSignatureSpan">twit.</span>file_uploader (params, twit)](#apidoc.element.twit.file_uploader.file_uploader)
- description and source-code
```javascript
file_uploader = function (params, twit) {
  assert(params)
  assert(params.file_path, 'Must specify 'file_path' to upload a file. Got: ' + params.file_path + '.')
  var self = this;
  self._file_path = params.file_path;
  self._twit = twit;
  self._isUploading = false;
  self._isFileStreamEnded = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.twit.file_uploader.prototype"></a>[module twit.file_uploader.prototype](#apidoc.module.twit.file_uploader.prototype)

#### <a name="apidoc.element.twit.file_uploader.prototype._appendMedia"></a>[function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_appendMedia (media_id_string, chunk_part, segment_index, cb)](#apidoc.element.twit.file_uploader.prototype._appendMedia)
- description and source-code
```javascript
_appendMedia = function (media_id_string, chunk_part, segment_index, cb) {
  var self = this;
  self._twit.post('media/upload', {
    command: 'APPEND',
    media_id: media_id_string.toString(),
    segment_index: segment_index,
    media: chunk_part,
  }, cb);
}
```
- example usage
```shell
...

      mediaFile.on('data', function (chunk) {
// Pause our file stream from emitting 'data' events until the upload of this chunk completes.
// Any data that becomes available will remain in the internal buffer.
mediaFile.pause();
self._isUploading = true;

self._appendMedia(mediaTmpId, chunk.toString('base64'), chunkNumber, function (err, bodyObj, resp) {
  self._isUploading = false;
  if (err) {
    cb(err);
  } else {
    if (self._isUploadComplete()) {
      // We've hit the end of our stream; send FINALIZE command.
      self._finalizeMedia(mediaTmpId, cb);
...
```

#### <a name="apidoc.element.twit.file_uploader.prototype._finalizeMedia"></a>[function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_finalizeMedia (media_id, cb)](#apidoc.element.twit.file_uploader.prototype._finalizeMedia)
- description and source-code
```javascript
_finalizeMedia = function (media_id, cb) {
  var self = this;
  self._twit.post('media/upload', {
    command: 'FINALIZE',
    media_id: media_id
  }, cb);
}
```
- example usage
```shell
...
self._appendMedia(mediaTmpId, chunk.toString('base64'), chunkNumber, function (err, bodyObj, resp) {
  self._isUploading = false;
  if (err) {
    cb(err);
  } else {
    if (self._isUploadComplete()) {
      // We've hit the end of our stream; send FINALIZE command.
      self._finalizeMedia(mediaTmpId, cb);
    } else {
      // Tell our file stream to start emitting 'data' events again.
      chunkNumber++;
      mediaFile.resume();
    }
  }
});
...
```

#### <a name="apidoc.element.twit.file_uploader.prototype._initMedia"></a>[function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_initMedia (cb)](#apidoc.element.twit.file_uploader.prototype._initMedia)
- description and source-code
```javascript
_initMedia = function (cb) {
  var self = this;
  var mediaType = mime.lookup(self._file_path);
  var mediaFileSizeBytes = fs.statSync(self._file_path).size;

  // Check the file size - it should not go over 15MB for video.
  // See https://dev.twitter.com/rest/reference/post/media/upload-chunked
  if (mediaFileSizeBytes < MAX_FILE_SIZE_BYTES) {
    self._twit.post('media/upload', {
      'command': 'INIT',
      'media_type': mediaType,
      'total_bytes': mediaFileSizeBytes
    }, cb);
  } else {
    var errMsg = util.format('This file is too large. Max size is %dB. Got: %dB.', MAX_FILE_SIZE_BYTES, mediaFileSizeBytes);
    cb(new Error(errMsg));
  }
}
```
- example usage
```shell
...
 *
 * @param  {Function} cb function (err, data, resp)
 */
FileUploader.prototype.upload = function (cb) {
var self = this;

// Send INIT command with file info and get back a media_id_string we can use to APPEND chunks to it.
self._initMedia(function (err, bodyObj, resp) {
  if (err) {
    cb(err);
    return;
  } else {
    var mediaTmpId = bodyObj.media_id_string;
    var chunkNumber = 0;
    var mediaFile = fs.createReadStream(self._file_path, { highWatermark: MAX_FILE_CHUNK_BYTES });
...
```

#### <a name="apidoc.element.twit.file_uploader.prototype._isUploadComplete"></a>[function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>_isUploadComplete ()](#apidoc.element.twit.file_uploader.prototype._isUploadComplete)
- description and source-code
```javascript
_isUploadComplete = function () {
  return !this._isUploading && this._isFileStreamEnded;
}
```
- example usage
```shell
...
self._isUploading = true;

self._appendMedia(mediaTmpId, chunk.toString('base64'), chunkNumber, function (err, bodyObj, resp) {
  self._isUploading = false;
  if (err) {
    cb(err);
  } else {
    if (self._isUploadComplete()) {
      // We've hit the end of our stream; send FINALIZE command.
      self._finalizeMedia(mediaTmpId, cb);
    } else {
      // Tell our file stream to start emitting 'data' events again.
      chunkNumber++;
      mediaFile.resume();
    }
...
```

#### <a name="apidoc.element.twit.file_uploader.prototype.upload"></a>[function <span class="apidocSignatureSpan">twit.file_uploader.prototype.</span>upload (cb)](#apidoc.element.twit.file_uploader.prototype.upload)
- description and source-code
```javascript
upload = function (cb) {
  var self = this;

  // Send INIT command with file info and get back a media_id_string we can use to APPEND chunks to it.
  self._initMedia(function (err, bodyObj, resp) {
    if (err) {
      cb(err);
      return;
    } else {
      var mediaTmpId = bodyObj.media_id_string;
      var chunkNumber = 0;
      var mediaFile = fs.createReadStream(self._file_path, { highWatermark: MAX_FILE_CHUNK_BYTES });

      mediaFile.on('data', function (chunk) {
        // Pause our file stream from emitting 'data' events until the upload of this chunk completes.
        // Any data that becomes available will remain in the internal buffer.
        mediaFile.pause();
        self._isUploading = true;

        self._appendMedia(mediaTmpId, chunk.toString('base64'), chunkNumber, function (err, bodyObj, resp) {
          self._isUploading = false;
          if (err) {
            cb(err);
          } else {
            if (self._isUploadComplete()) {
              // We've hit the end of our stream; send FINALIZE command.
              self._finalizeMedia(mediaTmpId, cb);
            } else {
              // Tell our file stream to start emitting 'data' events again.
              chunkNumber++;
              mediaFile.resume();
            }
          }
        });
      });

      mediaFile.on('end', function () {
        // Mark our file streaming complete, and if done, send FINALIZE command.
        self._isFileStreamEnded = true;
        if (self._isUploadComplete()) {
          self._finalizeMedia(mediaTmpId, cb);
        }
      });
    }
  })
}
```
- example usage
```shell
...
var MAX_FILE_SIZE_BYTES = 15 * 1024 * 1024;
var MAX_FILE_CHUNK_BYTES = 5 * 1024 * 1024;

/**
 * FileUploader class used to upload a file to twitter via the /media/upload (chunked) API.
 * Usage:
 *   var fu = new FileUploader({ file_path: '/foo/bar/baz.mp4' }, twit);
 *   fu.upload(function (err, bodyObj, resp) {
 *     console.log(err, bodyObj);
 *   })
 *
 * @param  {Object}         params  Object of the form { file_path: String }.
 * @param  {Twit(object)}   twit    Twit instance.
 */
var FileUploader = function (params, twit) {
...
```



# <a name="apidoc.module.twit.helpers"></a>[module twit.helpers](#apidoc.module.twit.helpers)

#### <a name="apidoc.element.twit.helpers.attachBodyInfoToError"></a>[function <span class="apidocSignatureSpan">twit.helpers.</span>attachBodyInfoToError (err, body)](#apidoc.element.twit.helpers.attachBodyInfoToError)
- description and source-code
```javascript
attachBodyInfoToError = function (err, body) {
  err.twitterReply = body;
  if (!body) {
    return
  }
  if (body.error) {
    // the body itself is an error object
    err.message = body.error
    err.allErrors = err.allErrors.concat([body])
  } else if (body.errors && body.errors.length) {
    // body contains multiple error objects
    err.message = body.errors[0].message;
    err.code = body.errors[0].code;
    err.allErrors = err.allErrors.concat(body.errors)
  }
}
```
- example usage
```shell
...
    'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8'
  },
  body: 'grant_type=client_credentials',
  json: true,
}, function (err, res, body) {
  if (err) {
    var error = exports.makeTwitError(err.toString());
    exports.attachBodyInfoToError(error, body);
    return cb(error, body, res);
  }

  if ( !body ) {
    var error = exports.makeTwitError('Not valid reply from Twitter upon obtaining bearer token');
    exports.attachBodyInfoToError(error, body);
    return cb(error, body, res);
...
```

#### <a name="apidoc.element.twit.helpers.getBearerToken"></a>[function <span class="apidocSignatureSpan">twit.helpers.</span>getBearerToken (consumer_key, consumer_secret, cb)](#apidoc.element.twit.helpers.getBearerToken)
- description and source-code
```javascript
getBearerToken = function (consumer_key, consumer_secret, cb) {
  // use OAuth 2 for app-only auth (Twitter requires this)
  // get a bearer token using our app's credentials
  var b64Credentials = new Buffer(consumer_key + ':' + consumer_secret).toString('base64');
  request.post({
    url: endpoints.API_HOST + '/oauth2/token',
    headers: {
      'Authorization': 'Basic ' + b64Credentials,
      'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8'
    },
    body: 'grant_type=client_credentials',
    json: true,
  }, function (err, res, body) {
    if (err) {
      var error = exports.makeTwitError(err.toString());
      exports.attachBodyInfoToError(error, body);
      return cb(error, body, res);
    }

    if ( !body ) {
      var error = exports.makeTwitError('Not valid reply from Twitter upon obtaining bearer token');
      exports.attachBodyInfoToError(error, body);
      return cb(error, body, res);
    }

    if (body.token_type !== 'bearer') {
      var error = exports.makeTwitError('Unexpected reply from Twitter upon obtaining bearer token');
      exports.attachBodyInfoToError(error, body);
      return cb(error, body, res);
    }

    return cb(err, body.access_token);
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.helpers.makeQueryString"></a>[function <span class="apidocSignatureSpan">twit.helpers.</span>makeQueryString (obj)](#apidoc.element.twit.helpers.makeQueryString)
- description and source-code
```javascript
makeQueryString = function (obj) {
  var qs = querystring.stringify(obj)
  qs = qs.replace(/\!/g, "%21")
         .replace(/\'/g, "%27")
         .replace(/\(/g, "%28")
         .replace(/\)/g, "%29")
         .replace(/\*/g, "%2A");
  return qs
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.helpers.makeTwitError"></a>[function <span class="apidocSignatureSpan">twit.helpers.</span>makeTwitError (message)](#apidoc.element.twit.helpers.makeTwitError)
- description and source-code
```javascript
makeTwitError = function (message) {
  var err = new Error()
  if (message) {
    err.message = message
  }
  err.code = null
  err.allErrors = []
  err.twitterReply = null
  return err
}
```
- example usage
```shell
...
    'Authorization': 'Basic ' + b64Credentials,
    'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8'
  },
  body: 'grant_type=client_credentials',
  json: true,
}, function (err, res, body) {
  if (err) {
    var error = exports.makeTwitError(err.toString());
    exports.attachBodyInfoToError(error, body);
    return cb(error, body, res);
  }

  if ( !body ) {
    var error = exports.makeTwitError('Not valid reply from Twitter upon obtaining bearer token');
    exports.attachBodyInfoToError(error, body);
...
```

#### <a name="apidoc.element.twit.helpers.moveParamsIntoPath"></a>[function <span class="apidocSignatureSpan">twit.helpers.</span>moveParamsIntoPath (params, path)](#apidoc.element.twit.helpers.moveParamsIntoPath)
- description and source-code
```javascript
moveParamsIntoPath = function (params, path) {
  var rgxParam = /\/:(\w+)/g
  var missingParamErr = null

  path = path.replace(rgxParam, function (hit) {
    var paramName = hit.slice(2)
    var suppliedVal = params[paramName]
    if (!suppliedVal) {
      throw new Error('Twit: Params object is missing a required parameter for this request: ''+paramName+''')
    }
    var retVal = '/' + suppliedVal
    delete params[paramName]
    return retVal
  })
  return path
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.twit.parser"></a>[module twit.parser](#apidoc.module.twit.parser)

#### <a name="apidoc.element.twit.parser.parser"></a>[function <span class="apidocSignatureSpan">twit.</span>parser ()](#apidoc.element.twit.parser.parser)
- description and source-code
```javascript
parser = function ()  {
  this.message = ''

  EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.parser.super_"></a>[function <span class="apidocSignatureSpan">twit.parser.</span>super_ ()](#apidoc.element.twit.parser.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.twit.parser.prototype"></a>[module twit.parser.prototype](#apidoc.module.twit.parser.prototype)

#### <a name="apidoc.element.twit.parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">twit.parser.prototype.</span>parse (chunk)](#apidoc.element.twit.parser.prototype.parse)
- description and source-code
```javascript
parse = function (chunk) {
  this.message += chunk;
  chunk = this.message;

  var size = chunk.length
    , start = 0
    , offset = 0
    , curr
    , next;

  while (offset < size) {
    curr = chunk[offset];
    next = chunk[offset + 1];

    if (curr === '\r' && next === '\n') {
      var piece = chunk.slice(start, offset);
      start = offset += 2;

      if (!piece.length) { continue; } //empty object

      if (piece === 'Exceeded connection limit for user') {
        this.emit('connection-limit-exceeded',
                  new Error('Twitter says: ' + piece + '. Only instantiate one stream per set of credentials.'));
        continue;
      }

      try {
        var msg = JSON.parse(piece)
      } catch (err) {
        this.emit('error', new Error('Error parsing twitter reply: ''+piece+'', error message ''+err+'''));
      } finally {
        if (msg)
          this.emit('element', msg)

        continue
      }
    }
    offset++;
  }

  this.message = chunk.slice(start, size);
}
```
- example usage
```shell
...
      if (piece === 'Exceeded connection limit for user') {
this.emit('connection-limit-exceeded',
          new Error('Twitter says: ' + piece + '. Only instantiate one stream per set of credentials.'));
continue;
      }

      try {
var msg = JSON.parse(piece)
      } catch (err) {
this.emit('error', new Error('Error parsing twitter reply: ''+piece+'', error message ''+err+'''));
      } finally {
if (msg)
  this.emit('element', msg)

continue
...
```



# <a name="apidoc.module.twit.streaming_api_connection"></a>[module twit.streaming_api_connection](#apidoc.module.twit.streaming_api_connection)

#### <a name="apidoc.element.twit.streaming_api_connection.streaming_api_connection"></a>[function <span class="apidocSignatureSpan">twit.</span>streaming_api_connection (reqOpts, twitOptions)](#apidoc.element.twit.streaming_api_connection.streaming_api_connection)
- description and source-code
```javascript
streaming_api_connection = function (reqOpts, twitOptions) {
  this.reqOpts = reqOpts
  this.twitOptions = twitOptions
  this._twitter_time_minus_local_time_ms = 0
  EventEmitter.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.streaming_api_connection.super_"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.</span>super_ ()](#apidoc.element.twit.streaming_api_connection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.twit.streaming_api_connection.prototype"></a>[module twit.streaming_api_connection.prototype](#apidoc.module.twit.streaming_api_connection.prototype)

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._handleDisconnect"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_handleDisconnect (twitterMsg)](#apidoc.element.twit.streaming_api_connection.prototype._handleDisconnect)
- description and source-code
```javascript
_handleDisconnect = function (twitterMsg) {
  this.emit('disconnect', twitterMsg);
  this.stop();
}
```
- example usage
```shell
...

  // handle twitter objects as they come in - emit the generic 'message' event
  // along with the specific event corresponding to the message
  self.parser.on('element', function (msg) {
self.emit('message', msg)

if      (msg.delete)          { self.emit('delete', msg) }
else if (msg.disconnect)      { self._handleDisconnect(msg) }
else if (msg.limit)           { self.emit('limit', msg) }
else if (msg.scrub_geo)       { self.emit('scrub_geo', msg) }
else if (msg.warning)         { self.emit('warning', msg) }
else if (msg.status_withheld) { self.emit('status_withheld', msg) }
else if (msg.user_withheld)   { self.emit('user_withheld', msg) }
else if (msg.friends || msg.friends_str) { self.emit('friends', msg) }
else if (msg.direct_message)  { self.emit('direct_message', msg) }
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._onClose"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_onClose ()](#apidoc.element.twit.streaming_api_connection.prototype._onClose)
- description and source-code
```javascript
_onClose = function () {
  var self = this;
  self._stopStallAbortTimeout();
  if (self._scheduledReconnect) {
    // if we already have a reconnect scheduled, don't schedule another one.
    // this race condition can happen if the http.ClientRequest and http.IncomingMessage both emit 'close'
    return
  }

  self._scheduleReconnect();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._resetConnection"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_resetConnection ()](#apidoc.element.twit.streaming_api_connection.prototype._resetConnection)
- description and source-code
```javascript
_resetConnection = function () {
  if (this.request) {
    // clear our reference to the 'request' instance
    this.request.removeAllListeners();
    this.request.destroy();
  }

  if (this.response) {
    // clear our reference to the http.IncomingMessage instance
    this.response.removeAllListeners();
    this.response.destroy();
  }

  if (this.parser) {
    this.parser.removeAllListeners()
  }

  // ensure a scheduled reconnect does not occur (if one was scheduled)
  // this can happen if we get a close event before .stop() is called
  clearTimeout(this._scheduledReconnect)
  delete this._scheduledReconnect

  // clear our stall abort timeout
  this._stopStallAbortTimeout()
}
```
- example usage
```shell
...
this._connectInterval = 0
// flag indicating whether we used a 0-delay reconnect
this._usedFirstReconnect = false
}

StreamingAPIConnection.prototype._startPersistentConnection = function () {
var self = this;
self._resetConnection();
self._setupParser();
self._resetStallAbortTimeout();
self._setOauthTimestamp();
self.request = request.post(this.reqOpts);
self.emit('connect', self.request);
self.request.on('response', function (response) {
  self._updateOauthTimestampOffsetFromResponse(response)
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._resetRetryParams"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_resetRetryParams ()](#apidoc.element.twit.streaming_api_connection.prototype._resetRetryParams)
- description and source-code
```javascript
_resetRetryParams = function () {
  // delay for next reconnection attempt
  this._connectInterval = 0
  // flag indicating whether we used a 0-delay reconnect
  this._usedFirstReconnect = false
}
```
- example usage
```shell
...
}

/**
* Kick off the http request, and persist the connection
*
*/
StreamingAPIConnection.prototype.start = function () {
 this._resetRetryParams();
 this._startPersistentConnection();
 return this;
}

/**
* Abort the http request, stop scheduled reconnect (if one was scheduled) and clear state
*
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._resetStallAbortTimeout"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_resetStallAbortTimeout ()](#apidoc.element.twit.streaming_api_connection.prototype._resetStallAbortTimeout)
- description and source-code
```javascript
_resetStallAbortTimeout = function () {
  var self = this;
  // stop the previous stall abort timer
  self._stopStallAbortTimeout();
  //start a new 90s timeout to trigger a close & reconnect if no data received
  self._stallAbortTimeout = setTimeout(function () {
    self._scheduleReconnect()
  }, 90000);
  return this;
}
```
- example usage
```shell
...
this._usedFirstReconnect = false
}

StreamingAPIConnection.prototype._startPersistentConnection = function () {
var self = this;
self._resetConnection();
self._setupParser();
self._resetStallAbortTimeout();
self._setOauthTimestamp();
self.request = request.post(this.reqOpts);
self.emit('connect', self.request);
self.request.on('response', function (response) {
  self._updateOauthTimestampOffsetFromResponse(response)
  // reset our reconnection attempt flag so next attempt goes through with 0 delay
  // if we get a transport-level error
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._scheduleReconnect"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_scheduleReconnect ()](#apidoc.element.twit.streaming_api_connection.prototype._scheduleReconnect)
- description and source-code
```javascript
_scheduleReconnect = function () {
  var self = this;
  if (self.response && self.response.statusCode === 420) {
    // we are being rate limited
    // start with a 1 minute wait and double each attempt
    if (!self._connectInterval) {
      self._connectInterval = 60000;
    } else {
      self._connectInterval *= 2;
    }
  } else if (self.response && String(self.response.statusCode).charAt(0) === '5') {
    // twitter 5xx errors
    // start with a 5s wait, double each attempt up to 320s
    if (!self._connectInterval) {
      self._connectInterval = 5000;
    } else if (self._connectInterval < 320000) {
      self._connectInterval *= 2;
    } else {
      self._connectInterval = 320000;
    }
  } else {
    // we did not get an HTTP response from our last connection attempt.
    // DNS/TCP error, or a stall in the stream (and stall timer closed the connection)
    if (!self._usedFirstReconnect) {
      // first reconnection attempt on a valid connection should occur immediately
      self._connectInterval = 0;
      self._usedFirstReconnect = true;
    } else if (self._connectInterval < 16000) {
      // linearly increase delay by 250ms up to 16s
      self._connectInterval += 250;
    } else {
      // cap out reconnect interval at 16s
      self._connectInterval = 16000;
    }
  }

  // schedule the reconnect
  self._scheduledReconnect = setTimeout(function () {
    self._startPersistentConnection();
  }, self._connectInterval);
  self.emit('reconnect', self.request, self.response, self._connectInterval);
}
```
- example usage
```shell
...
  var twitErr = helpers.makeTwitError(errMsg);
  twitErr.statusCode = self.response.statusCode;
  helpers.attachBodyInfoToError(twitErr, compressedBody);
  self.emit('parser-error', twitErr);
});
    } else if (self.response.statusCode === 420) {
// close the connection forcibly so a reconnect is scheduled by 'self.onClose()'
self._scheduleReconnect();
    } else {
// We got an OK status code - the response should be valid.
// Read the body from the response and return to the user.
var gunzip = zlib.createGunzip();
self.response.pipe(gunzip);

//pass all response data to parser
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._setOauthTimestamp"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_setOauthTimestamp ()](#apidoc.element.twit.streaming_api_connection.prototype._setOauthTimestamp)
- description and source-code
```javascript
_setOauthTimestamp = function () {
  var self = this;
  if (self.reqOpts.oauth) {
    var oauth_ts = Date.now() + self._twitter_time_minus_local_time_ms;
    self.reqOpts.oauth.timestamp = Math.floor(oauth_ts/1000).toString();
  }
}
```
- example usage
```shell
...
}

StreamingAPIConnection.prototype._startPersistentConnection = function () {
var self = this;
self._resetConnection();
self._setupParser();
self._resetStallAbortTimeout();
self._setOauthTimestamp();
self.request = request.post(this.reqOpts);
self.emit('connect', self.request);
self.request.on('response', function (response) {
  self._updateOauthTimestampOffsetFromResponse(response)
  // reset our reconnection attempt flag so next attempt goes through with 0 delay
  // if we get a transport-level error
  self._usedFirstReconnect = false;
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._setupParser"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_setupParser ()](#apidoc.element.twit.streaming_api_connection.prototype._setupParser)
- description and source-code
```javascript
_setupParser = function () {
  var self = this
  self.parser = new Parser()

  // handle twitter objects as they come in - emit the generic 'message' event
  // along with the specific event corresponding to the message
  self.parser.on('element', function (msg) {
    self.emit('message', msg)

    if      (msg.delete)          { self.emit('delete', msg) }
    else if (msg.disconnect)      { self._handleDisconnect(msg) }
    else if (msg.limit)           { self.emit('limit', msg) }
    else if (msg.scrub_geo)       { self.emit('scrub_geo', msg) }
    else if (msg.warning)         { self.emit('warning', msg) }
    else if (msg.status_withheld) { self.emit('status_withheld', msg) }
    else if (msg.user_withheld)   { self.emit('user_withheld', msg) }
    else if (msg.friends || msg.friends_str) { self.emit('friends', msg) }
    else if (msg.direct_message)  { self.emit('direct_message', msg) }
    else if (msg.event)           {
      self.emit('user_event', msg)
      // reference: https://dev.twitter.com/docs/streaming-apis/messages#User_stream_messages
      var ev = msg.event

      if      (ev === 'blocked')                { self.emit('blocked', msg) }
      else if (ev === 'unblocked')              { self.emit('unblocked', msg) }
      else if (ev === 'favorite')               { self.emit('favorite', msg) }
      else if (ev === 'unfavorite')             { self.emit('unfavorite', msg) }
      else if (ev === 'follow')                 { self.emit('follow', msg) }
      else if (ev === 'unfollow')               { self.emit('unfollow', msg) }
      else if (ev === 'mute')                   { self.emit('mute', msg) }
      else if (ev === 'unmute')                 { self.emit('unmute', msg) }
      else if (ev === 'user_update')            { self.emit('user_update', msg) }
      else if (ev === 'list_created')           { self.emit('list_created', msg) }
      else if (ev === 'list_destroyed')         { self.emit('list_destroyed', msg) }
      else if (ev === 'list_updated')           { self.emit('list_updated', msg) }
      else if (ev === 'list_member_added')      { self.emit('list_member_added', msg) }
      else if (ev === 'list_member_removed')    { self.emit('list_member_removed', msg) }
      else if (ev === 'list_user_subscribed')   { self.emit('list_user_subscribed', msg) }
      else if (ev === 'list_user_unsubscribed') { self.emit('list_user_unsubscribed', msg) }
      else if (ev === 'quoted_tweet')           { self.emit('quoted_tweet', msg) }
      else if (ev === 'favorited_retweet')      { self.emit('favorited_retweet', msg) }
      else if (ev === 'retweeted_retweet')      { self.emit('retweeted_retweet', msg) }
      else                                      { self.emit('unknown_user_event', msg) }
    } else                                      { self.emit('tweet', msg) }
  })

  self.parser.on('error', function (err) {
    self.emit('parser-error', err)
  });
  self.parser.on('connection-limit-exceeded', function (err) {
    self.emit('error', err);
  })
}
```
- example usage
```shell
...
// flag indicating whether we used a 0-delay reconnect
this._usedFirstReconnect = false
}

StreamingAPIConnection.prototype._startPersistentConnection = function () {
var self = this;
self._resetConnection();
self._setupParser();
self._resetStallAbortTimeout();
self._setOauthTimestamp();
self.request = request.post(this.reqOpts);
self.emit('connect', self.request);
self.request.on('response', function (response) {
  self._updateOauthTimestampOffsetFromResponse(response)
  // reset our reconnection attempt flag so next attempt goes through with 0 delay
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._startPersistentConnection"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_startPersistentConnection ()](#apidoc.element.twit.streaming_api_connection.prototype._startPersistentConnection)
- description and source-code
```javascript
_startPersistentConnection = function () {
  var self = this;
  self._resetConnection();
  self._setupParser();
  self._resetStallAbortTimeout();
  self._setOauthTimestamp();
  self.request = request.post(this.reqOpts);
  self.emit('connect', self.request);
  self.request.on('response', function (response) {
    self._updateOauthTimestampOffsetFromResponse(response)
    // reset our reconnection attempt flag so next attempt goes through with 0 delay
    // if we get a transport-level error
    self._usedFirstReconnect = false;
    // start a stall abort timeout handle
    self._resetStallAbortTimeout();
    self.response = response
    if (STATUS_CODES_TO_ABORT_ON.indexOf(self.response.statusCode) !== -1) {
      // We got a status code telling us we should abort the connection.
      // Read the body from the response and return an error to the user.
      var body = '';
      var compressedBody = '';

      self.response.on('data', function (chunk) {
        compressedBody += chunk.toString('utf8');
      })

      var gunzip = zlib.createGunzip();
      self.response.pipe(gunzip);
      gunzip.on('data', function (chunk) {
        body += chunk.toString('utf8')
      })

      gunzip.on('end', function () {
        try {
          body = JSON.parse(body)
        } catch (jsonDecodeError) {
          // Twitter may send an HTML body
          // if non-JSON text was returned, we'll just attach it to the error as-is
        }
        // surface the error to the user
        var error = helpers.makeTwitError('Bad Twitter streaming request: ' + self.response.statusCode)
        error.statusCode = response ? response.statusCode: null;
        helpers.attachBodyInfoToError(error, body)
        self.emit('error', error);
        // stop the stream explicitly so we don't reconnect
        self.stop()
        body = null;
      });
      gunzip.on('error', function (err) {
        // If Twitter sends us back an uncompressed HTTP response, gzip will error out.
        // Handle this by emitting an error with the uncompressed response body.
        var errMsg = 'Gzip error: ' + err.message;
        var twitErr = helpers.makeTwitError(errMsg);
        twitErr.statusCode = self.response.statusCode;
        helpers.attachBodyInfoToError(twitErr, compressedBody);
        self.emit('parser-error', twitErr);
      });
    } else if (self.response.statusCode === 420) {
      // close the connection forcibly so a reconnect is scheduled by 'self.onClose()'
      self._scheduleReconnect();
    } else {
      // We got an OK status code - the response should be valid.
      // Read the body from the response and return to the user.
      var gunzip = zlib.createGunzip();
      self.response.pipe(gunzip);

      //pass all response data to parser
      gunzip.on('data', function (chunk) {
        self._connectInterval = 0
        // stop stall timer, and start a new one
        self._resetStallAbortTimeout();
        self.parser.parse(chunk.toString('utf8'));
      });

      gunzip.on('close', self._onClose.bind(self))
      gunzip.on('error', function (err) {
        self.emit('error', err);
      })
      self.response.on('error', function (err) {
        // expose response errors on twit instance
        self.emit('error', err);
      })

      // connected without an error response from Twitter, emit 'connected' event
      // this must be emitted after all its event handlers are bound
      // so the reference to 'self.response' is not interfered-with by the user until it is emitted
      self.emit('connected', self.response);
    }
  });
  self.request.on('close', self._onClose.bind(self));
  self.request.on('error', function (err) { self._scheduleReconnect.bind(self) });
  return self;
}
```
- example usage
```shell
...

/**
* Kick off the http request, and persist the connection
*
*/
StreamingAPIConnection.prototype.start = function () {
 this._resetRetryParams();
 this._startPersistentConnection();
 return this;
}

/**
* Abort the http request, stop scheduled reconnect (if one was scheduled) and clear state
*
*/
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._stopStallAbortTimeout"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_stopStallAbortTimeout ()](#apidoc.element.twit.streaming_api_connection.prototype._stopStallAbortTimeout)
- description and source-code
```javascript
_stopStallAbortTimeout = function () {
  clearTimeout(this._stallAbortTimeout);
  // mark the timer as 'null' so it is clear via introspection that the timeout is not scheduled
  delete this._stallAbortTimeout;
  return this;
}
```
- example usage
```shell
...

// ensure a scheduled reconnect does not occur (if one was scheduled)
// this can happen if we get a close event before .stop() is called
clearTimeout(this._scheduledReconnect)
delete this._scheduledReconnect

// clear our stall abort timeout
this._stopStallAbortTimeout()
}

/**
 * Resets the parameters used in determining the next reconnect time
 */
StreamingAPIConnection.prototype._resetRetryParams = function () {
// delay for next reconnection attempt
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype._updateOauthTimestampOffsetFromResponse"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>_updateOauthTimestampOffsetFromResponse (resp)](#apidoc.element.twit.streaming_api_connection.prototype._updateOauthTimestampOffsetFromResponse)
- description and source-code
```javascript
_updateOauthTimestampOffsetFromResponse = function (resp) {
  if (resp && resp.headers && resp.headers.date &&
      new Date(resp.headers.date).toString() !== 'Invalid Date'
  ) {
    var twitterTimeMs = new Date(resp.headers.date).getTime()
    this._twitter_time_minus_local_time_ms = twitterTimeMs - Date.now();
  }
}
```
- example usage
```shell
...
self._resetConnection();
self._setupParser();
self._resetStallAbortTimeout();
self._setOauthTimestamp();
self.request = request.post(this.reqOpts);
self.emit('connect', self.request);
self.request.on('response', function (response) {
  self._updateOauthTimestampOffsetFromResponse(response)
  // reset our reconnection attempt flag so next attempt goes through with 0 delay
  // if we get a transport-level error
  self._usedFirstReconnect = false;
  // start a stall abort timeout handle
  self._resetStallAbortTimeout();
  self.response = response
  if (STATUS_CODES_TO_ABORT_ON.indexOf(self.response.statusCode) !== -1) {
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype.start"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>start ()](#apidoc.element.twit.streaming_api_connection.prototype.start)
- description and source-code
```javascript
start = function () {
  this._resetRetryParams();
  this._startPersistentConnection();
  return this;
}
```
- example usage
```shell
...
}
'''

##stream.stop()

Call this function on the stream to stop streaming (closes the connection with Twitter).

##stream.start()

Call this function to restart the stream after you called '.stop()' on it.
Note: there is no need to call '.start()' to begin streaming. 'Twit.stream' calls '.start()' for you.

-------

#What do I have access to?
...
```

#### <a name="apidoc.element.twit.streaming_api_connection.prototype.stop"></a>[function <span class="apidocSignatureSpan">twit.streaming_api_connection.prototype.</span>stop ()](#apidoc.element.twit.streaming_api_connection.prototype.stop)
- description and source-code
```javascript
stop = function () {
  // clear connection variables and timeout handles
  this._resetConnection();
  this._resetRetryParams();
  return this;
}
```
- example usage
```shell
...
  statusCode:   '...',  // statusCode from Twitter
  code:         '...',  // error code from Twitter
  twitterReply: '...',  // raw response data from Twitter
  allErrors:    '...'   // array of errors returned from Twitter
}
'''

##stream.stop()

Call this function on the stream to stop streaming (closes the connection with Twitter).

##stream.start()

Call this function to restart the stream after you called '.stop()' on it.
Note: there is no need to call '.start()' to begin streaming. 'Twit.stream' calls '.start()' for you.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
