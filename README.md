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
* __Machine:__ Linux fv-az1426-913 6.5.0-1016-azure #16~22.04.1-Ubuntu SMP Fri Feb 16 15:42:02 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon Apr  1 01:05:57 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 73994.8    | 13.02   | 13.20         |
| 0http                    | 3.5.2   | ✓      | 68740.0    | 14.06   | 12.26         |
| fastify                  | 3.29.5  | ✓      | 67787.2    | 14.25   | 12.09         |
| bare                     | 10.13.0 | ✗      | 66050.4    | 14.65   | 11.78         |
| foxify                   | 0.10.20 | ✓      | 63736.4    | 15.19   | 10.45         |
| polka                    | 0.5.2   | ✓      | 63398.8    | 15.27   | 11.31         |
| restana                  | 4.9.7   | ✓      | 62565.6    | 15.49   | 11.16         |
| connect                  | 3.7.0   | ✗      | 62021.2    | 15.63   | 11.06         |
| micro                    | 9.4.1   | ✗      | 61144.0    | 15.86   | 10.90         |
| server-base              | 7.1.32  | ✗      | 59159.2    | 16.40   | 10.55         |
| yeps                     | 1.1.1   | ✗      | 58557.6    | 16.58   | 10.44         |
| connect-router           | 1.3.8   | ✓      | 56663.2    | 17.15   | 10.11         |
| server-base-router       | 6.1.5   | ✓      | 55661.6    | 17.47   | 9.93          |
| trek-engine              | 1.0.5   | ✗      | 55571.2    | 17.50   | 9.12          |
| micro-route              | 2.5.0   | ✓      | 54646.4    | 17.80   | 9.75          |
| trek-router              | 1.2.0   | ✓      | 51616.8    | 18.88   | 8.47          |
| spirit                   | 0.6.1   | ✗      | 47272.0    | 20.67   | 8.43          |
| yeps-router              | 1.2.0   | ✓      | 47233.6    | 20.67   | 8.42          |
| vapr                     | 0.5.5   | ✓      | 46487.2    | 21.01   | 7.63          |
| spirit-router            | 0.5.0   | ✓      | 44880.8    | 21.78   | 8.00          |
| koa                      | 2.15.2  | ✗      | 44443.2    | 22.00   | 7.93          |
| restify                  | 8.6.1   | ✓      | 42052.8    | 23.28   | 7.58          |
| total.js                 | 3.4.13  | ✓      | 41998.4    | 23.31   | 12.86         |
| koa-router               | 10.1.1  | ✓      | 40611.0    | 24.12   | 7.24          |
| hapi                     | 20.3.0  | ✓      | 36387.0    | 26.98   | 6.49          |
| microrouter              | 3.1.3   | ✓      | 33578.2    | 29.28   | 5.99          |
| express                  | 4.19.2  | ✓      | 14897.6    | 66.58   | 2.66          |
| fastify-big-json         | 3.29.5  | ✓      | 13206.6    | 75.17   | 151.93        |
| express-with-middlewares | 4.19.2  | ✓      | 12358.6    | 80.37   | 4.74          |
| express-route-prefix     | 4.19.2  | ✓      | 11285.0    | 88.03   | 4.18          |
| egg.js                   | 2.37.0  | ✓      | 10521.4    | 94.48   | 3.70          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
