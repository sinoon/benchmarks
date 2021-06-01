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
* __Machine:__ Linux fv-az93-397 5.4.0-1047-azure #49-Ubuntu SMP Thu Apr 22 14:30:37 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.1`
* __Run:__ Tue Jun  1 01:13:41 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 43015.2    | 22.78   | 7.67          |
| micro                    | 9.3.4   | ✗      | 42917.6    | 22.81   | 7.65          |
| fastify                  | 3.17.0  | ✓      | 41167.2    | 23.80   | 7.34          |
| foxify                   | 0.10.20 | ✓      | 41015.2    | 23.89   | 6.73          |
| polka                    | 0.5.2   | ✓      | 40752.8    | 24.04   | 7.27          |
| 0http                    | 3.1.1   | ✓      | 40210.2    | 24.38   | 7.17          |
| bare                     | 10.13.0 | ✗      | 40000.0    | 24.50   | 7.13          |
| connect                  | 3.7.0   | ✗      | 39686.4    | 24.69   | 7.08          |
| rayo                     | 1.3.6   | ✓      | 37247.4    | 26.35   | 6.64          |
| server-base              | 7.1.27  | ✗      | 36033.4    | 27.26   | 6.43          |
| connect-router           | 1.3.5   | ✓      | 35082.0    | 28.01   | 6.26          |
| spirit-router            | 0.5.0   | ✓      | 34870.2    | 28.23   | 6.22          |
| trek-engine              | 1.0.5   | ✗      | 34028.0    | 28.89   | 5.58          |
| server-base-router       | 6.1.5   | ✓      | 33926.2    | 28.98   | 6.05          |
| spirit                   | 0.6.1   | ✗      | 33303.2    | 29.57   | 5.94          |
| yeps                     | 1.1.1   | ✗      | 32764.8    | 30.02   | 5.84          |
| micro-route              | 2.5.0   | ✓      | 32232.6    | 30.52   | 5.75          |
| trek-router              | 1.2.0   | ✓      | 30662.4    | 32.11   | 5.03          |
| yeps-router              | 1.2.0   | ✓      | 30432.4    | 32.37   | 5.43          |
| koa                      | 2.13.1  | ✗      | 28917.2    | 34.09   | 5.16          |
| vapr                     | 0.5.5   | ✓      | 28568.0    | 34.50   | 4.69          |
| restify                  | 8.5.1   | ✓      | 26419.2    | 37.37   | 4.76          |
| restana                  | 4.9.1   | ✓      | 26149.2    | 37.73   | 4.66          |
| total.js                 | 3.4.8   | ✓      | 25354.8    | 38.94   | 7.76          |
| koa-router               | 10.0.0  | ✓      | 23390.4    | 42.27   | 4.17          |
| hapi                     | 20.1.3  | ✓      | 21745.6    | 45.47   | 3.88          |
| microrouter              | 3.1.3   | ✓      | 19306.0    | 51.28   | 3.44          |
| egg.js                   | 2.29.4  | ✓      | 14248.6    | 69.67   | 5.01          |
| express                  | 4.17.1  | ✓      | 8772.5     | 113.39  | 1.56          |
| fastify-big-json         | 3.17.0  | ✓      | 8248.9     | 120.58  | 94.90         |
| express-with-middlewares | 4.17.1  | ✓      | 7678.8     | 129.66  | 2.94          |
| express-route-prefix     | 4.17.1  | ✓      | 7164.3     | 138.95  | 2.65          |
| farrow-http              | 1.10.6  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
