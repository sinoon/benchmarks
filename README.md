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
* __Machine:__ Linux fv-az659-754 6.2.0-1016-azure #16~22.04.1-Ubuntu SMP Tue Oct 10 17:11:51 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri Dec  1 01:05:55 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75371.2    | 12.78   | 13.44         |
| 0http                    | 3.5.2   | ✓      | 68217.2    | 14.16   | 12.17         |
| fastify                  | 3.29.5  | ✓      | 66451.6    | 14.55   | 11.85         |
| bare                     | 10.13.0 | ✗      | 64319.6    | 15.05   | 11.47         |
| foxify                   | 0.10.20 | ✓      | 63219.2    | 15.32   | 10.37         |
| polka                    | 0.5.2   | ✓      | 62504.0    | 15.50   | 11.15         |
| micro                    | 9.4.1   | ✗      | 61920.8    | 15.65   | 11.04         |
| restana                  | 4.9.7   | ✓      | 61472.0    | 15.76   | 10.96         |
| server-base              | 7.1.32  | ✗      | 61028.8    | 15.89   | 10.88         |
| connect                  | 3.7.0   | ✗      | 59973.6    | 16.19   | 10.70         |
| yeps                     | 1.1.1   | ✗      | 58214.4    | 16.68   | 10.38         |
| server-base-router       | 6.1.5   | ✓      | 57137.6    | 17.01   | 10.19         |
| trek-engine              | 1.0.5   | ✗      | 55104.8    | 17.65   | 9.04          |
| micro-route              | 2.5.0   | ✓      | 54416.8    | 17.88   | 9.70          |
| connect-router           | 1.3.8   | ✓      | 54014.4    | 18.02   | 9.63          |
| trek-router              | 1.2.0   | ✓      | 53176.8    | 18.31   | 8.72          |
| yeps-router              | 1.2.0   | ✓      | 47740.8    | 20.45   | 8.51          |
| vapr                     | 0.5.5   | ✓      | 46533.6    | 20.99   | 7.63          |
| koa                      | 2.14.2  | ✗      | 45649.6    | 21.41   | 8.14          |
| spirit                   | 0.6.1   | ✗      | 42755.2    | 22.90   | 7.62          |
| restify                  | 8.6.1   | ✓      | 42568.0    | 23.00   | 7.67          |
| total.js                 | 3.4.13  | ✓      | 42541.6    | 23.00   | 13.02         |
| spirit-router            | 0.5.0   | ✓      | 41360.8    | 23.68   | 7.38          |
| koa-router               | 10.1.1  | ✓      | 41044.6    | 23.86   | 7.32          |
| hapi                     | 20.3.0  | ✓      | 35697.0    | 27.51   | 6.37          |
| microrouter              | 3.1.3   | ✓      | 34149.2    | 28.77   | 6.09          |
| express                  | 4.18.2  | ✓      | 15127.6    | 65.57   | 2.70          |
| fastify-big-json         | 3.29.5  | ✓      | 13486.4    | 73.60   | 155.15        |
| express-with-middlewares | 4.18.2  | ✓      | 12643.6    | 78.55   | 4.85          |
| express-route-prefix     | 4.18.2  | ✓      | 11347.8    | 87.54   | 4.20          |
| egg.js                   | 2.37.0  | ✓      | 10425.8    | 95.35   | 3.67          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.5   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
