# api documentation for  [nodejs-websocket (v1.7.1)](https://github.com/sitegui/nodejs-websocket#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nodejs-websocket.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nodejs-websocket) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nodejs-websocket.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nodejs-websocket)
#### Basic server&client approach to websocket (text and binary frames)

[![NPM](https://nodei.co/npm/nodejs-websocket.png?downloads=true)](https://www.npmjs.com/package/nodejs-websocket)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nodejs-websocket/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nodejs-websocket_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nodejs-websocket/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nodejs-websocket/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nodejs-websocket/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sitegui",
        "email": "sitegui@sitegui.com.br"
    },
    "bugs": {
        "url": "https://github.com/sitegui/nodejs-websocket/issues"
    },
    "dependencies": {},
    "description": "Basic server&client approach to websocket (text and binary frames)",
    "devDependencies": {
        "mocha": "^3.0.2",
        "should": "^11.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cccfbba823bf1cfa9680f168ab7ab53121e48410",
        "tarball": "https://registry.npmjs.org/nodejs-websocket/-/nodejs-websocket-1.7.1.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "gitHead": "28835a2321afa8e575a283d4d914a681fefcc031",
    "homepage": "https://github.com/sitegui/nodejs-websocket#readme",
    "keywords": [
        "websocket",
        "websocket-server",
        "websocket-client"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "sitegui",
            "email": "sitegui@sitegui.com.br"
        }
    ],
    "name": "nodejs-websocket",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sitegui/nodejs-websocket.git"
    },
    "scripts": {
        "start": "node server.js",
        "test": "mocha -R spec -b"
    },
    "version": "1.7.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nodejs-websocket](#apidoc.module.nodejs-websocket)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>Connection (socket, parentOrOptions, callback)](#apidoc.element.nodejs-websocket.Connection)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>InStream ()](#apidoc.element.nodejs-websocket.InStream)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>OutStream (connection, minSize)](#apidoc.element.nodejs-websocket.OutStream)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>Server (secure, options, callback)](#apidoc.element.nodejs-websocket.Server)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>connect (URL, options, callback)](#apidoc.element.nodejs-websocket.connect)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>createServer (options, callback)](#apidoc.element.nodejs-websocket.createServer)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>setBinaryFragmentation (bytes)](#apidoc.element.nodejs-websocket.setBinaryFragmentation)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>setMaxBufferLength (bytes)](#apidoc.element.nodejs-websocket.setMaxBufferLength)
1.  object <span class="apidocSignatureSpan">nodejs-websocket.</span>Connection.prototype
1.  object <span class="apidocSignatureSpan">nodejs-websocket.</span>InStream.prototype
1.  object <span class="apidocSignatureSpan">nodejs-websocket.</span>OutStream.prototype
1.  object <span class="apidocSignatureSpan">nodejs-websocket.</span>Server.prototype
1.  object <span class="apidocSignatureSpan">nodejs-websocket.</span>frame

#### [module nodejs-websocket.Connection](#apidoc.module.nodejs-websocket.Connection)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>Connection (socket, parentOrOptions, callback)](#apidoc.element.nodejs-websocket.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.</span>super_ ()](#apidoc.element.nodejs-websocket.Connection.super_)
1.  number <span class="apidocSignatureSpan">nodejs-websocket.Connection.</span>binaryFragmentation
1.  number <span class="apidocSignatureSpan">nodejs-websocket.Connection.</span>maxBufferLength

#### [module nodejs-websocket.Connection.prototype](#apidoc.module.nodejs-websocket.Connection.prototype)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>answerHandshake (lines)](#apidoc.element.nodejs-websocket.Connection.prototype.answerHandshake)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>beginBinary ()](#apidoc.element.nodejs-websocket.Connection.prototype.beginBinary)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>buildRequest (requestLine, headers)](#apidoc.element.nodejs-websocket.Connection.prototype.buildRequest)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>checkHandshake (lines)](#apidoc.element.nodejs-websocket.Connection.prototype.checkHandshake)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>close (code, reason)](#apidoc.element.nodejs-websocket.Connection.prototype.close)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>doRead ()](#apidoc.element.nodejs-websocket.Connection.prototype.doRead)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>extractFrame ()](#apidoc.element.nodejs-websocket.Connection.prototype.extractFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>processCloseFrame (payload)](#apidoc.element.nodejs-websocket.Connection.prototype.processCloseFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>processFrame (fin, opcode, payload)](#apidoc.element.nodejs-websocket.Connection.prototype.processFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>readHandshake ()](#apidoc.element.nodejs-websocket.Connection.prototype.readHandshake)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>readHeaders (lines)](#apidoc.element.nodejs-websocket.Connection.prototype.readHeaders)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>send (data, callback)](#apidoc.element.nodejs-websocket.Connection.prototype.send)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>sendBinary (data, callback)](#apidoc.element.nodejs-websocket.Connection.prototype.sendBinary)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>sendPing (data)](#apidoc.element.nodejs-websocket.Connection.prototype.sendPing)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>sendText (str, callback)](#apidoc.element.nodejs-websocket.Connection.prototype.sendText)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>startHandshake ()](#apidoc.element.nodejs-websocket.Connection.prototype.startHandshake)
1.  number <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>CLOSED
1.  number <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>CLOSING
1.  number <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>CONNECTING
1.  number <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>OPEN

#### [module nodejs-websocket.InStream](#apidoc.module.nodejs-websocket.InStream)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>InStream ()](#apidoc.element.nodejs-websocket.InStream.InStream)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.InStream.</span>super_ (options)](#apidoc.element.nodejs-websocket.InStream.super_)

#### [module nodejs-websocket.InStream.prototype](#apidoc.module.nodejs-websocket.InStream.prototype)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.InStream.prototype.</span>_read ()](#apidoc.element.nodejs-websocket.InStream.prototype._read)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.InStream.prototype.</span>addData (data)](#apidoc.element.nodejs-websocket.InStream.prototype.addData)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.InStream.prototype.</span>end ()](#apidoc.element.nodejs-websocket.InStream.prototype.end)

#### [module nodejs-websocket.OutStream](#apidoc.module.nodejs-websocket.OutStream)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>OutStream (connection, minSize)](#apidoc.element.nodejs-websocket.OutStream.OutStream)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.OutStream.</span>super_ (options)](#apidoc.element.nodejs-websocket.OutStream.super_)

#### [module nodejs-websocket.OutStream.prototype](#apidoc.module.nodejs-websocket.OutStream.prototype)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.OutStream.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.nodejs-websocket.OutStream.prototype._write)

#### [module nodejs-websocket.Server](#apidoc.module.nodejs-websocket.Server)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.</span>Server (secure, options, callback)](#apidoc.element.nodejs-websocket.Server.Server)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Server.</span>super_ ()](#apidoc.element.nodejs-websocket.Server.super_)

#### [module nodejs-websocket.Server.prototype](#apidoc.module.nodejs-websocket.Server.prototype)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Server.prototype.</span>_buildSelectProtocol (validProtocols)](#apidoc.element.nodejs-websocket.Server.prototype._buildSelectProtocol)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Server.prototype.</span>close (callback)](#apidoc.element.nodejs-websocket.Server.prototype.close)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.Server.prototype.</span>listen (port, host, callback)](#apidoc.element.nodejs-websocket.Server.prototype.listen)

