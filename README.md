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
* __Machine:__ Linux fv-az802-93 6.5.0-1025-azure #26~22.04.1-Ubuntu SMP Thu Jul 11 22:33:04 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Jan  1 01:11:56 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 76716.8    | 12.54   | 13.68         |
| fastify                  | 3.29.5  | ✓      | 67990.8    | 14.22   | 12.12         |
| bare                     | 10.13.0 | ✗      | 67725.6    | 14.27   | 12.08         |
| foxify                   | 0.10.20 | ✓      | 65242.8    | 14.83   | 10.70         |
| connect                  | 3.7.0   | ✗      | 64537.2    | 14.99   | 11.51         |
| polka                    | 0.5.2   | ✓      | 63764.0    | 15.18   | 11.37         |
| server-base              | 7.1.32  | ✗      | 61526.4    | 15.76   | 10.97         |
| micro                    | 9.4.1   | ✗      | 60756.0    | 15.96   | 10.83         |
| yeps                     | 1.1.1   | ✗      | 58943.2    | 16.46   | 10.51         |
| micro-route              | 2.5.0   | ✓      | 56641.6    | 17.15   | 10.10         |
| server-base-router       | 6.1.5   | ✓      | 56613.6    | 17.16   | 10.10         |
| connect-router           | 1.3.8   | ✓      | 56089.6    | 17.33   | 10.00         |
| trek-engine              | 1.0.5   | ✗      | 54665.6    | 17.80   | 8.97          |
| trek-router              | 1.2.0   | ✓      | 54190.4    | 17.95   | 8.89          |
| yeps-router              | 1.2.0   | ✓      | 48717.6    | 20.02   | 8.69          |
| vapr                     | 0.5.5   | ✓      | 47387.2    | 20.61   | 7.77          |
| koa                      | 2.15.3  | ✗      | 46914.4    | 20.82   | 8.37          |
| spirit                   | 0.6.1   | ✗      | 46620.0    | 20.94   | 8.31          |
| spirit-router            | 0.5.0   | ✓      | 46054.4    | 21.18   | 8.21          |
| total.js                 | 3.4.13  | ✓      | 43263.2    | 22.62   | 13.24         |
| restify                  | 8.6.1   | ✓      | 42384.0    | 23.10   | 7.64          |
| koa-router               | 10.1.1  | ✓      | 41489.6    | 23.61   | 7.40          |
| hapi                     | 20.3.0  | ✓      | 36263.2    | 27.07   | 6.47          |
| microrouter              | 3.1.3   | ✓      | 33538.8    | 29.31   | 5.98          |
| express                  | 4.21.2  | ✓      | 14806.8    | 66.99   | 2.64          |
| fastify-big-json         | 3.29.5  | ✓      | 13445.2    | 73.83   | 154.69        |
| express-with-middlewares | 4.21.2  | ✓      | 12631.4    | 78.60   | 4.84          |
| express-route-prefix     | 4.21.2  | ✓      | 11364.0    | 87.43   | 4.20          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
