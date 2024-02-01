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
* __Machine:__ Linux fv-az849-367 6.2.0-1019-azure #19~22.04.1-Ubuntu SMP Wed Jan 10 22:57:03 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu Feb  1 01:03:53 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74067.6    | 13.00   | 13.21         |
| 0http                    | 3.5.2   | ✓      | 69962.8    | 13.79   | 12.48         |
| fastify                  | 3.29.5  | ✓      | 66010.0    | 14.65   | 11.77         |
| bare                     | 10.13.0 | ✗      | 65844.0    | 14.69   | 11.74         |
| foxify                   | 0.10.20 | ✓      | 64588.4    | 14.98   | 10.59         |
| connect                  | 3.7.0   | ✗      | 63103.2    | 15.35   | 11.25         |
| polka                    | 0.5.2   | ✓      | 62793.6    | 15.42   | 11.20         |
| restana                  | 4.9.7   | ✓      | 61348.0    | 15.80   | 10.94         |
| micro                    | 9.4.1   | ✗      | 61100.8    | 15.87   | 10.90         |
| server-base              | 7.1.32  | ✗      | 59481.6    | 16.31   | 10.61         |
| yeps                     | 1.1.1   | ✗      | 58143.2    | 16.70   | 10.37         |
| connect-router           | 1.3.8   | ✓      | 55396.8    | 17.55   | 9.88          |
| micro-route              | 2.5.0   | ✓      | 54986.4    | 17.69   | 9.81          |
| server-base-router       | 6.1.5   | ✓      | 54446.4    | 17.87   | 9.71          |
| trek-engine              | 1.0.5   | ✗      | 54093.6    | 17.99   | 8.87          |
| trek-router              | 1.2.0   | ✓      | 52974.4    | 18.38   | 8.69          |
| yeps-router              | 1.2.0   | ✓      | 47285.6    | 20.65   | 8.43          |
| spirit                   | 0.6.1   | ✗      | 46715.2    | 20.86   | 8.33          |
| vapr                     | 0.5.5   | ✓      | 45964.0    | 21.25   | 7.54          |
| koa                      | 2.15.0  | ✗      | 45674.4    | 21.40   | 8.15          |
| total.js                 | 3.4.13  | ✓      | 42385.6    | 23.10   | 12.97         |
| restify                  | 8.6.1   | ✓      | 42205.6    | 23.19   | 7.61          |
| koa-router               | 10.1.1  | ✓      | 41936.0    | 23.35   | 7.48          |
| spirit-router            | 0.5.0   | ✓      | 37204.8    | 26.38   | 6.63          |
| hapi                     | 20.3.0  | ✓      | 35639.4    | 27.56   | 6.36          |
| microrouter              | 3.1.3   | ✓      | 33737.6    | 29.14   | 6.02          |
| express                  | 4.18.2  | ✓      | 14853.8    | 66.79   | 2.65          |
| fastify-big-json         | 3.29.5  | ✓      | 13417.2    | 73.98   | 154.35        |
| express-with-middlewares | 4.18.2  | ✓      | 12547.6    | 79.16   | 4.81          |
| express-route-prefix     | 4.18.2  | ✓      | 11290.2    | 88.01   | 4.18          |
| egg.js                   | 2.37.0  | ✓      | 10659.0    | 93.21   | 3.75          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
