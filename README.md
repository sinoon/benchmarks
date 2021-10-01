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
* __Machine:__ Linux fv-az252-296 5.8.0-1042-azure #45~20.04.1-Ubuntu SMP Wed Sep 15 14:24:15 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.6`
* __Run:__ Fri Oct  1 01:47:39 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| 0http                    | 3.1.1   | ✓      | 69074.8    | 14.00   | 12.32         |
| bare                     | 10.13.0 | ✗      | 68485.2    | 14.11   | 12.21         |
| server-base              | 7.1.29  | ✗      | 67188.8    | 14.40   | 11.98         |
| fastify                  | 3.22.0  | ✓      | 65619.6    | 14.75   | 11.70         |
| polkadot                 | 1.0.0   | ✗      | 64816.0    | 14.94   | 11.56         |
| foxify                   | 0.10.20 | ✓      | 64648.0    | 14.98   | 10.60         |
| restana                  | 4.9.1   | ✓      | 63816.8    | 15.19   | 11.38         |
| micro                    | 9.3.4   | ✗      | 62781.2    | 15.43   | 11.20         |
| polka                    | 0.5.2   | ✓      | 62221.6    | 15.57   | 11.10         |
| rayo                     | 1.3.6   | ✓      | 61785.6    | 15.68   | 11.02         |
| server-base-router       | 6.1.5   | ✓      | 60359.2    | 16.07   | 10.76         |
| connect                  | 3.7.0   | ✗      | 59624.8    | 16.28   | 10.63         |
| yeps                     | 1.1.1   | ✗      | 59456.0    | 16.33   | 10.60         |
| connect-router           | 1.3.5   | ✓      | 56488.8    | 17.20   | 10.07         |
| micro-route              | 2.5.0   | ✓      | 56196.8    | 17.29   | 10.02         |
| trek-engine              | 1.0.5   | ✗      | 50627.2    | 19.26   | 8.30          |
| trek-router              | 1.2.0   | ✓      | 50296.8    | 19.38   | 8.25          |
| yeps-router              | 1.2.0   | ✓      | 47504.8    | 20.55   | 8.47          |
| koa                      | 2.13.3  | ✗      | 46826.4    | 20.86   | 8.35          |
| spirit                   | 0.6.1   | ✗      | 45689.6    | 21.41   | 8.15          |
| spirit-router            | 0.5.0   | ✓      | 44687.2    | 21.89   | 7.97          |
| vapr                     | 0.5.5   | ✓      | 44639.2    | 21.90   | 7.32          |
| total.js                 | 3.4.10  | ✓      | 43221.6    | 22.65   | 13.23         |
| restify                  | 8.6.0   | ✓      | 39628.0    | 24.74   | 7.14          |
| koa-router               | 10.1.1  | ✓      | 38845.8    | 25.25   | 6.93          |
| microrouter              | 3.1.3   | ✓      | 34910.4    | 28.14   | 6.23          |
| hapi                     | 20.2.0  | ✓      | 32630.4    | 30.15   | 5.82          |
| egg.js                   | 2.30.0  | ✓      | 18809.5    | 52.65   | 6.62          |
| express                  | 4.17.1  | ✓      | 13160.0    | 75.44   | 2.35          |
| express-with-middlewares | 4.17.1  | ✓      | 11281.0    | 88.06   | 4.32          |
| express-route-prefix     | 4.17.1  | ✓      | 10721.5    | 92.69   | 3.97          |
| fastify-big-json         | 3.22.0  | ✓      | 10540.8    | 94.30   | 121.26        |
| farrow-http              | 1.10.9  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
