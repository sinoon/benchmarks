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
* __Machine:__ Linux fv-az21-132 5.4.0-1032-azure #33~18.04.1-Ubuntu SMP Tue Nov 17 11:40:52 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.20.0`
* __Run:__ Fri Jan  1 01:49:15 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 42622.4    | 22.99   | 7.60          |
| micro                    | 9.3.4   | ✗      | 40207.2    | 24.38   | 7.17          |
| bare                     | 10.13.0 | ✗      | 39807.4    | 24.64   | 7.10          |
| fastify                  | 3.9.2   | ✓      | 39791.2    | 24.65   | 7.10          |
| foxify                   | 0.10.20 | ✓      | 39576.0    | 24.78   | 6.49          |
| 0http                    | 3.0.0   | ✓      | 39517.4    | 24.84   | 7.05          |
| polka                    | 0.5.2   | ✓      | 39155.2    | 25.04   | 6.98          |
| rayo                     | 1.3.6   | ✓      | 38013.6    | 25.80   | 6.78          |
| server-base              | 7.1.23  | ✗      | 36348.6    | 27.01   | 6.48          |
| connect                  | 3.7.0   | ✗      | 35060.6    | 28.03   | 6.25          |
| restana                  | 4.8.1   | ✓      | 34182.4    | 28.75   | 6.10          |
| spirit-router            | 0.5.0   | ✓      | 34166.2    | 28.81   | 6.09          |
| server-base-router       | 6.1.5   | ✓      | 33845.6    | 29.04   | 6.04          |
| spirit                   | 0.6.1   | ✗      | 33567.6    | 29.33   | 5.99          |
| connect-router           | 1.3.5   | ✓      | 33321.8    | 29.52   | 5.94          |
| yeps                     | 1.1.1   | ✗      | 33057.6    | 29.75   | 5.90          |
| micro-route              | 2.5.0   | ✓      | 32274.2    | 30.48   | 5.76          |
| trek-router              | 1.2.0   | ✓      | 32128.0    | 30.62   | 5.27          |
| trek-engine              | 1.0.5   | ✗      | 31906.6    | 30.86   | 5.23          |
| yeps-router              | 1.2.0   | ✓      | 30434.8    | 32.36   | 5.43          |
| koa                      | 2.13.0  | ✗      | 28573.2    | 34.52   | 5.10          |
| restify                  | 8.5.1   | ✓      | 27054.4    | 36.46   | 4.88          |
| vapr                     | 0.5.5   | ✓      | 26594.8    | 37.09   | 4.36          |
| koa-router               | 10.0.0  | ✓      | 23658.1    | 41.75   | 4.22          |
| total.js                 | 3.4.6   | ✓      | 23530.0    | 41.99   | 7.20          |
| hapi                     | 20.0.3  | ✓      | 20832.4    | 47.49   | 3.72          |
| microrouter              | 3.1.3   | ✓      | 18970.1    | 52.19   | 3.38          |
| egg.js                   | 2.29.1  | ✓      | 13935.8    | 71.22   | 4.90          |
| express                  | 4.17.1  | ✓      | 8585.4     | 115.89  | 1.53          |
| fastify-big-json         | 3.9.2   | ✓      | 7875.9     | 126.36  | 90.60         |
| express-with-middlewares | 4.17.1  | ✓      | 7369.7     | 135.03  | 2.83          |
| express-route-prefix     | 4.17.1  | ✓      | 7029.1     | 141.51  | 2.60          |
| farrow-http              | 1.3.4   | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
