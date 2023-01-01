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
* __Machine:__ Linux fv-az351-823 5.15.0-1024-azure #30-Ubuntu SMP Wed Nov 16 23:37:59 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Jan  1 01:06:03 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 65252.4    | 14.84   | 11.64         |
| bare                     | 10.13.0 | ✗      | 63999.2    | 15.15   | 11.41         |
| fastify                  | 3.29.4  | ✓      | 63991.2    | 15.16   | 11.41         |
| connect                  | 3.7.0   | ✗      | 62482.4    | 15.52   | 11.14         |
| foxify                   | 0.10.20 | ✓      | 62196.0    | 15.58   | 10.20         |
| 0http                    | 3.4.2   | ✓      | 61907.2    | 15.65   | 11.04         |
| polka                    | 0.5.2   | ✓      | 60699.2    | 15.97   | 10.82         |
| micro                    | 9.4.1   | ✗      | 59068.8    | 16.44   | 10.53         |
| server-base              | 7.1.32  | ✗      | 58988.0    | 16.47   | 10.52         |
| yeps                     | 1.1.1   | ✗      | 58184.8    | 16.69   | 10.38         |
| restana                  | 4.9.7   | ✓      | 56612.0    | 17.18   | 10.10         |
| micro-route              | 2.5.0   | ✓      | 55183.2    | 17.63   | 9.84          |
| connect-router           | 1.3.7   | ✓      | 54741.6    | 17.77   | 9.76          |
| trek-engine              | 1.0.5   | ✗      | 51808.0    | 18.80   | 8.50          |
| server-base-router       | 6.1.5   | ✓      | 51789.6    | 18.81   | 9.24          |
| trek-router              | 1.2.0   | ✓      | 51681.6    | 18.85   | 8.48          |
| yeps-router              | 1.2.0   | ✓      | 47769.6    | 20.44   | 8.52          |
| vapr                     | 0.5.5   | ✓      | 45055.2    | 21.69   | 7.39          |
| koa                      | 2.14.1  | ✗      | 44352.0    | 22.06   | 7.91          |
| spirit                   | 0.6.1   | ✗      | 42572.0    | 23.01   | 7.59          |
| spirit-router            | 0.5.0   | ✓      | 42276.8    | 23.17   | 7.54          |
| total.js                 | 3.4.13  | ✓      | 41253.6    | 23.74   | 12.63         |
| restify                  | 8.6.1   | ✓      | 40515.2    | 24.18   | 7.30          |
| koa-router               | 10.1.1  | ✓      | 39824.0    | 24.61   | 7.10          |
| hapi                     | 20.2.2  | ✓      | 33324.2    | 29.51   | 5.94          |
| microrouter              | 3.1.3   | ✓      | 31728.4    | 31.02   | 5.66          |
| express                  | 4.18.2  | ✓      | 13082.2    | 75.90   | 2.33          |
| express-with-middlewares | 4.18.2  | ✓      | 11364.6    | 87.45   | 4.36          |
| express-route-prefix     | 4.18.2  | ✓      | 11177.4    | 88.92   | 4.14          |
| fastify-big-json         | 3.29.4  | ✓      | 10372.8    | 95.85   | 119.33        |
| egg.js                   | 2.37.0  | ✓      | 7602.1     | 130.92  | 2.68          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
