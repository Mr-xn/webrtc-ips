# WebRTC IPs
[![Build Status](https://travis-ci.org/vitalets/webrtc-ips.svg?branch=master)](https://travis-ci.org/vitalets/webrtc-ips)
[![npm](https://img.shields.io/npm/v/webrtc-ips.svg)](https://www.npmjs.com/package/webrtc-ips)
[![license](https://img.shields.io/npm/l/webrtc-ips.svg)](https://www.npmjs.com/package/webrtc-ips)

This library uses WebRTC to detect your local IP address on the web page.

## Live Demo
https://vitalets.github.io/webrtc-ips/demo/


## Installation
```bash
npm i webrtc-ips
```

## Usage
```js
import {getIPs, getIPv4, getIPv6} from 'webrtc-ips';

const ips = await getIPs();
// => [{address: '95.108.174.12', v6: false}, {address: '2a02:6b8::408:5830:47a6:d045:a9ac', v6: true}]

const ipv4 = await getIPv4();
// => '95.108.174.12'

const ipv6 = await getIPv6();
// => '2a02:6b8::408:5830:47a6:d045:a9ac'

```

## Browser support
* Chrome (Windows, OSX, Android)
* Firefox (Windows, OSX, Android)

## Credits
This is a fork of original [diafygi/webrtc-ips](https://github.com/diafygi/webrtc-ips) project 
with refactored source code, added tests and published to npm. 

## License
MIT
