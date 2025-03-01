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
* __Machine:__ Linux fv-az1719-529 6.8.0-1021-azure #25-Ubuntu SMP Wed Jan 15 20:45:09 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Mar  1 01:12:25 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 77326.4    | 12.42   | 13.79         |
| fastify                  | 3.29.5  | ✓      | 66031.6    | 14.65   | 11.77         |
| polka                    | 0.5.2   | ✓      | 64984.4    | 14.89   | 11.59         |
| bare                     | 10.13.0 | ✗      | 64462.8    | 15.01   | 11.50         |
| foxify                   | 0.10.20 | ✓      | 63430.0    | 15.27   | 10.40         |
| connect                  | 3.7.0   | ✗      | 62699.2    | 15.46   | 11.18         |
| micro                    | 9.4.1   | ✗      | 60362.4    | 16.07   | 10.76         |
| server-base              | 7.1.32  | ✗      | 59997.6    | 16.17   | 10.70         |
| yeps                     | 1.1.1   | ✗      | 58199.2    | 16.69   | 10.38         |
| server-base-router       | 6.1.5   | ✓      | 56092.0    | 17.33   | 10.00         |
| connect-router           | 1.3.8   | ✓      | 55004.8    | 17.69   | 9.81          |
| micro-route              | 2.5.0   | ✓      | 54819.2    | 17.75   | 9.78          |
| trek-engine              | 1.0.5   | ✗      | 51621.6    | 18.87   | 8.47          |
| trek-router              | 1.2.0   | ✓      | 50665.6    | 19.24   | 8.31          |
| yeps-router              | 1.2.0   | ✓      | 46891.2    | 20.83   | 8.36          |
| spirit                   | 0.6.1   | ✗      | 46752.8    | 20.86   | 8.34          |
| vapr                     | 0.5.5   | ✓      | 46529.6    | 21.00   | 7.63          |
| spirit-router            | 0.5.0   | ✓      | 45841.6    | 21.30   | 8.18          |
| koa                      | 2.16.0  | ✗      | 45788.0    | 21.34   | 8.17          |
| restify                  | 8.6.1   | ✓      | 41856.8    | 23.39   | 7.54          |
| koa-router               | 10.1.1  | ✓      | 41751.2    | 23.45   | 7.45          |
| total.js                 | 3.4.13  | ✓      | 41288.0    | 23.72   | 12.64         |
| hapi                     | 20.3.0  | ✓      | 35869.0    | 27.38   | 6.40          |
| microrouter              | 3.1.3   | ✓      | 33936.6    | 28.96   | 6.05          |
| express                  | 4.21.2  | ✓      | 14787.0    | 67.10   | 2.64          |
| fastify-big-json         | 3.29.5  | ✓      | 12726.8    | 78.02   | 146.40        |
| express-with-middlewares | 4.21.2  | ✓      | 12403.0    | 80.08   | 4.75          |
| express-route-prefix     | 4.21.2  | ✓      | 11305.0    | 87.90   | 4.18          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
