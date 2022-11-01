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
* __Machine:__ Linux fv-az290-341 5.15.0-1022-azure #27~20.04.1-Ubuntu SMP Mon Oct 17 02:03:50 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Tue Nov  1 01:13:02 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 43474.4    | 22.52   | 7.75          |
| fastify                  | 3.29.3  | ✓      | 40615.2    | 24.12   | 7.24          |
| micro                    | 9.4.1   | ✗      | 37929.6    | 25.87   | 6.76          |
| polka                    | 0.5.2   | ✓      | 37698.2    | 26.03   | 6.72          |
| 0http                    | 3.4.1   | ✓      | 37442.6    | 26.21   | 6.68          |
| connect                  | 3.7.0   | ✗      | 37239.0    | 26.37   | 6.64          |
| bare                     | 10.13.0 | ✗      | 37170.6    | 26.41   | 6.63          |
| foxify                   | 0.10.20 | ✓      | 36682.2    | 26.76   | 6.02          |
| yeps                     | 1.1.1   | ✗      | 35235.2    | 27.88   | 6.28          |
| rayo                     | 1.3.10  | ✓      | 34234.6    | 28.71   | 6.11          |
| restana                  | 4.9.6   | ✓      | 33220.2    | 29.60   | 5.92          |
| connect-router           | 1.3.7   | ✓      | 32177.4    | 30.58   | 5.74          |
| server-base              | 7.1.32  | ✗      | 31696.4    | 31.05   | 5.65          |
| trek-router              | 1.2.0   | ✓      | 30008.8    | 32.83   | 4.92          |
| micro-route              | 2.5.0   | ✓      | 29250.8    | 33.68   | 5.22          |
| spirit                   | 0.6.1   | ✗      | 29043.2    | 34.00   | 5.18          |
| server-base-router       | 6.1.5   | ✓      | 29021.2    | 33.95   | 5.18          |
| yeps-router              | 1.2.0   | ✓      | 28764.4    | 34.27   | 5.13          |
| spirit-router            | 0.5.0   | ✓      | 28124.8    | 35.09   | 5.02          |
| trek-engine              | 1.0.5   | ✗      | 28006.4    | 35.20   | 4.59          |
| koa                      | 2.13.4  | ✗      | 26143.6    | 37.74   | 4.66          |
| vapr                     | 0.5.5   | ✓      | 24565.2    | 40.20   | 4.03          |
| restify                  | 8.6.1   | ✓      | 24304.0    | 40.64   | 4.38          |
| total.js                 | 3.4.13  | ✓      | 23370.8    | 42.29   | 7.15          |
| koa-router               | 10.1.1  | ✓      | 21831.6    | 45.29   | 3.89          |
| hapi                     | 20.2.2  | ✓      | 20452.4    | 48.38   | 3.65          |
| microrouter              | 3.1.3   | ✓      | 19403.2    | 51.04   | 3.46          |
| egg.js                   | 2.37.0  | ✓      | 12476.4    | 79.61   | 4.39          |
| express                  | 4.18.2  | ✓      | 8041.6     | 123.73  | 1.43          |
| fastify-big-json         | 3.29.3  | ✓      | 7855.1     | 126.67  | 90.37         |
| express-route-prefix     | 4.18.2  | ✓      | 7249.4     | 137.20  | 2.68          |
| express-with-middlewares | 4.18.2  | ✓      | 6783.0     | 146.75  | 2.60          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
