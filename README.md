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
* __Machine:__ Linux fv-az238-210 5.8.0-1039-azure #42~20.04.1-Ubuntu SMP Thu Jul 15 14:11:07 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.3`
* __Run:__ Sun Aug  1 01:48:50 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.19.2  | ✓      | 71594.0    | 13.51   | 12.77         |
| polkadot                 | 1.0.0   | ✗      | 70080.0    | 13.79   | 12.50         |
| 0http                    | 3.1.1   | ✓      | 68707.2    | 14.08   | 12.25         |
| micro                    | 9.3.4   | ✗      | 67633.2    | 14.30   | 12.06         |
| polka                    | 0.5.2   | ✓      | 65724.0    | 14.72   | 11.72         |
| bare                     | 10.13.0 | ✗      | 63786.8    | 15.18   | 11.38         |
| connect                  | 3.7.0   | ✗      | 62483.2    | 15.51   | 11.14         |
| restana                  | 4.9.1   | ✓      | 62252.0    | 15.57   | 11.10         |
| foxify                   | 0.10.20 | ✓      | 61061.6    | 15.88   | 10.02         |
| rayo                     | 1.3.6   | ✓      | 60368.8    | 16.07   | 10.77         |
| server-base              | 7.1.27  | ✗      | 58747.2    | 16.53   | 10.48         |
| yeps                     | 1.1.1   | ✗      | 57217.6    | 16.98   | 10.20         |
| micro-route              | 2.5.0   | ✓      | 55124.8    | 17.64   | 9.83          |
| server-base-router       | 6.1.5   | ✓      | 54299.2    | 17.92   | 9.68          |
| connect-router           | 1.3.5   | ✓      | 54218.4    | 17.95   | 9.67          |
| trek-router              | 1.2.0   | ✓      | 51368.0    | 18.97   | 8.43          |
| trek-engine              | 1.0.5   | ✗      | 51285.6    | 19.01   | 8.41          |
| total.js                 | 3.4.9   | ✓      | 47761.6    | 20.44   | 14.62         |
| vapr                     | 0.5.5   | ✓      | 45225.0    | 21.62   | 7.42          |
| yeps-router              | 1.2.0   | ✓      | 44991.2    | 21.73   | 8.02          |
| koa                      | 2.13.1  | ✗      | 44631.2    | 21.91   | 7.96          |
| spirit                   | 0.6.1   | ✗      | 44104.0    | 22.18   | 7.87          |
| koa-router               | 10.0.0  | ✓      | 43392.8    | 22.54   | 7.74          |
| restify                  | 8.5.1   | ✓      | 39809.6    | 24.64   | 7.18          |
| spirit-router            | 0.5.0   | ✓      | 39531.2    | 24.81   | 7.05          |
| microrouter              | 3.1.3   | ✓      | 33313.6    | 29.52   | 5.94          |
| hapi                     | 20.1.5  | ✓      | 32868.0    | 29.92   | 5.86          |
| egg.js                   | 2.29.4  | ✓      | 20166.3    | 49.07   | 7.10          |
| express                  | 4.17.1  | ✓      | 13546.6    | 73.28   | 2.42          |
| express-with-middlewares | 4.17.1  | ✓      | 11617.4    | 85.53   | 4.45          |
| express-route-prefix     | 4.17.1  | ✓      | 10981.0    | 90.45   | 4.06          |
| fastify-big-json         | 3.19.2  | ✓      | 2771.9     | 358.98  | 31.88         |
| farrow-http              | 1.10.9  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
