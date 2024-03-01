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
* __Machine:__ Linux fv-az1020-757 6.5.0-1015-azure #15~22.04.1-Ubuntu SMP Tue Feb 13 01:15:12 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri Mar  1 01:05:28 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 73882.0    | 13.04   | 13.18         |
| 0http                    | 3.5.2   | ✓      | 71303.6    | 13.54   | 12.72         |
| fastify                  | 3.29.5  | ✓      | 66528.4    | 14.54   | 11.87         |
| bare                     | 10.13.0 | ✗      | 65960.0    | 14.66   | 11.76         |
| polka                    | 0.5.2   | ✓      | 63451.2    | 15.26   | 11.32         |
| foxify                   | 0.10.20 | ✓      | 63120.8    | 15.35   | 10.35         |
| connect                  | 3.7.0   | ✗      | 63016.0    | 15.38   | 11.24         |
| restana                  | 4.9.7   | ✓      | 62703.2    | 15.45   | 11.18         |
| micro                    | 9.4.1   | ✗      | 60713.6    | 15.98   | 10.83         |
| server-base              | 7.1.32  | ✗      | 59804.0    | 16.22   | 10.67         |
| yeps                     | 1.1.1   | ✗      | 57403.2    | 16.93   | 10.24         |
| connect-router           | 1.3.8   | ✓      | 55664.8    | 17.47   | 9.93          |
| server-base-router       | 6.1.5   | ✓      | 55619.2    | 17.48   | 9.92          |
| micro-route              | 2.5.0   | ✓      | 54930.4    | 17.71   | 9.80          |
| trek-engine              | 1.0.5   | ✗      | 54206.4    | 17.95   | 8.89          |
| trek-router              | 1.2.0   | ✓      | 53385.6    | 18.24   | 8.76          |
| yeps-router              | 1.2.0   | ✓      | 47288.8    | 20.65   | 8.43          |
| vapr                     | 0.5.5   | ✓      | 46569.6    | 20.98   | 7.64          |
| koa                      | 2.15.0  | ✗      | 45807.2    | 21.33   | 8.17          |
| spirit                   | 0.6.1   | ✗      | 44926.4    | 21.76   | 8.01          |
| restify                  | 8.6.1   | ✓      | 43214.4    | 22.64   | 7.79          |
| spirit-router            | 0.5.0   | ✓      | 43047.2    | 22.75   | 7.68          |
| total.js                 | 3.4.13  | ✓      | 42367.2    | 23.10   | 12.97         |
| koa-router               | 10.1.1  | ✓      | 40859.2    | 23.97   | 7.29          |
| hapi                     | 20.3.0  | ✓      | 35509.4    | 27.66   | 6.33          |
| microrouter              | 3.1.3   | ✓      | 33940.6    | 28.95   | 6.05          |
| express                  | 4.18.3  | ✓      | 15029.4    | 65.99   | 2.68          |
| fastify-big-json         | 3.29.5  | ✓      | 13048.2    | 76.09   | 150.11        |
| express-with-middlewares | 4.18.3  | ✓      | 12578.2    | 78.93   | 4.82          |
| express-route-prefix     | 4.18.3  | ✓      | 11313.8    | 87.81   | 4.19          |
| egg.js                   | 2.37.0  | ✓      | 10497.8    | 94.71   | 3.69          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
