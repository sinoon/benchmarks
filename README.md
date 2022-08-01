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
* __Machine:__ Linux fv-az74-311 5.15.0-1014-azure #17~20.04.1-Ubuntu SMP Thu Jun 23 20:01:51 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon Aug  1 01:08:39 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.29.1  | ✓      | 59240.0    | 16.40   | 10.57         |
| polka                    | 0.5.2   | ✓      | 57320.8    | 16.96   | 10.22         |
| polkadot                 | 1.0.0   | ✗      | 57207.2    | 17.00   | 10.20         |
| bare                     | 10.13.0 | ✗      | 57144.8    | 17.01   | 10.19         |
| foxify                   | 0.10.20 | ✓      | 55796.8    | 17.43   | 9.15          |
| connect                  | 3.7.0   | ✗      | 55412.0    | 17.55   | 9.88          |
| micro                    | 9.4.1   | ✗      | 54616.8    | 17.81   | 9.74          |
| rayo                     | 1.3.10  | ✓      | 53809.6    | 18.08   | 9.60          |
| 0http                    | 3.4.1   | ✓      | 52985.6    | 18.39   | 9.45          |
| server-base              | 7.1.32  | ✗      | 51872.0    | 18.78   | 9.25          |
| connect-router           | 1.3.7   | ✓      | 51511.2    | 18.92   | 9.19          |
| server-base-router       | 6.1.5   | ✓      | 51366.4    | 18.97   | 9.16          |
| yeps                     | 1.1.1   | ✗      | 50616.8    | 19.26   | 9.03          |
| restana                  | 4.9.6   | ✓      | 49988.8    | 19.52   | 8.91          |
| micro-route              | 2.5.0   | ✓      | 49824.8    | 19.57   | 8.89          |
| trek-router              | 1.2.0   | ✓      | 47451.2    | 20.58   | 7.78          |
| trek-engine              | 1.0.5   | ✗      | 46838.4    | 20.85   | 7.68          |
| yeps-router              | 1.2.0   | ✓      | 43740.0    | 22.36   | 7.80          |
| spirit                   | 0.6.1   | ✗      | 41232.0    | 23.78   | 7.35          |
| vapr                     | 0.5.5   | ✓      | 40772.8    | 24.03   | 6.69          |
| koa                      | 2.13.4  | ✗      | 40563.4    | 24.16   | 7.23          |
| spirit-router            | 0.5.0   | ✓      | 38702.4    | 25.36   | 6.90          |
| total.js                 | 3.4.13  | ✓      | 38014.4    | 25.80   | 11.64         |
| koa-router               | 10.1.1  | ✓      | 36150.6    | 27.16   | 6.45          |
| restify                  | 8.6.1   | ✓      | 35954.6    | 27.33   | 6.48          |
| hapi                     | 20.2.2  | ✓      | 29777.2    | 33.08   | 5.31          |
| microrouter              | 3.1.3   | ✓      | 27660.8    | 35.65   | 4.93          |
| egg.js                   | 2.36.0  | ✓      | 18752.5    | 52.83   | 6.60          |
| express                  | 4.18.1  | ✓      | 11179.6    | 88.91   | 1.99          |
| express-with-middlewares | 4.18.1  | ✓      | 9624.5     | 103.34  | 3.69          |
| express-route-prefix     | 4.18.1  | ✓      | 9536.0     | 104.29  | 3.53          |
| fastify-big-json         | 3.29.1  | ✓      | 9043.9     | 109.97  | 104.05        |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
