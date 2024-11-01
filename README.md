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
* __Machine:__ Linux fv-az2026-920 6.5.0-1025-azure #26~22.04.1-Ubuntu SMP Thu Jul 11 22:33:04 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri Nov  1 01:11:40 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74708.4    | 12.89   | 13.32         |
| fastify                  | 3.29.5  | ✓      | 66584.8    | 14.53   | 11.87         |
| bare                     | 10.13.0 | ✗      | 65042.4    | 14.88   | 11.60         |
| polka                    | 0.5.2   | ✓      | 63185.6    | 15.33   | 11.27         |
| foxify                   | 0.10.20 | ✓      | 62858.4    | 15.41   | 10.31         |
| connect                  | 3.7.0   | ✗      | 62059.2    | 15.62   | 11.07         |
| micro                    | 9.4.1   | ✗      | 61016.8    | 15.89   | 10.88         |
| server-base              | 7.1.32  | ✗      | 60444.8    | 16.05   | 10.78         |
| yeps                     | 1.1.1   | ✗      | 58922.4    | 16.47   | 10.51         |
| server-base-router       | 6.1.5   | ✓      | 55408.8    | 17.55   | 9.88          |
| connect-router           | 1.3.8   | ✓      | 55321.6    | 17.58   | 9.87          |
| micro-route              | 2.5.0   | ✓      | 54296.0    | 17.92   | 9.68          |
| trek-engine              | 1.0.5   | ✗      | 53028.0    | 18.36   | 8.70          |
| trek-router              | 1.2.0   | ✓      | 52580.8    | 18.52   | 8.63          |
| yeps-router              | 1.2.0   | ✓      | 47060.8    | 20.75   | 8.39          |
| vapr                     | 0.5.5   | ✓      | 46211.2    | 21.14   | 7.58          |
| spirit                   | 0.6.1   | ✗      | 45748.0    | 21.36   | 8.16          |
| spirit-router            | 0.5.0   | ✓      | 45148.0    | 21.67   | 8.05          |
| koa                      | 2.15.3  | ✗      | 44707.2    | 21.87   | 7.97          |
| restify                  | 8.6.1   | ✓      | 41962.4    | 23.33   | 7.56          |
| total.js                 | 3.4.13  | ✓      | 41220.0    | 23.76   | 12.62         |
| koa-router               | 10.1.1  | ✓      | 40505.6    | 24.19   | 7.22          |
| hapi                     | 20.3.0  | ✓      | 35642.2    | 27.56   | 6.36          |
| microrouter              | 3.1.3   | ✓      | 33135.2    | 29.68   | 5.91          |
| express                  | 4.21.1  | ✓      | 14410.4    | 68.86   | 2.57          |
| fastify-big-json         | 3.29.5  | ✓      | 13392.2    | 74.12   | 154.06        |
| express-with-middlewares | 4.21.1  | ✓      | 12415.2    | 79.97   | 4.76          |
| express-route-prefix     | 4.21.1  | ✓      | 10999.6    | 90.32   | 4.07          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
