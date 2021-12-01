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
* __Machine:__ Linux fv-az163-734 5.11.0-1021-azure #22~20.04.1-Ubuntu SMP Fri Oct 29 01:11:25 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.7`
* __Run:__ Wed Dec  1 01:48:23 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.24.1  | ✓      | 59324.0    | 16.38   | 10.58         |
| polkadot                 | 1.0.0   | ✗      | 58776.0    | 16.53   | 10.48         |
| foxify                   | 0.10.20 | ✓      | 58423.2    | 16.63   | 9.58          |
| 0http                    | 3.1.1   | ✓      | 57037.6    | 17.04   | 10.17         |
| bare                     | 10.13.0 | ✗      | 56638.4    | 17.16   | 10.10         |
| polka                    | 0.5.2   | ✓      | 56515.2    | 17.20   | 10.08         |
| connect                  | 3.7.0   | ✗      | 54690.4    | 17.79   | 9.75          |
| rayo                     | 1.3.6   | ✓      | 54116.0    | 17.99   | 9.65          |
| micro                    | 9.3.4   | ✗      | 54028.0    | 18.01   | 9.64          |
| server-base              | 7.1.29  | ✗      | 53783.2    | 18.10   | 9.59          |
| connect-router           | 1.3.6   | ✓      | 50726.4    | 19.22   | 9.05          |
| restana                  | 4.9.2   | ✓      | 50687.8    | 19.23   | 9.04          |
| yeps                     | 1.1.1   | ✗      | 49516.8    | 19.70   | 8.83          |
| micro-route              | 2.5.0   | ✓      | 49067.2    | 19.89   | 8.75          |
| server-base-router       | 6.1.5   | ✓      | 48524.0    | 20.11   | 8.65          |
| trek-router              | 1.2.0   | ✓      | 46590.6    | 20.97   | 7.64          |
| trek-engine              | 1.0.5   | ✗      | 46137.0    | 21.18   | 7.57          |
| yeps-router              | 1.2.0   | ✓      | 41838.4    | 23.40   | 7.46          |
| koa                      | 2.13.4  | ✗      | 40833.4    | 23.99   | 7.28          |
| vapr                     | 0.5.5   | ✓      | 40564.8    | 24.15   | 6.65          |
| spirit                   | 0.6.1   | ✗      | 37920.0    | 25.88   | 6.76          |
| total.js                 | 3.4.13  | ✓      | 37803.4    | 25.95   | 11.57         |
| spirit-router            | 0.5.0   | ✓      | 36010.4    | 27.27   | 6.42          |
| koa-router               | 10.1.1  | ✓      | 35459.0    | 27.70   | 6.32          |
| restify                  | 8.6.0   | ✓      | 34999.4    | 28.07   | 6.31          |
| hapi                     | 20.2.1  | ✓      | 29152.0    | 33.80   | 5.20          |
| microrouter              | 3.1.3   | ✓      | 27318.4    | 36.11   | 4.87          |
| egg.js                   | 2.32.0  | ✓      | 18790.2    | 52.71   | 6.61          |
| express                  | 4.17.1  | ✓      | 11540.2    | 86.08   | 2.06          |
| express-with-middlewares | 4.17.1  | ✓      | 9581.1     | 103.78  | 3.67          |
| fastify-big-json         | 3.24.1  | ✓      | 9290.5     | 107.02  | 106.88        |
| express-route-prefix     | 4.17.1  | ✓      | 9123.0     | 109.04  | 3.38          |
| farrow-http              | 1.10.12 | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
