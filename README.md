<div align="center">
<img src="https://github.com/fastify/graphics/raw/master/full-logo.png" width="650" height="auto"/>
</div>

<div align="center">

[![Build Status](https://travis-ci.org/fastify/fastify.svg?branch=master)](https://travis-ci.org/fastify/fastify)
[![Coverage Status](https://coveralls.io/repos/github/fastify/fastify/badge.svg?branch=master)](https://coveralls.io/github/fastify/fastify?branch=master)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)
[![NPM version](https://img.shields.io/npm/v/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify)
[![NPM downloads](https://img.shields.io/npm/dm/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify) [![Gitter](https://badges.gitter.im/gitterHQ/gitter.svg)](https://gitter.im/fastify)
</div>
<br />

# TL;DR

* [Fastify](https://github.com/fastify/fastify) is, fast and low overhead web framework for Node.js
* This package shows how fast it is comparatively.

# Installing

```
npm i -g fastify-benchmarks
```

# Usage

```
benchmark [arguments (optional)]
```

#### Arguments

* `-h`: Help on how to use the tool.
* `compare`: Get comparative data for your benchmarks.

> You may also compare all test results, at once, in a single table; `benchmark compare -t`

> You can also extend the comparison table with percentage values based on fastest result; `benchmark compare -p`
# Benchmarks
* __Machine:__ Linux pkrvmf6wy0o8zjz 6.11.0-1014-azure #14~24.04.1-Ubuntu SMP Thu Apr 24 17:41:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Jun  1 01:20:06 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| server-base              | 7.1.32  | ✗      | 46057.6    | 21.23   | 8.21          |
| connect                  | 3.7.0   | ✗      | 45022.2    | 21.72   | 8.03          |
| polkadot                 | 1.0.0   | ✗      | 42985.0    | 22.81   | 7.67          |
| fastify                  | 3.29.5  | ✓      | 41993.6    | 23.34   | 7.49          |
| polka                    | 0.5.2   | ✓      | 41324.0    | 23.71   | 7.37          |
| connect-router           | 1.3.8   | ✓      | 39960.2    | 24.53   | 7.13          |
| server-base-router       | 6.1.5   | ✓      | 39348.0    | 24.94   | 7.02          |
| foxify                   | 0.10.20 | ✓      | 38337.6    | 25.61   | 6.29          |
| micro                    | 9.4.1   | ✗      | 38184.6    | 25.71   | 6.81          |
| bare                     | 10.13.0 | ✗      | 37926.0    | 25.89   | 6.76          |
| micro-route              | 2.5.0   | ✓      | 36506.6    | 26.90   | 6.51          |
| trek-engine              | 1.0.5   | ✗      | 34818.6    | 28.23   | 5.71          |
| restify                  | 8.6.1   | ✓      | 33917.8    | 28.98   | 6.11          |
| yeps                     | 1.1.1   | ✗      | 33273.2    | 29.56   | 5.93          |
| trek-router              | 1.2.0   | ✓      | 32346.4    | 30.43   | 5.31          |
| spirit                   | 0.6.1   | ✗      | 30529.0    | 32.27   | 5.44          |
| spirit-router            | 0.5.0   | ✓      | 28668.4    | 34.38   | 5.11          |
| vapr                     | 0.5.5   | ✓      | 28597.4    | 34.48   | 4.69          |
| yeps-router              | 1.2.0   | ✓      | 25480.0    | 38.76   | 4.54          |
| koa                      | 2.16.1  | ✗      | 25435.6    | 38.82   | 4.54          |
| total.js                 | 3.4.13  | ✓      | 25026.8    | 39.46   | 7.66          |
| koa-router               | 10.1.1  | ✓      | 23865.2    | 41.44   | 4.26          |
| microrouter              | 3.1.3   | ✓      | 21258.4    | 46.53   | 3.79          |
| hapi                     | 20.3.0  | ✓      | 21111.7    | 46.86   | 3.76          |
| express                  | 4.21.2  | ✓      | 10298.0    | 96.56   | 1.84          |
| express-with-middlewares | 4.21.2  | ✓      | 8903.3     | 111.59  | 3.41          |
| express-route-prefix     | 4.21.2  | ✓      | 5868.7     | 169.47  | 2.17          |
| fastify-big-json         | 3.29.5  | ✓      | 5669.1     | 175.58  | 65.22         |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
