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
* __Machine:__ Linux fv-az617-826 6.2.0-1012-azure #12~22.04.1-Ubuntu SMP Thu Sep  7 14:07:14 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Oct  1 01:05:37 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.29.5  | ✓      | 56344.8    | 17.26   | 10.05         |
| polkadot                 | 1.0.0   | ✗      | 55831.2    | 17.43   | 9.96          |
| foxify                   | 0.10.20 | ✓      | 55113.6    | 17.66   | 9.04          |
| bare                     | 10.13.0 | ✗      | 52846.4    | 18.43   | 9.42          |
| polka                    | 0.5.2   | ✓      | 52203.2    | 18.67   | 9.31          |
| connect                  | 3.7.0   | ✗      | 51898.4    | 18.77   | 9.25          |
| micro                    | 9.4.1   | ✗      | 51798.4    | 18.81   | 9.24          |
| 0http                    | 3.5.2   | ✓      | 51463.2    | 18.94   | 9.18          |
| server-base              | 7.1.32  | ✗      | 49359.2    | 19.76   | 8.80          |
| yeps                     | 1.1.1   | ✗      | 48614.4    | 20.08   | 8.67          |
| connect-router           | 1.3.8   | ✓      | 47247.2    | 20.67   | 8.43          |
| micro-route              | 2.5.0   | ✓      | 47157.6    | 20.71   | 8.41          |
| server-base-router       | 6.1.5   | ✓      | 47037.6    | 20.76   | 8.39          |
| restana                  | 4.9.7   | ✓      | 46892.0    | 20.83   | 8.36          |
| trek-engine              | 1.0.5   | ✗      | 44297.8    | 22.08   | 7.27          |
| trek-router              | 1.2.0   | ✓      | 42884.2    | 22.82   | 7.03          |
| koa                      | 2.14.2  | ✗      | 40657.2    | 24.10   | 7.25          |
| yeps-router              | 1.2.0   | ✓      | 40525.6    | 24.18   | 7.23          |
| vapr                     | 0.5.5   | ✓      | 39677.6    | 24.70   | 6.51          |
| spirit                   | 0.6.1   | ✗      | 37162.6    | 26.45   | 6.63          |
| spirit-router            | 0.5.0   | ✓      | 36236.4    | 27.12   | 6.46          |
| koa-router               | 10.1.1  | ✓      | 35945.4    | 27.33   | 6.41          |
| total.js                 | 3.4.13  | ✓      | 35186.8    | 27.92   | 10.77         |
| restify                  | 8.6.1   | ✓      | 34126.0    | 28.80   | 6.15          |
| hapi                     | 20.3.0  | ✓      | 28562.4    | 34.50   | 5.09          |
| microrouter              | 3.1.3   | ✓      | 28160.0    | 35.01   | 5.02          |
| express                  | 4.18.2  | ✓      | 11000.5    | 90.32   | 1.96          |
| express-with-middlewares | 4.18.2  | ✓      | 9315.5     | 106.76  | 3.57          |
| fastify-big-json         | 3.29.5  | ✓      | 8652.5     | 114.96  | 99.54         |
| express-route-prefix     | 4.18.2  | ✓      | 8356.3     | 119.07  | 3.09          |
| egg.js                   | 2.37.0  | ✓      | 6492.1     | 153.34  | 2.28          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
