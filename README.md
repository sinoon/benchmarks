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
* __Machine:__ Linux fv-az246-793 5.11.0-1022-azure #23~20.04.1-Ubuntu SMP Fri Nov 19 10:20:52 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.8`
* __Run:__ Sat Jan  1 01:50:49 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| bare                     | 10.13.0 | ✗      | 69683.6    | 13.88   | 12.43         |
| fastify                  | 3.25.3  | ✓      | 69342.8    | 13.93   | 12.37         |
| 0http                    | 3.1.1   | ✓      | 68257.6    | 14.17   | 12.17         |
| polkadot                 | 1.0.0   | ✗      | 67496.8    | 14.34   | 12.04         |
| rayo                     | 1.3.10  | ✓      | 62438.8    | 15.53   | 11.14         |
| foxify                   | 0.10.20 | ✓      | 60779.2    | 15.95   | 9.97          |
| server-base              | 7.1.29  | ✗      | 59089.6    | 16.43   | 10.54         |
| polka                    | 0.5.2   | ✓      | 57527.2    | 16.89   | 10.26         |
| connect                  | 3.7.0   | ✗      | 57181.6    | 16.99   | 10.20         |
| connect-router           | 1.3.6   | ✓      | 57180.8    | 16.99   | 10.20         |
| restana                  | 4.9.2   | ✓      | 57068.8    | 17.03   | 10.18         |
| server-base-router       | 6.1.5   | ✓      | 54540.0    | 17.84   | 9.73          |
| micro                    | 9.3.4   | ✗      | 54304.0    | 17.92   | 9.68          |
| yeps                     | 1.1.1   | ✗      | 52891.2    | 18.41   | 9.43          |
| micro-route              | 2.5.0   | ✓      | 50563.2    | 19.28   | 9.02          |
| trek-router              | 1.2.0   | ✓      | 48443.2    | 20.15   | 7.95          |
| trek-engine              | 1.0.5   | ✗      | 47696.6    | 20.47   | 7.82          |
| koa                      | 2.13.4  | ✗      | 43147.4    | 22.68   | 7.69          |
| yeps-router              | 1.2.0   | ✓      | 42926.4    | 22.80   | 7.66          |
| vapr                     | 0.5.5   | ✓      | 42256.8    | 23.17   | 6.93          |
| restify                  | 8.6.0   | ✓      | 39643.2    | 24.72   | 7.15          |
| spirit                   | 0.6.1   | ✗      | 38498.4    | 25.48   | 6.87          |
| total.js                 | 3.4.13  | ✓      | 38480.8    | 25.49   | 11.78         |
| koa-router               | 10.1.1  | ✓      | 37006.6    | 26.52   | 6.60          |
| spirit-router            | 0.5.0   | ✓      | 35691.4    | 27.52   | 6.37          |
| hapi                     | 20.2.1  | ✓      | 31431.2    | 31.31   | 5.61          |
| microrouter              | 3.1.3   | ✓      | 29896.8    | 32.95   | 5.33          |
| egg.js                   | 2.33.1  | ✓      | 18940.5    | 52.30   | 6.66          |
| express                  | 4.17.2  | ✓      | 13574.2    | 73.12   | 2.42          |
| express-with-middlewares | 4.17.2  | ✓      | 11136.0    | 89.25   | 4.27          |
| express-route-prefix     | 4.17.2  | ✓      | 10752.4    | 92.42   | 3.98          |
| fastify-big-json         | 3.25.3  | ✓      | 10492.6    | 94.72   | 120.71        |
| farrow-http              | 1.11.2  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
