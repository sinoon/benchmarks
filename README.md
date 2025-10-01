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
* __Machine:__ Linux runnervm3ublj 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Oct  1 01:15:14 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75256.0    | 12.80   | 13.42         |
| fastify                  | 3.29.5  | ✓      | 67897.2    | 14.23   | 12.11         |
| bare                     | 10.13.0 | ✗      | 67121.6    | 14.40   | 11.97         |
| foxify                   | 0.10.20 | ✓      | 64878.4    | 14.92   | 10.64         |
| polka                    | 0.5.2   | ✓      | 63740.0    | 15.19   | 11.37         |
| connect                  | 3.7.0   | ✗      | 62828.0    | 15.42   | 11.20         |
| micro                    | 9.4.1   | ✗      | 60832.0    | 15.94   | 10.85         |
| server-base              | 7.1.32  | ✗      | 60187.2    | 16.12   | 10.73         |
| yeps                     | 1.1.1   | ✗      | 58962.4    | 16.46   | 10.52         |
| connect-router           | 1.3.8   | ✓      | 57392.0    | 16.93   | 10.24         |
| micro-route              | 2.5.0   | ✓      | 56515.2    | 17.20   | 10.08         |
| server-base-router       | 6.1.5   | ✓      | 55641.6    | 17.48   | 9.92          |
| trek-engine              | 1.0.5   | ✗      | 54504.0    | 17.85   | 8.94          |
| trek-router              | 1.2.0   | ✓      | 51812.8    | 18.80   | 8.50          |
| yeps-router              | 1.2.0   | ✓      | 47697.6    | 20.47   | 8.51          |
| vapr                     | 0.5.5   | ✓      | 46488.8    | 21.01   | 7.63          |
| koa                      | 2.16.2  | ✗      | 44609.6    | 21.92   | 7.96          |
| spirit                   | 0.6.1   | ✗      | 44331.2    | 22.06   | 7.91          |
| spirit-router            | 0.5.0   | ✓      | 43112.0    | 22.71   | 7.69          |
| total.js                 | 3.4.13  | ✓      | 42840.8    | 22.84   | 13.12         |
| restify                  | 8.6.1   | ✓      | 41940.8    | 23.34   | 7.56          |
| koa-router               | 10.1.1  | ✓      | 40343.2    | 24.29   | 7.19          |
| hapi                     | 20.3.0  | ✓      | 35414.4    | 27.74   | 6.32          |
| microrouter              | 3.1.3   | ✓      | 33084.6    | 29.73   | 5.90          |
| express                  | 4.21.2  | ✓      | 14491.2    | 68.48   | 2.58          |
| fastify-big-json         | 3.29.5  | ✓      | 12859.8    | 77.21   | 147.96        |
| express-with-middlewares | 4.21.2  | ✓      | 12418.8    | 79.98   | 4.76          |
| express-route-prefix     | 4.21.2  | ✓      | 11120.6    | 89.34   | 4.11          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
