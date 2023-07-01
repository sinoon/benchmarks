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
* __Machine:__ Linux fv-az559-169 5.15.0-1040-azure #47-Ubuntu SMP Thu Jun 1 19:38:24 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Jul  1 02:35:58 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 38960.6    | 25.20   | 6.95          |
| bare                     | 10.13.0 | ✗      | 37660.2    | 26.07   | 6.72          |
| fastify                  | 3.29.5  | ✓      | 37441.0    | 26.22   | 6.68          |
| connect                  | 3.7.0   | ✗      | 36473.0    | 26.92   | 6.50          |
| polka                    | 0.5.2   | ✓      | 35993.0    | 27.28   | 6.42          |
| yeps                     | 1.1.1   | ✗      | 34960.6    | 28.12   | 6.23          |
| foxify                   | 0.10.20 | ✓      | 34626.6    | 28.39   | 5.68          |
| server-base              | 7.1.32  | ✗      | 34596.8    | 28.41   | 6.17          |
| micro                    | 9.4.1   | ✗      | 34461.0    | 28.52   | 6.15          |
| 0http                    | 3.5.2   | ✓      | 33965.0    | 28.95   | 6.06          |
| restana                  | 4.9.7   | ✓      | 32962.6    | 29.83   | 5.88          |
| spirit-router            | 0.5.0   | ✓      | 32517.4    | 30.34   | 5.80          |
| spirit                   | 0.6.1   | ✗      | 31531.0    | 31.26   | 5.62          |
| connect-router           | 1.3.8   | ✓      | 31403.2    | 31.35   | 5.60          |
| micro-route              | 2.5.0   | ✓      | 30132.4    | 32.68   | 5.37          |
| trek-engine              | 1.0.5   | ✗      | 29512.4    | 33.39   | 4.84          |
| server-base-router       | 6.1.5   | ✓      | 29044.4    | 33.92   | 5.18          |
| trek-router              | 1.2.0   | ✓      | 27434.0    | 35.94   | 4.50          |
| yeps-router              | 1.2.0   | ✓      | 27378.4    | 36.03   | 4.88          |
| vapr                     | 0.5.5   | ✓      | 26758.0    | 36.86   | 4.39          |
| restify                  | 8.6.1   | ✓      | 25552.0    | 38.63   | 4.61          |
| koa                      | 2.14.2  | ✗      | 23788.0    | 41.55   | 4.24          |
| total.js                 | 3.4.13  | ✓      | 22838.4    | 43.28   | 6.99          |
| koa-router               | 10.1.1  | ✓      | 21800.0    | 45.36   | 3.89          |
| hapi                     | 20.3.0  | ✓      | 19780.4    | 50.03   | 3.53          |
| microrouter              | 3.1.3   | ✓      | 19356.0    | 51.15   | 3.45          |
| express                  | 4.18.2  | ✓      | 8454.9     | 117.67  | 1.51          |
| express-route-prefix     | 4.18.2  | ✓      | 7453.4     | 133.52  | 2.76          |
| fastify-big-json         | 3.29.5  | ✓      | 7191.4     | 138.38  | 82.73         |
| express-with-middlewares | 4.18.2  | ✓      | 7052.2     | 141.00  | 2.70          |
| egg.js                   | 2.37.0  | ✓      | 5493.8     | 181.40  | 1.93          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
