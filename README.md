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
* __Machine:__ Linux pkrvmccyg1gnepe 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon Sep  1 01:18:02 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74758.8    | 12.89   | 13.33         |
| fastify                  | 3.29.5  | ✓      | 68432.4    | 14.11   | 12.20         |
| bare                     | 10.13.0 | ✗      | 67099.6    | 14.41   | 11.97         |
| foxify                   | 0.10.20 | ✓      | 63803.2    | 15.18   | 10.47         |
| connect                  | 3.7.0   | ✗      | 62810.4    | 15.42   | 11.20         |
| polka                    | 0.5.2   | ✓      | 62552.0    | 15.48   | 11.16         |
| micro                    | 9.4.1   | ✗      | 62312.0    | 15.56   | 11.11         |
| server-base              | 7.1.32  | ✗      | 59751.2    | 16.23   | 10.66         |
| yeps                     | 1.1.1   | ✗      | 58605.6    | 16.57   | 10.45         |
| server-base-router       | 6.1.5   | ✓      | 56753.6    | 17.12   | 10.12         |
| connect-router           | 1.3.8   | ✓      | 56739.2    | 17.13   | 10.12         |
| trek-engine              | 1.0.5   | ✗      | 54700.8    | 17.78   | 8.97          |
| micro-route              | 2.5.0   | ✓      | 54593.6    | 17.82   | 9.74          |
| trek-router              | 1.2.0   | ✓      | 51780.8    | 18.81   | 8.49          |
| yeps-router              | 1.2.0   | ✓      | 47140.8    | 20.72   | 8.41          |
| spirit                   | 0.6.1   | ✗      | 46972.0    | 20.81   | 8.38          |
| vapr                     | 0.5.5   | ✓      | 46946.4    | 20.80   | 7.70          |
| koa                      | 2.16.2  | ✗      | 45356.8    | 21.55   | 8.09          |
| spirit-router            | 0.5.0   | ✓      | 43509.6    | 22.48   | 7.76          |
| total.js                 | 3.4.13  | ✓      | 42121.6    | 23.24   | 12.89         |
| restify                  | 8.6.1   | ✓      | 41732.8    | 23.46   | 7.52          |
| koa-router               | 10.1.1  | ✓      | 41068.8    | 23.85   | 7.32          |
| hapi                     | 20.3.0  | ✓      | 36449.4    | 26.93   | 6.50          |
| microrouter              | 3.1.3   | ✓      | 33555.8    | 29.31   | 5.98          |
| express                  | 4.21.2  | ✓      | 14320.6    | 69.30   | 2.55          |
| fastify-big-json         | 3.29.5  | ✓      | 13133.6    | 75.59   | 151.09        |
| express-with-middlewares | 4.21.2  | ✓      | 12251.2    | 81.08   | 4.70          |
| express-route-prefix     | 4.21.2  | ✓      | 11156.2    | 89.06   | 4.13          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
