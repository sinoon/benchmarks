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
* __Machine:__ Linux fv-az1538-207 6.2.0-1018-azure #18~22.04.1-Ubuntu SMP Tue Nov 21 19:25:02 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon Jan  1 01:06:22 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75662.0    | 12.73   | 13.49         |
| 0http                    | 3.5.2   | ✓      | 71383.6    | 13.52   | 12.73         |
| fastify                  | 3.29.5  | ✓      | 67808.4    | 14.25   | 12.09         |
| bare                     | 10.13.0 | ✗      | 67416.0    | 14.35   | 12.02         |
| polka                    | 0.5.2   | ✓      | 64633.2    | 14.97   | 11.53         |
| foxify                   | 0.10.20 | ✓      | 63257.6    | 15.31   | 10.38         |
| connect                  | 3.7.0   | ✗      | 62864.8    | 15.41   | 11.21         |
| restana                  | 4.9.7   | ✓      | 62290.4    | 15.56   | 11.11         |
| micro                    | 9.4.1   | ✗      | 61111.2    | 15.87   | 10.90         |
| server-base              | 7.1.32  | ✗      | 60131.2    | 16.13   | 10.72         |
| yeps                     | 1.1.1   | ✗      | 58881.6    | 16.49   | 10.50         |
| server-base-router       | 6.1.5   | ✓      | 56296.8    | 17.26   | 10.04         |
| connect-router           | 1.3.8   | ✓      | 55547.2    | 17.50   | 9.91          |
| trek-engine              | 1.0.5   | ✗      | 54416.8    | 17.88   | 8.93          |
| micro-route              | 2.5.0   | ✓      | 54274.4    | 17.93   | 9.68          |
| trek-router              | 1.2.0   | ✓      | 53584.0    | 18.17   | 8.79          |
| yeps-router              | 1.2.0   | ✓      | 47564.8    | 20.52   | 8.48          |
| vapr                     | 0.5.5   | ✓      | 47215.2    | 20.69   | 7.74          |
| spirit-router            | 0.5.0   | ✓      | 46408.0    | 21.01   | 8.28          |
| spirit                   | 0.6.1   | ✗      | 46118.4    | 21.17   | 8.22          |
| koa                      | 2.15.0  | ✗      | 45663.2    | 21.40   | 8.14          |
| total.js                 | 3.4.13  | ✓      | 42616.0    | 22.96   | 13.05         |
| restify                  | 8.6.1   | ✓      | 42604.0    | 22.97   | 7.68          |
| koa-router               | 10.1.1  | ✓      | 41809.4    | 23.43   | 7.46          |
| hapi                     | 20.3.0  | ✓      | 36547.0    | 26.86   | 6.52          |
| microrouter              | 3.1.3   | ✓      | 34376.8    | 28.58   | 6.13          |
| express                  | 4.18.2  | ✓      | 15124.2    | 65.58   | 2.70          |
| fastify-big-json         | 3.29.5  | ✓      | 13049.0    | 76.09   | 150.12        |
| express-with-middlewares | 4.18.2  | ✓      | 12682.8    | 78.30   | 4.86          |
| express-route-prefix     | 4.18.2  | ✓      | 11417.8    | 87.02   | 4.22          |
| egg.js                   | 2.37.0  | ✓      | 10522.8    | 94.46   | 3.70          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.5   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
