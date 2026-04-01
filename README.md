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
* __Machine:__ Linux runnervmrg6be 6.17.0-1008-azure #8~24.04.1-Ubuntu SMP Mon Jan 26 18:35:40 UTC 2026 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Apr  1 01:31:23 UTC 2026

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75448.0    | 12.77   | 13.46         |
| bare                     | 10.13.0 | ✗      | 67403.6    | 14.35   | 12.02         |
| fastify                  | 3.29.5  | ✓      | 67114.8    | 14.40   | 11.97         |
| polka                    | 0.5.2   | ✓      | 64829.6    | 14.93   | 11.56         |
| foxify                   | 0.10.20 | ✓      | 64708.4    | 14.95   | 10.61         |
| connect                  | 3.7.0   | ✗      | 64097.2    | 15.11   | 11.43         |
| micro                    | 9.4.1   | ✗      | 62537.6    | 15.49   | 11.15         |
| server-base              | 7.1.32  | ✗      | 61482.4    | 15.77   | 10.96         |
| yeps                     | 1.1.1   | ✗      | 59837.6    | 16.22   | 10.67         |
| server-base-router       | 6.1.5   | ✓      | 57762.4    | 16.81   | 10.30         |
| connect-router           | 1.3.8   | ✓      | 57347.2    | 16.94   | 10.23         |
| trek-engine              | 1.0.5   | ✗      | 55465.6    | 17.53   | 9.10          |
| micro-route              | 2.5.0   | ✓      | 55392.8    | 17.56   | 9.88          |
| trek-router              | 1.2.0   | ✓      | 54550.4    | 17.83   | 8.95          |
| vapr                     | 0.5.5   | ✓      | 48233.6    | 20.24   | 7.91          |
| yeps-router              | 1.2.0   | ✓      | 48044.0    | 20.32   | 8.57          |
| koa                      | 2.16.4  | ✗      | 46296.0    | 21.10   | 8.26          |
| spirit-router            | 0.5.0   | ✓      | 44864.0    | 21.79   | 8.00          |
| total.js                 | 3.4.13  | ✓      | 43156.0    | 22.67   | 13.21         |
| spirit                   | 0.6.1   | ✗      | 43076.8    | 22.71   | 7.68          |
| restify                  | 8.6.1   | ✓      | 41697.6    | 23.48   | 7.52          |
| koa-router               | 10.1.1  | ✓      | 41348.8    | 23.68   | 7.37          |
| hapi                     | 20.3.0  | ✓      | 35140.8    | 27.96   | 6.27          |
| microrouter              | 3.1.3   | ✓      | 33422.0    | 29.41   | 5.96          |
| express                  | 4.22.1  | ✓      | 14345.2    | 69.16   | 2.56          |
| fastify-big-json         | 3.29.5  | ✓      | 12982.0    | 76.48   | 149.35        |
| express-with-middlewares | 4.22.1  | ✓      | 12390.4    | 80.13   | 4.75          |
| express-route-prefix     | 4.22.1  | ✓      | 10996.0    | 90.36   | 4.07          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
