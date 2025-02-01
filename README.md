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
* __Machine:__ Linux fv-az1945-329 6.8.0-1020-azure #23-Ubuntu SMP Mon Dec  9 16:58:58 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Feb  1 01:10:56 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74630.4    | 12.91   | 13.31         |
| fastify                  | 3.29.5  | ✓      | 70191.6    | 13.75   | 12.52         |
| foxify                   | 0.10.20 | ✓      | 66192.4    | 14.62   | 10.86         |
| polka                    | 0.5.2   | ✓      | 65631.2    | 14.74   | 11.71         |
| bare                     | 10.13.0 | ✗      | 65612.0    | 14.75   | 11.70         |
| connect                  | 3.7.0   | ✗      | 62789.6    | 15.43   | 11.20         |
| micro                    | 9.4.1   | ✗      | 61843.2    | 15.67   | 11.03         |
| server-base              | 7.1.32  | ✗      | 61236.8    | 15.83   | 10.92         |
| yeps                     | 1.1.1   | ✗      | 58892.8    | 16.48   | 10.50         |
| server-base-router       | 6.1.5   | ✓      | 56738.4    | 17.13   | 10.12         |
| connect-router           | 1.3.8   | ✓      | 56712.0    | 17.14   | 10.11         |
| micro-route              | 2.5.0   | ✓      | 56694.4    | 17.14   | 10.11         |
| trek-engine              | 1.0.5   | ✗      | 54610.4    | 17.82   | 8.96          |
| trek-router              | 1.2.0   | ✓      | 53062.4    | 18.35   | 8.70          |
| vapr                     | 0.5.5   | ✓      | 46400.8    | 21.05   | 7.61          |
| yeps-router              | 1.2.0   | ✓      | 46251.2    | 21.12   | 8.25          |
| koa                      | 2.15.3  | ✗      | 46114.4    | 21.19   | 8.22          |
| spirit                   | 0.6.1   | ✗      | 43904.8    | 22.29   | 7.83          |
| spirit-router            | 0.5.0   | ✓      | 43328.8    | 22.65   | 7.73          |
| restify                  | 8.6.1   | ✓      | 42622.4    | 22.96   | 7.68          |
| total.js                 | 3.4.13  | ✓      | 42009.6    | 23.30   | 12.86         |
| koa-router               | 10.1.1  | ✓      | 41766.4    | 23.45   | 7.45          |
| hapi                     | 20.3.0  | ✓      | 36320.8    | 27.03   | 6.48          |
| microrouter              | 3.1.3   | ✓      | 34282.2    | 28.66   | 6.11          |
| express                  | 4.21.2  | ✓      | 14481.2    | 68.52   | 2.58          |
| fastify-big-json         | 3.29.5  | ✓      | 12979.8    | 76.48   | 149.32        |
| express-with-middlewares | 4.21.2  | ✓      | 12169.2    | 81.62   | 4.66          |
| express-route-prefix     | 4.21.2  | ✓      | 11103.6    | 89.49   | 4.11          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
