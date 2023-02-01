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
* __Machine:__ Linux fv-az563-803 5.15.0-1031-azure #38-Ubuntu SMP Mon Jan 9 12:49:59 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Feb  1 01:06:51 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| bare                     | 10.13.0 | ✗      | 64225.2    | 15.08   | 11.45         |
| polkadot                 | 1.0.0   | ✗      | 63881.6    | 15.18   | 11.39         |
| fastify                  | 3.29.5  | ✓      | 62976.4    | 15.39   | 11.23         |
| polka                    | 0.5.2   | ✓      | 62129.6    | 15.61   | 11.08         |
| foxify                   | 0.10.20 | ✓      | 62095.2    | 15.62   | 10.19         |
| 0http                    | 3.4.2   | ✓      | 60451.2    | 16.05   | 10.78         |
| micro                    | 9.4.1   | ✗      | 60128.8    | 16.14   | 10.72         |
| connect                  | 3.7.0   | ✗      | 59987.2    | 16.18   | 10.70         |
| server-base              | 7.1.32  | ✗      | 59192.0    | 16.40   | 10.56         |
| yeps                     | 1.1.1   | ✗      | 56681.6    | 17.14   | 10.11         |
| connect-router           | 1.3.7   | ✓      | 54473.6    | 17.86   | 9.71          |
| server-base-router       | 6.1.5   | ✓      | 53060.0    | 18.34   | 9.46          |
| micro-route              | 2.5.0   | ✓      | 52917.6    | 18.40   | 9.44          |
| trek-router              | 1.2.0   | ✓      | 52653.6    | 18.50   | 8.64          |
| restana                  | 4.9.7   | ✓      | 52596.0    | 18.51   | 9.38          |
| trek-engine              | 1.0.5   | ✗      | 51072.0    | 19.08   | 8.38          |
| yeps-router              | 1.2.0   | ✓      | 46050.4    | 21.22   | 8.21          |
| vapr                     | 0.5.5   | ✓      | 45141.6    | 21.66   | 7.40          |
| koa                      | 2.14.1  | ✗      | 41711.2    | 23.48   | 7.44          |
| spirit                   | 0.6.1   | ✗      | 41645.6    | 23.52   | 7.43          |
| total.js                 | 3.4.13  | ✓      | 40539.2    | 24.17   | 12.41         |
| restify                  | 8.6.1   | ✓      | 40221.6    | 24.36   | 7.25          |
| spirit-router            | 0.5.0   | ✓      | 40128.8    | 24.43   | 7.16          |
| koa-router               | 10.1.1  | ✓      | 39189.8    | 25.02   | 6.99          |
| hapi                     | 20.2.2  | ✓      | 32274.6    | 30.49   | 5.76          |
| microrouter              | 3.1.3   | ✓      | 31498.8    | 31.25   | 5.62          |
| express                  | 4.18.2  | ✓      | 12758.4    | 77.82   | 2.28          |
| express-with-middlewares | 4.18.2  | ✓      | 10879.2    | 91.35   | 4.17          |
| express-route-prefix     | 4.18.2  | ✓      | 10819.9    | 91.85   | 4.00          |
| fastify-big-json         | 3.29.5  | ✓      | 10077.6    | 98.66   | 115.94        |
| egg.js                   | 2.37.0  | ✓      | 7331.3     | 135.62  | 2.58          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
