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
* __Machine:__ Linux fv-az477-628 6.2.0-1015-azure #15~22.04.1-Ubuntu SMP Fri Oct  6 13:20:44 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Nov  1 01:04:04 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 70945.6    | 13.61   | 12.65         |
| bare                     | 10.13.0 | ✗      | 67461.6    | 14.33   | 12.03         |
| fastify                  | 3.29.5  | ✓      | 66640.8    | 14.51   | 11.88         |
| 0http                    | 3.5.2   | ✓      | 66246.0    | 14.60   | 11.81         |
| polka                    | 0.5.2   | ✓      | 65124.0    | 14.86   | 11.61         |
| connect                  | 3.7.0   | ✗      | 64819.2    | 14.93   | 11.56         |
| foxify                   | 0.10.20 | ✓      | 64179.2    | 15.08   | 10.53         |
| micro                    | 9.4.1   | ✗      | 63157.6    | 15.34   | 11.26         |
| restana                  | 4.9.7   | ✓      | 60582.4    | 16.03   | 10.80         |
| server-base              | 7.1.32  | ✗      | 60483.2    | 16.03   | 10.79         |
| yeps                     | 1.1.1   | ✗      | 60430.4    | 16.05   | 10.78         |
| connect-router           | 1.3.8   | ✓      | 58230.4    | 16.68   | 10.38         |
| server-base-router       | 6.1.5   | ✓      | 57760.8    | 16.82   | 10.30         |
| micro-route              | 2.5.0   | ✓      | 57434.4    | 16.92   | 10.24         |
| trek-engine              | 1.0.5   | ✗      | 54537.6    | 17.84   | 8.95          |
| trek-router              | 1.2.0   | ✓      | 52968.0    | 18.39   | 8.69          |
| yeps-router              | 1.2.0   | ✓      | 48470.4    | 20.13   | 8.64          |
| vapr                     | 0.5.5   | ✓      | 48073.6    | 20.30   | 7.89          |
| koa                      | 2.14.2  | ✗      | 46888.0    | 20.83   | 8.36          |
| spirit                   | 0.6.1   | ✗      | 45808.0    | 21.33   | 8.17          |
| spirit-router            | 0.5.0   | ✓      | 43220.0    | 22.64   | 7.71          |
| total.js                 | 3.4.13  | ✓      | 42839.2    | 22.85   | 13.11         |
| koa-router               | 10.1.1  | ✓      | 42219.4    | 23.19   | 7.53          |
| restify                  | 8.6.1   | ✓      | 41781.4    | 23.44   | 7.53          |
| hapi                     | 20.3.0  | ✓      | 36259.4    | 27.08   | 6.47          |
| microrouter              | 3.1.3   | ✓      | 34001.8    | 28.91   | 6.06          |
| express                  | 4.18.2  | ✓      | 14155.2    | 70.12   | 2.52          |
| express-with-middlewares | 4.18.2  | ✓      | 12365.0    | 80.32   | 4.74          |
| fastify-big-json         | 3.29.5  | ✓      | 11354.6    | 87.51   | 130.63        |
| express-route-prefix     | 4.18.2  | ✓      | 10357.6    | 95.93   | 3.83          |
| egg.js                   | 2.37.0  | ✓      | 8359.3     | 119.09  | 2.94          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.5   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