#### [module nodejs-websocket.frame](#apidoc.module.nodejs-websocket.frame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createBinaryFrame (data, masked, first, fin)](#apidoc.element.nodejs-websocket.frame.createBinaryFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createCloseFrame (code, reason, masked)](#apidoc.element.nodejs-websocket.frame.createCloseFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createPingFrame (data, masked)](#apidoc.element.nodejs-websocket.frame.createPingFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createPongFrame (data, masked)](#apidoc.element.nodejs-websocket.frame.createPongFrame)
1.  [function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createTextFrame (data, masked)](#apidoc.element.nodejs-websocket.frame.createTextFrame)



# <a name="apidoc.module.nodejs-websocket"></a>[module nodejs-websocket](#apidoc.module.nodejs-websocket)

#### <a name="apidoc.element.nodejs-websocket.Connection"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>Connection (socket, parentOrOptions, callback)](#apidoc.element.nodejs-websocket.Connection)
- description and source-code
```javascript
function Connection(socket, parentOrOptions, callback) {
	var that = this,
		connectEvent

	if (parentOrOptions instanceof Server) {
		// Server-side connection
		this.server = parentOrOptions
		this.path = null
		this.host = null
		this.extraHeaders = null
		this.protocols = []
	} else {
		// Client-side
		this.server = null
		this.path = parentOrOptions.path
		this.host = parentOrOptions.host
		this.extraHeaders = parentOrOptions.extraHeaders
		this.protocols = parentOrOptions.protocols || []
	}

	this.protocol = undefined
	this.socket = socket
	this.readyState = this.CONNECTING
	this.buffer = new Buffer(0)
	this.frameBuffer = null // string for text frames and InStream for binary frames
	this.outStream = null // current allocated OutStream object for sending binary frames
	this.key = null // the Sec-WebSocket-Key header
	this.headers = {} // read only map of header names and values. Header names are lower-cased

	// Set listeners
	socket.on('readable', function () {
		that.doRead()
	})

	socket.on('error', function (err) {
		that.emit('error', err)
	})

	if (!this.server) {
		connectEvent = socket.constructor.name === 'CleartextStream' ? 'secureConnect' : 'connect'
		socket.on(connectEvent, function () {
			that.startHandshake()
		})
	}

	// Close listeners
	var onclose = function () {
		if (that.readyState === that.CONNECTING || that.readyState === that.OPEN) {
			that.emit('close', 1006, '')
		}
		that.readyState = this.CLOSED
		if (that.frameBuffer instanceof InStream) {
			that.frameBuffer.end()
			that.frameBuffer = null
		}
		if (that.outStream instanceof OutStream) {
			that.outStream.end()
			that.outStream = null
		}
	}
	socket.once('close', onclose)
	socket.once('finish', onclose)

	// super constructor
	events.EventEmitter.call(this)
	if (callback) {
		this.once('connect', callback)
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.InStream"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>InStream ()](#apidoc.element.nodejs-websocket.InStream)
- description and source-code
```javascript
function InStream() {
	stream.Readable.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.OutStream"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>OutStream (connection, minSize)](#apidoc.element.nodejs-websocket.OutStream)
- description and source-code
```javascript
function OutStream(connection, minSize) {
	var that = this
	this.connection = connection
	this.minSize = minSize
	this.buffer = new Buffer(0)
	this.hasSent = false // Indicates if any frame has been sent yet
	stream.Writable.call(this)
	this.on('finish', function () {
		if (that.connection.readyState === that.connection.OPEN) {
			// Ignore if not connected anymore
			that.connection.socket.write(frame.createBinaryFrame(that.buffer, !that.connection.server, !that.hasSent, true))
		}
		that.connection.outStream = null
	})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.Server"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>Server (secure, options, callback)](#apidoc.element.nodejs-websocket.Server)
- description and source-code
```javascript
function Server(secure, options, callback) {
	var that = this

	if (typeof options === 'function') {
		callback = options
		options = undefined
	}

	var onConnection = function (socket) {
		var conn = new Connection(socket, that, function () {
			that.connections.push(conn)
			conn.removeListener('error', nop)
			that.emit('connection', conn)
		})
		conn.on('close', function () {
			var pos = that.connections.indexOf(conn)
			if (pos !== -1) {
				that.connections.splice(pos, 1)
			}
		})

		// Ignore errors before the connection is established
		conn.on('error', nop)
	}

	if (secure) {
		this.socket = tls.createServer(options, onConnection)
	} else {
		this.socket = net.createServer(options, onConnection)
	}

	this.socket.on('close', function () {
		that.emit('close')
	})
	this.socket.on('error', function (err) {
		that.emit('error', err)
	})
	this.connections = []

	// super constructor
	events.EventEmitter.call(this)
	if (callback) {
		this.on('connection', callback)
	}

	// Add protocol agreement handling
	/**
	 * @member {?SelectProtocolCallback}
	 * @private
	 */
	this._selectProtocol = null

	if (options && options.selectProtocol) {
		// User-provided logic
		this._selectProtocol = options.selectProtocol
	} else if (options && options.validProtocols) {
		// Default logic
		this._selectProtocol = this._buildSelectProtocol(options.validProtocols)
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.connect"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>connect (URL, options, callback)](#apidoc.element.nodejs-websocket.connect)
- description and source-code
```javascript
connect = function (URL, options, callback) {
	var socket

	if (typeof options === 'function') {
		callback = options
		options = undefined
	}
	options = options || {}

	var connectionOptions = parseWSURL(URL)
	options.port = connectionOptions.port
	options.host = connectionOptions.host

	connectionOptions.extraHeaders = options.extraHeaders
	connectionOptions.protocols = options.protocols

	if (connectionOptions.secure) {
		socket = tls.connect(options)
	} else {
		socket = net.connect(options)
	}

	return new Connection(socket, connectionOptions, callback)
}
```
- example usage
```shell
...

To support protocols, the 'options' object may have either of these properties:
* 'validProtocols': an array of protocol names the server accepts. The server will pick the most preferred protocol in the client
's list.
* 'selectProtocol': a callback to resolve the protocol negotiation. This callback will be passed two parameters: the connection
handling the handshake and the array of protocol names informed by the client, ordered by preference. It should return the resolved
 protocol, or empty if there is no agreement.

The 'callback' is a function which is automatically added to the '"connection"' event.

## ws.connect(URL, [options], [callback])
Returns a new 'Connection' object, representing a websocket client connection

'URL' is a string with the format "ws://localhost:8000/chat" (the port can be omitted)

'options' is an object that will be passed to net.connect() (or tls.connect() if the protocol is "wss:").
The properties "host" and "port" will be read from the 'URL'.
The optional property 'extraHeaders' will be used to add more headers to the HTTP handshake request. If present, it must be an object
, like '{'X-My-Header': 'value'}'.
...
```

#### <a name="apidoc.element.nodejs-websocket.createServer"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>createServer (options, callback)](#apidoc.element.nodejs-websocket.createServer)
- description and source-code
```javascript
createServer = function (options, callback) {
	if (typeof options === 'function' || !arguments.length) {
		return new Server(false, options)
	}
	return new Server(Boolean(options.secure), options, callback)
}
```
- example usage
```shell
...

# How to use it
Install with 'npm install nodejs-websocket' or put all files in a folder called "nodejs-websocket", and:
'''javascript
var ws = require("nodejs-websocket")

// Scream server example: "hi" -> "HI!!!"
var server = ws.createServer(function (conn) {
	console.log("New connection")
	conn.on("text", function (str) {
		console.log("Received "+str)
		conn.sendText(str.toUpperCase()+"!!!")
	})
	conn.on("close", function (code, reason) {
		console.log("Connection closed")
...
```

#### <a name="apidoc.element.nodejs-websocket.setBinaryFragmentation"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>setBinaryFragmentation (bytes)](#apidoc.element.nodejs-websocket.setBinaryFragmentation)
- description and source-code
```javascript
setBinaryFragmentation = function (bytes) {
	Connection.binaryFragmentation = bytes
}
```
- example usage
```shell
...
'options' is an object that will be passed to net.connect() (or tls.connect() if the protocol is "wss:").
The properties "host" and "port" will be read from the 'URL'.
The optional property 'extraHeaders' will be used to add more headers to the HTTP handshake request. If present, it must be an object
, like '{'X-My-Header': 'value'}'.
The optional property 'protocols' will be used in the handshake (as "Sec-WebSocket-Protocol" header) to allow the server to choose
 one of those values. If present, it must be an array of strings.

'callback' will be added as "connect" listener

## ws.setBinaryFragmentation(bytes)
Sets the minimum size of a pack of binary data to send in a single frame (default: 512kiB)

## ws.setMaxBufferLength(bytes)
Set the maximum size the internal Buffer can grow (default: 2MiB)
If at any time it stays bigger than this, the connection will be closed with code 1009
This is a security measure, to avoid memory attacks
...
```

#### <a name="apidoc.element.nodejs-websocket.setMaxBufferLength"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>setMaxBufferLength (bytes)](#apidoc.element.nodejs-websocket.setMaxBufferLength)
- description and source-code
```javascript
setMaxBufferLength = function (bytes) {
	Connection.maxBufferLength = bytes
}
```
- example usage
```shell
...
The optional property 'protocols' will be used in the handshake (as "Sec-WebSocket-Protocol" header) to allow the server to choose
 one of those values. If present, it must be an array of strings.

'callback' will be added as "connect" listener

## ws.setBinaryFragmentation(bytes)
Sets the minimum size of a pack of binary data to send in a single frame (default: 512kiB)

## ws.setMaxBufferLength(bytes)
Set the maximum size the internal Buffer can grow (default: 2MiB)
If at any time it stays bigger than this, the connection will be closed with code 1009
This is a security measure, to avoid memory attacks

# Server
The class that represents a websocket server, much like a HTTP server
...
```



# <a name="apidoc.module.nodejs-websocket.Connection"></a>[module nodejs-websocket.Connection](#apidoc.module.nodejs-websocket.Connection)

#### <a name="apidoc.element.nodejs-websocket.Connection.Connection"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>Connection (socket, parentOrOptions, callback)](#apidoc.element.nodejs-websocket.Connection.Connection)
- description and source-code
```javascript
function Connection(socket, parentOrOptions, callback) {
	var that = this,
		connectEvent

	if (parentOrOptions instanceof Server) {
		// Server-side connection
		this.server = parentOrOptions
		this.path = null
		this.host = null
		this.extraHeaders = null
		this.protocols = []
	} else {
		// Client-side
		this.server = null
		this.path = parentOrOptions.path
		this.host = parentOrOptions.host
		this.extraHeaders = parentOrOptions.extraHeaders
		this.protocols = parentOrOptions.protocols || []
	}

	this.protocol = undefined
	this.socket = socket
	this.readyState = this.CONNECTING
	this.buffer = new Buffer(0)
	this.frameBuffer = null // string for text frames and InStream for binary frames
	this.outStream = null // current allocated OutStream object for sending binary frames
	this.key = null // the Sec-WebSocket-Key header
	this.headers = {} // read only map of header names and values. Header names are lower-cased

	// Set listeners
	socket.on('readable', function () {
		that.doRead()
	})

	socket.on('error', function (err) {
		that.emit('error', err)
	})

	if (!this.server) {
		connectEvent = socket.constructor.name === 'CleartextStream' ? 'secureConnect' : 'connect'
		socket.on(connectEvent, function () {
			that.startHandshake()
		})
	}

	// Close listeners
	var onclose = function () {
		if (that.readyState === that.CONNECTING || that.readyState === that.OPEN) {
			that.emit('close', 1006, '')
		}
		that.readyState = this.CLOSED
		if (that.frameBuffer instanceof InStream) {
			that.frameBuffer.end()
			that.frameBuffer = null
		}
		if (that.outStream instanceof OutStream) {
			that.outStream.end()
			that.outStream = null
		}
	}
	socket.once('close', onclose)
	socket.once('finish', onclose)

	// super constructor
	events.EventEmitter.call(this)
	if (callback) {
		this.once('connect', callback)
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.Connection.super_"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.</span>super_ ()](#apidoc.element.nodejs-websocket.Connection.super_)
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



# <a name="apidoc.module.nodejs-websocket.Connection.prototype"></a>[module nodejs-websocket.Connection.prototype](#apidoc.module.nodejs-websocket.Connection.prototype)

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.answerHandshake"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>answerHandshake (lines)](#apidoc.element.nodejs-websocket.Connection.prototype.answerHandshake)
- description and source-code
```javascript
answerHandshake = function (lines) {
	var path, key, sha1, headers

	// First line
	if (lines.length < 6) {
		return false
	}
	path = lines[0].match(/^GET (.+) HTTP\/\d\.\d$/i)
	if (!path) {
		return false
	}
	this.path = path[1]

	// Extract all headers
	this.readHeaders(lines)

	// Validate necessary headers
	if (!('host' in this.headers) ||
		!('sec-websocket-key' in this.headers) ||
		!('upgrade' in this.headers) ||
		!('connection' in this.headers)) {
		return false
	}
	if (this.headers.upgrade.toLowerCase() !== 'websocket' ||
		this.headers.connection.toLowerCase().split(', ').indexOf('upgrade') === -1) {
		return false
	}
	if (this.headers['sec-websocket-version'] !== '13') {
		return false
	}

	this.key = this.headers['sec-websocket-key']

	// Agree on a protocol
	if ('sec-websocket-protocol' in this.headers) {
		// Parse
		this.protocols = this.headers['sec-websocket-protocol'].split(',').map(function (each) {
			return each.trim()
		})

		// Select protocol
		if (this.server._selectProtocol) {
			this.protocol = this.server._selectProtocol(this, this.protocols)
		}
	}

	// Build and send the response
	sha1 = crypto.createHash('sha1')
	sha1.end(this.key + '258EAFA5-E914-47DA-95CA-C5AB0DC85B11')
	key = sha1.read().toString('base64')
	headers = {
		Upgrade: 'websocket',
		Connection: 'Upgrade',
		'Sec-WebSocket-Accept': key
	}
	if (this.protocol) {
		headers['Sec-WebSocket-Protocol'] = this.protocol
	}
	this.socket.write(this.buildRequest('HTTP/1.1 101 Switching Protocols', headers))
	return true
}
```
- example usage
```shell
...
		}
	}
	if (!found) {
		// Wait for more data
		return false
	}
	data = this.buffer.slice(0, i + 4).toString().split('\r\n')
	if (this.server ? this.answerHandshake(data) : this.checkHandshake(data)) {
		this.buffer = this.buffer.slice(i + 4)
		this.readyState = this.OPEN
		this.emit('connect')
		return true
	} else {
		this.socket.end(this.server ? 'HTTP/1.1 400 Bad Request\r\n\r\n' : undefined)
		return false
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.beginBinary"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>beginBinary ()](#apidoc.element.nodejs-websocket.Connection.prototype.beginBinary)
- description and source-code
```javascript
beginBinary = function () {
	if (this.readyState === this.OPEN) {
		if (!this.outStream) {
			return (this.outStream = new OutStream(this, Connection.binaryFragmentation))
		}
		this.emit('error', new Error('You can\'t send more binary frames until you finish sending the previous binary frames'))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}
```
- example usage
```shell
...
You cannot send text data while sending binary data. If you try to do so, the connection will emit an "error" event

## connection.sendText(str, [callback])
Sends a given string to the other side. You can't send text data in the middle of a binary transmission.

'callback' will be added as a listener to write operation over the socket

## connection.beginBinary()
Asks the connection to begin transmitting binary data. Returns a WritableStream.
The binary transmission will end when the WritableStream finishes (like when you call .end on it)

## connection.sendBinary(data, [callback])
Sends a single chunk of binary data (like calling connection.beginBinary().end(data))

'callback' will be added as a listener to write operation over the socket
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.buildRequest"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>buildRequest (requestLine, headers)](#apidoc.element.nodejs-websocket.Connection.prototype.buildRequest)
- description and source-code
```javascript
buildRequest = function (requestLine, headers) {
	var headerString = requestLine + '\r\n',
		headerName

	for (headerName in headers) {
		headerString += headerName + ': ' + headers[headerName] + '\r\n'
	}

	return headerString + '\r\n'
}
```
- example usage
```shell
...
		headers['Sec-WebSocket-Protocol'] = this.protocols.join(', ')
	}

	for (header in this.extraHeaders) {
		headers[header] = this.extraHeaders[header]
	}

	str = this.buildRequest('GET ' + this.path + ' HTTP/1.1', headers)
	this.socket.write(str)
}

/**
* Try to read the handshake from the internal buffer
* If it succeeds, the handshake data is consumed from the internal buffer
* @returns {boolean} - whether the handshake was done
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.checkHandshake"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>checkHandshake (lines)](#apidoc.element.nodejs-websocket.Connection.prototype.checkHandshake)
- description and source-code
```javascript
checkHandshake = function (lines) {
	var key, sha1, protocol

	// First line
	if (lines.length < 4) {
		this.emit('error', new Error('Invalid handshake: too short'))
		return false
	}
	if (!lines[0].match(/^HTTP\/\d\.\d 101( .*)?$/i)) {
		this.emit('error', new Error('Invalid handshake: invalid first line format'))
		return false
	}

	// Extract all headers
	this.readHeaders(lines)

	// Validate necessary headers
	if (!('upgrade' in this.headers) ||
		!('sec-websocket-accept' in this.headers) ||
		!('connection' in this.headers)) {
		this.emit('error', new Error('Invalid handshake: missing required headers'))
		return false
	}
	if (this.headers.upgrade.toLowerCase() !== 'websocket' ||
		this.headers.connection.toLowerCase().split(', ').indexOf('upgrade') === -1) {
		this.emit('error', new Error('Invalid handshake: invalid Upgrade or Connection header'))
		return false
	}
	key = this.headers['sec-websocket-accept']

	// Check protocol negotiation
	protocol = this.headers['sec-websocket-protocol']
	if (this.protocols && this.protocols.length) {
		// The server must choose one from our list
		if (!protocol || this.protocols.indexOf(protocol) === -1) {
			this.emit('error', new Error('Invalid handshake: no protocol was negotiated'))
			return false
		}
	} else {
		// The server must not choose a protocol
		if (protocol) {
			this.emit('error', new Error('Invalid handshake: no protocol negotiation was expected'))
			return false
		}
	}
	this.protocol = protocol

	// Check the key
	sha1 = crypto.createHash('sha1')
	sha1.end(this.key + '258EAFA5-E914-47DA-95CA-C5AB0DC85B11')
	if (key !== sha1.read().toString('base64')) {
		this.emit('error', new Error('Invalid handshake: hash mismatch'))
		return false
	}
	return true
}
```
- example usage
```shell
...
		}
	}
	if (!found) {
		// Wait for more data
		return false
	}
	data = this.buffer.slice(0, i + 4).toString().split('\r\n')
	if (this.server ? this.answerHandshake(data) : this.checkHandshake(data)) {
		this.buffer = this.buffer.slice(i + 4)
		this.readyState = this.OPEN
		this.emit('connect')
		return true
	} else {
		this.socket.end(this.server ? 'HTTP/1.1 400 Bad Request\r\n\r\n' : undefined)
		return false
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.close"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>close (code, reason)](#apidoc.element.nodejs-websocket.Connection.prototype.close)
- description and source-code
```javascript
close = function (code, reason) {
	if (this.readyState === this.OPEN) {
		this.socket.write(frame.createCloseFrame(code, reason, !this.server))
		this.readyState = this.CLOSING
	} else if (this.readyState !== this.CLOSED) {
		this.socket.end()
		this.readyState = this.CLOSED
	}
	this.emit('close', code, reason)
}
```
- example usage
```shell
...

If the 'host' is omitted, the server will accept connections directed to any IPv4 address (INADDR_ANY).

A 'port' value of zero will assign a random port.

'callback' will be added as an listener for the ''listening'' event.

## server.close([callback])
Stops the server from accepting new connections and keeps existing connections. This function is asynchronous, the server is finally
 closed when all connections are ended and the server emits a 'close' event. The optional callback will be called once the 'close
' event occurs.

## server.socket
The underlying socket, returned by net.createServer or tls.createServer

## server.connections
An Array with all connected clients. It's useful for broadcasting a message:
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.doRead"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>doRead ()](#apidoc.element.nodejs-websocket.Connection.prototype.doRead)
- description and source-code
```javascript
doRead = function () {
	var buffer, temp

	// Fetches the data
	buffer = this.socket.read()
	if (!buffer) {
		// Waits for more data
		return
	}

	// Save to the internal buffer
	this.buffer = Buffer.concat([this.buffer, buffer], this.buffer.length + buffer.length)

	if (this.readyState === this.CONNECTING) {
		if (!this.readHandshake()) {
			// May have failed or we're waiting for more data
			return
		}
	}

	if (this.readyState !== this.CLOSED) {
		// Try to read as many frames as possible
		while ((temp = this.extractFrame()) === true) {}
		if (temp === false) {
			// Protocol error
			this.close(1002)
		} else if (this.buffer.length > Connection.maxBufferLength) {
			// Frame too big
			this.close(1009)
		}
	}
}
```
- example usage
```shell
...
	this.frameBuffer = null // string for text frames and InStream for binary frames
	this.outStream = null // current allocated OutStream object for sending binary frames
	this.key = null // the Sec-WebSocket-Key header
	this.headers = {} // read only map of header names and values. Header names are lower-cased

	// Set listeners
	socket.on('readable', function () {
		that.doRead()
	})

	socket.on('error', function (err) {
		that.emit('error', err)
	})

	if (!this.server) {
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.extractFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>extractFrame ()](#apidoc.element.nodejs-websocket.Connection.prototype.extractFrame)
- description and source-code
```javascript
extractFrame = function () {
	var fin, opcode, B, HB, mask, len, payload, start, i, hasMask

	if (this.buffer.length < 2) {
		return
	}

	// Is this the last frame in a sequence?
	B = this.buffer[0]
	HB = B >> 4
	if (HB % 8) {
		// RSV1, RSV2 and RSV3 must be clear
		return false
	}
	fin = HB === 8
	opcode = B % 16

	if (opcode !== 0 && opcode !== 1 && opcode !== 2 &&
		opcode !== 8 && opcode !== 9 && opcode !== 10) {
		// Invalid opcode
		return false
	}
	if (opcode >= 8 && !fin) {
		// Control frames must not be fragmented
		return false
	}

	B = this.buffer[1]
	hasMask = B >> 7
	if ((this.server && !hasMask) || (!this.server && hasMask)) {
		// Frames sent by clients must be masked
		return false
	}
	len = B % 128
	start = hasMask ? 6 : 2

	if (this.buffer.length < start + len) {
		// Not enough data in the buffer
		return
	}

	// Get the actual payload length
	if (len === 126) {
		len = this.buffer.readUInt16BE(2)
		start += 2
	} else if (len === 127) {
		// Warning: JS can only store up to 2^53 in its number format
		len = this.buffer.readUInt32BE(2) * Math.pow(2, 32) + this.buffer.readUInt32BE(6)
		start += 8
	}
	if (this.buffer.length < start + len) {
		return
	}

	// Extract the payload
	payload = this.buffer.slice(start, start + len)
	if (hasMask) {
		// Decode with the given mask
		mask = this.buffer.slice(start - 4, start)
		for (i = 0; i < payload.length; i++) {
			payload[i] ^= mask[i % 4]
		}
	}
	this.buffer = this.buffer.slice(start + len)

	// Proceeds to frame processing
	return this.processFrame(fin, opcode, payload)
}
```
- example usage
```shell
...
			// May have failed or we're waiting for more data
			return
		}
	}

	if (this.readyState !== this.CLOSED) {
		// Try to read as many frames as possible
		while ((temp = this.extractFrame()) === true) {}
		if (temp === false) {
			// Protocol error
			this.close(1002)
		} else if (this.buffer.length > Connection.maxBufferLength) {
			// Frame too big
			this.close(1009)
		}
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.processCloseFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>processCloseFrame (payload)](#apidoc.element.nodejs-websocket.Connection.prototype.processCloseFrame)
- description and source-code
```javascript
processCloseFrame = function (payload) {
	var code, reason
	if (payload.length >= 2) {
		code = payload.readUInt16BE(0)
		reason = payload.slice(2).toString()
	} else {
		code = 1005
		reason = ''
	}
	this.socket.write(frame.createCloseFrame(code, reason, !this.server))
	this.readyState = this.CLOSED
	this.emit('close', code, reason)
}
```
- example usage
```shell
...
 */
Connection.prototype.processFrame = function (fin, opcode, payload) {
	if (opcode === 8) {
		// Close frame
		if (this.readyState === this.CLOSING) {
			this.socket.end()
		} else if (this.readyState === this.OPEN) {
			this.processCloseFrame(payload)
		}
		return true
	} else if (opcode === 9) {
		// Ping frame
		if (this.readyState === this.OPEN) {
			this.socket.write(frame.createPongFrame(payload.toString(), !this.server))
		}
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.processFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>processFrame (fin, opcode, payload)](#apidoc.element.nodejs-websocket.Connection.prototype.processFrame)
- description and source-code
```javascript
processFrame = function (fin, opcode, payload) {
	if (opcode === 8) {
		// Close frame
		if (this.readyState === this.CLOSING) {
			this.socket.end()
		} else if (this.readyState === this.OPEN) {
			this.processCloseFrame(payload)
		}
		return true
	} else if (opcode === 9) {
		// Ping frame
		if (this.readyState === this.OPEN) {
			this.socket.write(frame.createPongFrame(payload.toString(), !this.server))
		}
		return true
	} else if (opcode === 10) {
		// Pong frame
		this.emit('pong', payload.toString())
		return true
	}

	if (this.readyState !== this.OPEN) {
		// Ignores if the connection isn't opened anymore
		return true
	}

	if (opcode === 0 && this.frameBuffer === null) {
		// Unexpected continuation frame
		return false
	} else if (opcode !== 0 && this.frameBuffer !== null) {
		// Last sequence didn't finished correctly
		return false
	}

	if (!opcode) {
		// Get the current opcode for fragmented frames
		opcode = typeof this.frameBuffer === 'string' ? 1 : 2
	}

	if (opcode === 1) {
		// Save text frame
		payload = payload.toString()
		this.frameBuffer = this.frameBuffer ? this.frameBuffer + payload : payload

		if (fin) {
			// Emits 'text' event
			this.emit('text', this.frameBuffer)
			this.frameBuffer = null
		}
	} else {
		// Sends the buffer for InStream object
		if (!this.frameBuffer) {
			// Emits the 'binary' event
			this.frameBuffer = new InStream
			this.emit('binary', this.frameBuffer)
		}
		this.frameBuffer.addData(payload)

		if (fin) {
			// Emits 'end' event
			this.frameBuffer.end()
			this.frameBuffer = null
		}
	}

	return true
}
```
- example usage
```shell
...
		for (i = 0; i < payload.length; i++) {
			payload[i] ^= mask[i % 4]
		}
	}
	this.buffer = this.buffer.slice(start + len)

	// Proceeds to frame processing
	return this.processFrame(fin, opcode, payload)
}

/**
* Process a given frame received
* @param {boolean} fin
* @param {number} opcode
* @param {Buffer} payload
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.readHandshake"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>readHandshake ()](#apidoc.element.nodejs-websocket.Connection.prototype.readHandshake)
- description and source-code
```javascript
readHandshake = function () {
	var found = false,
		i, data

	// Do the handshake and try to connect
	if (this.buffer.length > Connection.maxBufferLength) {
		// Too big for a handshake
		if (this.server) {
			this.socket.end('HTTP/1.1 400 Bad Request\r\n\r\n')
		} else {
			this.socket.end()
			this.emit('error', new Error('Handshake is too big'))
		}
		return false
	}

	// Search for '\r\n\r\n'
	for (i = 0; i < this.buffer.length - 3; i++) {
		if (this.buffer[i] === 13 && this.buffer[i + 2] === 13 &&
			this.buffer[i + 1] === 10 && this.buffer[i + 3] === 10) {
			found = true
			break
		}
	}
	if (!found) {
		// Wait for more data
		return false
	}
	data = this.buffer.slice(0, i + 4).toString().split('\r\n')
	if (this.server ? this.answerHandshake(data) : this.checkHandshake(data)) {
		this.buffer = this.buffer.slice(i + 4)
		this.readyState = this.OPEN
		this.emit('connect')
		return true
	} else {
		this.socket.end(this.server ? 'HTTP/1.1 400 Bad Request\r\n\r\n' : undefined)
		return false
	}
}
```
- example usage
```shell
...
		return
	}

	// Save to the internal buffer
	this.buffer = Buffer.concat([this.buffer, buffer], this.buffer.length + buffer.length)

	if (this.readyState === this.CONNECTING) {
		if (!this.readHandshake()) {
			// May have failed or we're waiting for more data
			return
		}
	}

	if (this.readyState !== this.CLOSED) {
		// Try to read as many frames as possible
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.readHeaders"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>readHeaders (lines)](#apidoc.element.nodejs-websocket.Connection.prototype.readHeaders)
- description and source-code
```javascript
readHeaders = function (lines) {
	var i, match

	// Extract all headers
	// Ignore bad-formed lines and ignore the first line (HTTP header)
	for (i = 1; i < lines.length; i++) {
		if ((match = lines[i].match(/^([a-z-]+): (.+)$/i))) {
			this.headers[match[1].toLowerCase()] = match[2]
		}
	}
}
```
- example usage
```shell
...
	}
	if (!lines[0].match(/^HTTP\/\d\.\d 101( .*)?$/i)) {
		this.emit('error', new Error('Invalid handshake: invalid first line format'))
		return false
	}

	// Extract all headers
	this.readHeaders(lines)

	// Validate necessary headers
	if (!('upgrade' in this.headers) ||
		!('sec-websocket-accept' in this.headers) ||
		!('connection' in this.headers)) {
		this.emit('error', new Error('Invalid handshake: missing required headers'))
		return false
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.send"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>send (data, callback)](#apidoc.element.nodejs-websocket.Connection.prototype.send)
- description and source-code
```javascript
send = function (data, callback) {
	if (typeof data === 'string') {
		this.sendText(data, callback)
	} else if (Buffer.isBuffer(data)) {
		this.sendBinary(data, callback)
	} else {
		throw new TypeError('data should be either a string or a Buffer instance')
	}
}
```
- example usage
```shell
...
The binary transmission will end when the WritableStream finishes (like when you call .end on it)

## connection.sendBinary(data, [callback])
Sends a single chunk of binary data (like calling connection.beginBinary().end(data))

'callback' will be added as a listener to write operation over the socket

## connection.send(data, [callback])
Sends a given string or Buffer to the other side. This is simply an alias for 'sendText()' if data is a string or 'sendBinary()'
if the data is a Buffer.

'callback' will be added as a listener to write operation over the socket

## connection.sendPing([data=''])
Sends a [ping](http://tools.ietf.org/html/rfc6455#section-5.5.2) with optional payload
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.sendBinary"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>sendBinary (data, callback)](#apidoc.element.nodejs-websocket.Connection.prototype.sendBinary)
- description and source-code
```javascript
sendBinary = function (data, callback) {
	if (this.readyState === this.OPEN) {
		if (!this.outStream) {
			return this.socket.write(frame.createBinaryFrame(data, !this.server, true, true), callback)
		}
		this.emit('error', new Error('You can\'t send more binary frames until you finish sending the previous binary frames'))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}
```
- example usage
```shell
...

'callback' will be added as a listener to write operation over the socket

## connection.beginBinary()
Asks the connection to begin transmitting binary data. Returns a WritableStream.
The binary transmission will end when the WritableStream finishes (like when you call .end on it)

## connection.sendBinary(data, [callback])
Sends a single chunk of binary data (like calling connection.beginBinary().end(data))

'callback' will be added as a listener to write operation over the socket

## connection.send(data, [callback])
Sends a given string or Buffer to the other side. This is simply an alias for 'sendText()' if data is a string or 'sendBinary()'
if the data is a Buffer.
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.sendPing"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>sendPing (data)](#apidoc.element.nodejs-websocket.Connection.prototype.sendPing)
- description and source-code
```javascript
sendPing = function (data) {
	if (this.readyState === this.OPEN) {
		this.socket.write(frame.createPingFrame(data || '', !this.server))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}
```
- example usage
```shell
...
'callback' will be added as a listener to write operation over the socket

## connection.send(data, [callback])
Sends a given string or Buffer to the other side. This is simply an alias for 'sendText()' if data is a string or 'sendBinary()'
if the data is a Buffer.

'callback' will be added as a listener to write operation over the socket

## connection.sendPing([data=''])
Sends a [ping](http://tools.ietf.org/html/rfc6455#section-5.5.2) with optional payload

## connection.close([code, [reason]])
Starts the closing handshake (sends a close frame)

## connection.socket
The underlying net or tls socket
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.sendText"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>sendText (str, callback)](#apidoc.element.nodejs-websocket.Connection.prototype.sendText)
- description and source-code
```javascript
sendText = function (str, callback) {
	if (this.readyState === this.OPEN) {
		if (!this.outStream) {
			return this.socket.write(frame.createTextFrame(str, !this.server), callback)
		}
		this.emit('error', new Error('You can\'t send a text frame until you finish sending binary frames'))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}
```
- example usage
```shell
...
var ws = require("nodejs-websocket")

// Scream server example: "hi" -> "HI!!!"
var server = ws.createServer(function (conn) {
	console.log("New connection")
	conn.on("text", function (str) {
		console.log("Received "+str)
		conn.sendText(str.toUpperCase()+"!!!")
	})
	conn.on("close", function (code, reason) {
		console.log("Connection closed")
	})
}).listen(8001)
'''
...
```

#### <a name="apidoc.element.nodejs-websocket.Connection.prototype.startHandshake"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Connection.prototype.</span>startHandshake ()](#apidoc.element.nodejs-websocket.Connection.prototype.startHandshake)
- description and source-code
```javascript
startHandshake = function () {
	var str, i, key, headers, header
	key = new Buffer(16)
	for (i = 0; i < 16; i++) {
		key[i] = Math.floor(Math.random() * 256)
	}
	this.key = key.toString('base64')
	headers = {
		Host: this.host,
		Upgrade: 'websocket',
		Connection: 'Upgrade',
		'Sec-WebSocket-Key': this.key,
		'Sec-WebSocket-Version': '13'
	}

	if (this.protocols && this.protocols.length) {
		headers['Sec-WebSocket-Protocol'] = this.protocols.join(', ')
	}

	for (header in this.extraHeaders) {
		headers[header] = this.extraHeaders[header]
	}

	str = this.buildRequest('GET ' + this.path + ' HTTP/1.1', headers)
	this.socket.write(str)
}
```
- example usage
```shell
...
	socket.on('error', function (err) {
		that.emit('error', err)
	})

	if (!this.server) {
		connectEvent = socket.constructor.name === 'CleartextStream' ? 'secureConnect' : 'connect'
		socket.on(connectEvent, function () {
			that.startHandshake()
		})
	}

	// Close listeners
	var onclose = function () {
		if (that.readyState === that.CONNECTING || that.readyState === that.OPEN) {
			that.emit('close', 1006, '')
...
```



# <a name="apidoc.module.nodejs-websocket.InStream"></a>[module nodejs-websocket.InStream](#apidoc.module.nodejs-websocket.InStream)

#### <a name="apidoc.element.nodejs-websocket.InStream.InStream"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>InStream ()](#apidoc.element.nodejs-websocket.InStream.InStream)
- description and source-code
```javascript
function InStream() {
	stream.Readable.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.InStream.super_"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.InStream.</span>super_ (options)](#apidoc.element.nodejs-websocket.InStream.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodejs-websocket.InStream.prototype"></a>[module nodejs-websocket.InStream.prototype](#apidoc.module.nodejs-websocket.InStream.prototype)

#### <a name="apidoc.element.nodejs-websocket.InStream.prototype._read"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.InStream.prototype.</span>_read ()](#apidoc.element.nodejs-websocket.InStream.prototype._read)
- description and source-code
```javascript
_read = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.InStream.prototype.addData"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.InStream.prototype.</span>addData (data)](#apidoc.element.nodejs-websocket.InStream.prototype.addData)
- description and source-code
```javascript
addData = function (data) {
	this.push(data)
}
```
- example usage
```shell
...
	} else {
		// Sends the buffer for InStream object
		if (!this.frameBuffer) {
			// Emits the 'binary' event
			this.frameBuffer = new InStream
			this.emit('binary', this.frameBuffer)
		}
		this.frameBuffer.addData(payload)

		if (fin) {
			// Emits 'end' event
			this.frameBuffer.end()
			this.frameBuffer = null
		}
	}
...
```

#### <a name="apidoc.element.nodejs-websocket.InStream.prototype.end"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.InStream.prototype.</span>end ()](#apidoc.element.nodejs-websocket.InStream.prototype.end)
- description and source-code
```javascript
end = function () {
	this.push(null)
}
```
- example usage
```shell
...
'callback' will be added as a listener to write operation over the socket

## connection.beginBinary()
Asks the connection to begin transmitting binary data. Returns a WritableStream.
The binary transmission will end when the WritableStream finishes (like when you call .end on it)

## connection.sendBinary(data, [callback])
Sends a single chunk of binary data (like calling connection.beginBinary().end(data))

'callback' will be added as a listener to write operation over the socket

## connection.send(data, [callback])
Sends a given string or Buffer to the other side. This is simply an alias for 'sendText()' if data is a string or 'sendBinary()'
if the data is a Buffer.

'callback' will be added as a listener to write operation over the socket
...
```



# <a name="apidoc.module.nodejs-websocket.OutStream"></a>[module nodejs-websocket.OutStream](#apidoc.module.nodejs-websocket.OutStream)

#### <a name="apidoc.element.nodejs-websocket.OutStream.OutStream"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>OutStream (connection, minSize)](#apidoc.element.nodejs-websocket.OutStream.OutStream)
- description and source-code
```javascript
function OutStream(connection, minSize) {
	var that = this
	this.connection = connection
	this.minSize = minSize
	this.buffer = new Buffer(0)
	this.hasSent = false // Indicates if any frame has been sent yet
	stream.Writable.call(this)
	this.on('finish', function () {
		if (that.connection.readyState === that.connection.OPEN) {
			// Ignore if not connected anymore
			that.connection.socket.write(frame.createBinaryFrame(that.buffer, !that.connection.server, !that.hasSent, true))
		}
		that.connection.outStream = null
	})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.OutStream.super_"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.OutStream.</span>super_ (options)](#apidoc.element.nodejs-websocket.OutStream.super_)
- description and source-code
```javascript
function Writable(options) {
  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!(realHasInstance.call(Writable, this)) &&
      !(this instanceof Stream.Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function')
      this._write = options.write;

    if (typeof options.writev === 'function')
      this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodejs-websocket.OutStream.prototype"></a>[module nodejs-websocket.OutStream.prototype](#apidoc.module.nodejs-websocket.OutStream.prototype)

#### <a name="apidoc.element.nodejs-websocket.OutStream.prototype._write"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.OutStream.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.nodejs-websocket.OutStream.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
	var frameBuffer
	this.buffer = Buffer.concat([this.buffer, chunk], this.buffer.length + chunk.length)
	if (this.buffer.length >= this.minSize) {
		if (this.connection.readyState === this.connection.OPEN) {
			// Ignore if not connected anymore
			frameBuffer = frame.createBinaryFrame(this.buffer, !this.connection.server, !this.hasSent, false)
			this.connection.socket.write(frameBuffer, encoding, callback)
		}
		this.buffer = new Buffer(0)
		this.hasSent = true
		if (this.connection.readyState !== this.connection.OPEN) {
			callback()
		}
	} else {
		callback()
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodejs-websocket.Server"></a>[module nodejs-websocket.Server](#apidoc.module.nodejs-websocket.Server)

#### <a name="apidoc.element.nodejs-websocket.Server.Server"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.</span>Server (secure, options, callback)](#apidoc.element.nodejs-websocket.Server.Server)
- description and source-code
```javascript
function Server(secure, options, callback) {
	var that = this

	if (typeof options === 'function') {
		callback = options
		options = undefined
	}

	var onConnection = function (socket) {
		var conn = new Connection(socket, that, function () {
			that.connections.push(conn)
			conn.removeListener('error', nop)
			that.emit('connection', conn)
		})
		conn.on('close', function () {
			var pos = that.connections.indexOf(conn)
			if (pos !== -1) {
				that.connections.splice(pos, 1)
			}
		})

		// Ignore errors before the connection is established
		conn.on('error', nop)
	}

	if (secure) {
		this.socket = tls.createServer(options, onConnection)
	} else {
		this.socket = net.createServer(options, onConnection)
	}

	this.socket.on('close', function () {
		that.emit('close')
	})
	this.socket.on('error', function (err) {
		that.emit('error', err)
	})
	this.connections = []

	// super constructor
	events.EventEmitter.call(this)
	if (callback) {
		this.on('connection', callback)
	}

	// Add protocol agreement handling
	/**
	 * @member {?SelectProtocolCallback}
	 * @private
	 */
	this._selectProtocol = null

	if (options && options.selectProtocol) {
		// User-provided logic
		this._selectProtocol = options.selectProtocol
	} else if (options && options.validProtocols) {
		// Default logic
		this._selectProtocol = this._buildSelectProtocol(options.validProtocols)
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodejs-websocket.Server.super_"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Server.</span>super_ ()](#apidoc.element.nodejs-websocket.Server.super_)
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



# <a name="apidoc.module.nodejs-websocket.Server.prototype"></a>[module nodejs-websocket.Server.prototype](#apidoc.module.nodejs-websocket.Server.prototype)

#### <a name="apidoc.element.nodejs-websocket.Server.prototype._buildSelectProtocol"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Server.prototype.</span>_buildSelectProtocol (validProtocols)](#apidoc.element.nodejs-websocket.Server.prototype._buildSelectProtocol)
- description and source-code
```javascript
_buildSelectProtocol = function (validProtocols) {
	return function (conn, protocols) {
		var i

		for (i = 0; i < protocols.length; i++) {
			if (validProtocols.indexOf(protocols[i]) !== -1) {
				// A valid protocol was found
				return protocols[i]
			}
		}

		// No agreement
	}
}
```
- example usage
```shell
...
	this._selectProtocol = null

	if (options && options.selectProtocol) {
		// User-provided logic
		this._selectProtocol = options.selectProtocol
	} else if (options && options.validProtocols) {
		// Default logic
		this._selectProtocol = this._buildSelectProtocol(options.validProtocols)
	}
}

util.inherits(Server, events.EventEmitter)
module.exports = Server

Connection = require('./Connection')
...
```

#### <a name="apidoc.element.nodejs-websocket.Server.prototype.close"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Server.prototype.</span>close (callback)](#apidoc.element.nodejs-websocket.Server.prototype.close)
- description and source-code
```javascript
close = function (callback) {
	if (callback) {
		this.once('close', callback)
	}
	this.socket.close()
}
```
- example usage
```shell
...

If the 'host' is omitted, the server will accept connections directed to any IPv4 address (INADDR_ANY).

A 'port' value of zero will assign a random port.

'callback' will be added as an listener for the ''listening'' event.

## server.close([callback])
Stops the server from accepting new connections and keeps existing connections. This function is asynchronous, the server is finally
 closed when all connections are ended and the server emits a 'close' event. The optional callback will be called once the 'close
' event occurs.

## server.socket
The underlying socket, returned by net.createServer or tls.createServer

## server.connections
An Array with all connected clients. It's useful for broadcasting a message:
...
```

#### <a name="apidoc.element.nodejs-websocket.Server.prototype.listen"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.Server.prototype.</span>listen (port, host, callback)](#apidoc.element.nodejs-websocket.Server.prototype.listen)
- description and source-code
```javascript
listen = function (port, host, callback) {
	var that = this

	if (typeof host === 'function') {
		callback = host
		host = undefined
	}

	if (callback) {
		this.on('listening', callback)
	}

	this.socket.listen(port, host, function () {
		that.emit('listening')
	})

	return this
}
```
- example usage
```shell
...
	conn.on("text", function (str) {
		console.log("Received "+str)
		conn.sendText(str.toUpperCase()+"!!!")
	})
	conn.on("close", function (code, reason) {
		console.log("Connection closed")
	})
}).listen(8001)
'''

Se other examples inside the folder samples

# ws
The main object, returned by 'require("nodejs-websocket")'.
...
```



# <a name="apidoc.module.nodejs-websocket.frame"></a>[module nodejs-websocket.frame](#apidoc.module.nodejs-websocket.frame)

#### <a name="apidoc.element.nodejs-websocket.frame.createBinaryFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createBinaryFrame (data, masked, first, fin)](#apidoc.element.nodejs-websocket.frame.createBinaryFrame)
- description and source-code
```javascript
createBinaryFrame = function (data, masked, first, fin) {
	var payload, meta

	first = first === undefined ? true : first
	masked = masked === undefined ? false : masked
	if (masked) {
		payload = new Buffer(data.length)
		data.copy(payload)
	} else {
		payload = data
	}
	meta = generateMetaData(fin === undefined ? true : fin, first ? 2 : 0, masked, payload)

	return Buffer.concat([meta, payload], meta.length + payload.length)
}
```
- example usage
```shell
...
 * Sends a binary buffer at once
 * @param {Buffer} data
 * @param {Function} [callback] will be executed when the data is finally written out
 */
Connection.prototype.sendBinary = function (data, callback) {
	if (this.readyState === this.OPEN) {
		if (!this.outStream) {
			return this.socket.write(frame.createBinaryFrame(data, !this.server, true, true), callback)
		}
		this.emit('error', new Error('You can\'t send more binary frames until you finish sending the previous binary frames'))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}
...
```

#### <a name="apidoc.element.nodejs-websocket.frame.createCloseFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createCloseFrame (code, reason, masked)](#apidoc.element.nodejs-websocket.frame.createCloseFrame)
- description and source-code
```javascript
createCloseFrame = function (code, reason, masked) {
	var payload, meta

	if (code !== undefined && code !== 1005) {
		payload = new Buffer(reason === undefined ? '--' : '--' + reason)
		payload.writeUInt16BE(code, 0)
	} else {
		payload = new Buffer(0)
	}
	meta = generateMetaData(true, 8, masked === undefined ? false : masked, payload)

	return Buffer.concat([meta, payload], meta.length + payload.length)
}
```
- example usage
```shell
...
 * If the connection isn't OPEN, closes it without sending a close frame
 * @param {number} [code]
 * @param {string} [reason]
 * @fires close
 */
Connection.prototype.close = function (code, reason) {
	if (this.readyState === this.OPEN) {
		this.socket.write(frame.createCloseFrame(code, reason, !this.server))
		this.readyState = this.CLOSING
	} else if (this.readyState !== this.CLOSED) {
		this.socket.end()
		this.readyState = this.CLOSED
	}
	this.emit('close', code, reason)
}
...
```

#### <a name="apidoc.element.nodejs-websocket.frame.createPingFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createPingFrame (data, masked)](#apidoc.element.nodejs-websocket.frame.createPingFrame)
- description and source-code
```javascript
createPingFrame = function (data, masked) {
	var payload, meta

	payload = new Buffer(data)
	meta = generateMetaData(true, 9, masked === undefined ? false : masked, payload)

	return Buffer.concat([meta, payload], meta.length + payload.length)
}
```
- example usage
```shell
...
/**
* Sends a ping to the remote
* @param {string} [data=''] - optional ping data
* @fires pong when pong reply is received
*/
Connection.prototype.sendPing = function (data) {
	if (this.readyState === this.OPEN) {
		this.socket.write(frame.createPingFrame(data || '', !this.server))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}

/**
* Close the connection, sending a close frame and waiting for response
...
```

#### <a name="apidoc.element.nodejs-websocket.frame.createPongFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createPongFrame (data, masked)](#apidoc.element.nodejs-websocket.frame.createPongFrame)
- description and source-code
```javascript
createPongFrame = function (data, masked) {
	var payload, meta

	payload = new Buffer(data)
	meta = generateMetaData(true, 10, masked === undefined ? false : masked, payload)

	return Buffer.concat([meta, payload], meta.length + payload.length)
}
```
- example usage
```shell
...
		} else if (this.readyState === this.OPEN) {
			this.processCloseFrame(payload)
		}
		return true
	} else if (opcode === 9) {
		// Ping frame
		if (this.readyState === this.OPEN) {
			this.socket.write(frame.createPongFrame(payload.toString(), !this.server))
		}
		return true
	} else if (opcode === 10) {
		// Pong frame
		this.emit('pong', payload.toString())
		return true
	}
...
```

#### <a name="apidoc.element.nodejs-websocket.frame.createTextFrame"></a>[function <span class="apidocSignatureSpan">nodejs-websocket.frame.</span>createTextFrame (data, masked)](#apidoc.element.nodejs-websocket.frame.createTextFrame)
- description and source-code
```javascript
createTextFrame = function (data, masked) {
	var payload, meta

	payload = new Buffer(data)
	meta = generateMetaData(true, 1, masked === undefined ? false : masked, payload)

	return Buffer.concat([meta, payload], meta.length + payload.length)
}
```
- example usage
```shell
...
 * Send a given string to the other side
 * @param {string} str
 * @param {Function} [callback] will be executed when the data is finally written out
 */
Connection.prototype.sendText = function (str, callback) {
	if (this.readyState === this.OPEN) {
		if (!this.outStream) {
			return this.socket.write(frame.createTextFrame(str, !this.server), callback)
		}
		this.emit('error', new Error('You can\'t send a text frame until you finish sending binary frames'))
	} else {
		this.emit('error', new Error('You can\'t write to a non-open connection'))
	}
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
