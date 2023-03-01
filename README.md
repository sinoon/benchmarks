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
* __Machine:__ Linux fv-az578-101 5.15.0-1033-azure #40-Ubuntu SMP Mon Jan 23 20:36:59 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Mar  1 01:08:36 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 39915.0    | 24.59   | 7.12          |
| fastify                  | 3.29.5  | ✓      | 38807.2    | 25.28   | 6.92          |
| bare                     | 10.13.0 | ✗      | 37719.0    | 26.02   | 6.73          |
| 0http                    | 3.4.4   | ✓      | 37165.4    | 26.41   | 6.63          |
| foxify                   | 0.10.20 | ✓      | 36362.6    | 27.01   | 5.96          |
| connect                  | 3.7.0   | ✗      | 36257.0    | 27.08   | 6.47          |
| micro                    | 9.4.1   | ✗      | 35149.8    | 27.96   | 6.27          |
| polka                    | 0.5.2   | ✓      | 34426.2    | 28.56   | 6.14          |
| spirit-router            | 0.5.0   | ✓      | 33994.4    | 29.02   | 6.06          |
| server-base              | 7.1.32  | ✗      | 33839.2    | 29.05   | 6.03          |
| spirit                   | 0.6.1   | ✗      | 32703.0    | 30.18   | 5.83          |
| micro-route              | 2.5.0   | ✓      | 32289.6    | 30.47   | 5.76          |
| yeps                     | 1.1.1   | ✗      | 32233.2    | 30.53   | 5.75          |
| connect-router           | 1.3.8   | ✓      | 31323.2    | 31.42   | 5.59          |
| trek-engine              | 1.0.5   | ✗      | 31028.4    | 31.73   | 5.09          |
| server-base-router       | 6.1.5   | ✓      | 30450.8    | 32.34   | 5.43          |
| restana                  | 4.9.7   | ✓      | 29911.2    | 32.93   | 5.33          |
| trek-router              | 1.2.0   | ✓      | 29684.8    | 33.19   | 4.87          |
| yeps-router              | 1.2.0   | ✓      | 27638.0    | 35.69   | 4.93          |
| restify                  | 8.6.1   | ✓      | 24205.6    | 40.80   | 4.36          |
| vapr                     | 0.5.5   | ✓      | 23778.8    | 41.54   | 3.90          |
| koa                      | 2.14.1  | ✗      | 23529.6    | 41.99   | 4.20          |
| total.js                 | 3.4.13  | ✓      | 22424.0    | 44.09   | 6.87          |
| koa-router               | 10.1.1  | ✓      | 21698.4    | 45.60   | 3.87          |
| hapi                     | 20.3.0  | ✓      | 19674.9    | 50.32   | 3.51          |
| microrouter              | 3.1.3   | ✓      | 19417.2    | 51.00   | 3.46          |
| express                  | 4.18.2  | ✓      | 8303.8     | 119.82  | 1.48          |
| fastify-big-json         | 3.29.5  | ✓      | 8176.4     | 121.66  | 94.06         |
| express-route-prefix     | 4.18.2  | ✓      | 7325.3     | 135.88  | 2.71          |
| express-with-middlewares | 4.18.2  | ✓      | 6774.1     | 146.95  | 2.60          |
| egg.js                   | 2.37.0  | ✓      | 5544.9     | 179.82  | 1.95          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
