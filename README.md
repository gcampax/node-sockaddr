# node-sockaddr

[![Build Status](https://travis-ci.org/stanford-oval/node-sockaddr.svg?branch=master)](https://travis-ci.org/stanford-oval/node-sockaddr) [![Coverage Status](https://coveralls.io/repos/github/stanford-oval/node-sockaddr/badge.svg?branch=master)](https://coveralls.io/github/stanford-oval/node-sockaddr?branch=master) [![Dependency Status](https://david-dm.org/stanford-oval/node-sockaddr/status.svg)](https://david-dm.org/stanford-oval/node-sockaddr) [![Greenkeeper badge](https://badges.greenkeeper.io/stanford-oval/node-sockaddr.svg)](https://greenkeeper.io/) [![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/stanford-oval/node-sockaddr.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/stanford-oval/node-sockaddr/context:javascript)

A simple library to convert a string into an object suitable to pass to `net.Socket.connect` and `net.Server.listen`.
Useful for configuration files and setting hosts and ports in environment variables.
Supports both Unix domain sockets and TCP sockets.

## Usage

```javascript
const sockaddr = require('sockaddr');

let socket = ...;
socket.connect(sockaddr('hostname:1234'));
```

See [./test.js](./test.js) for the full set of options supported.
