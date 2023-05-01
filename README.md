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
* __Machine:__ Linux fv-az796-797 5.15.0-1036-azure #43-Ubuntu SMP Wed Mar 29 16:11:05 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon May  1 01:05:04 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.29.5  | ✓      | 72654.8    | 13.28   | 12.96         |
| polkadot                 | 1.0.0   | ✗      | 72556.4    | 13.29   | 12.94         |
| 0http                    | 3.5.2   | ✓      | 70025.2    | 13.78   | 12.49         |
| bare                     | 10.13.0 | ✗      | 69726.8    | 13.85   | 12.44         |
| foxify                   | 0.10.20 | ✓      | 69450.8    | 13.89   | 11.39         |
| polka                    | 0.5.2   | ✓      | 67891.2    | 14.24   | 12.11         |
| connect                  | 3.7.0   | ✗      | 66691.6    | 14.49   | 11.89         |
| micro                    | 9.4.1   | ✗      | 65113.2    | 14.86   | 11.61         |
| server-base              | 7.1.32  | ✗      | 64239.6    | 15.08   | 11.46         |
| yeps                     | 1.1.1   | ✗      | 63458.0    | 15.26   | 11.32         |
| restana                  | 4.9.7   | ✓      | 63213.6    | 15.32   | 11.27         |
| server-base-router       | 6.1.5   | ✓      | 62371.2    | 15.54   | 11.12         |
| micro-route              | 2.5.0   | ✓      | 60892.0    | 15.93   | 10.86         |
| connect-router           | 1.3.8   | ✓      | 57092.0    | 17.01   | 10.18         |
| trek-engine              | 1.0.5   | ✗      | 56954.4    | 17.07   | 9.34          |
| trek-router              | 1.2.0   | ✓      | 56198.4    | 17.29   | 9.22          |
| yeps-router              | 1.2.0   | ✓      | 49941.6    | 19.52   | 8.91          |
| vapr                     | 0.5.5   | ✓      | 49828.0    | 19.57   | 8.17          |
| koa                      | 2.14.2  | ✗      | 48817.6    | 19.98   | 8.71          |
| spirit-router            | 0.5.0   | ✓      | 48780.0    | 20.01   | 8.70          |
| spirit                   | 0.6.1   | ✗      | 48199.2    | 20.25   | 8.60          |
| total.js                 | 3.4.13  | ✓      | 45876.0    | 21.30   | 14.04         |
| restify                  | 8.6.1   | ✓      | 44443.2    | 22.00   | 8.01          |
| koa-router               | 10.1.1  | ✓      | 43387.4    | 22.54   | 7.74          |
| hapi                     | 20.3.0  | ✓      | 37883.2    | 25.90   | 6.76          |
| microrouter              | 3.1.3   | ✓      | 35626.2    | 27.56   | 6.35          |
| express                  | 4.18.2  | ✓      | 14722.8    | 67.38   | 2.63          |
| express-with-middlewares | 4.18.2  | ✓      | 12726.6    | 78.03   | 4.88          |
| express-route-prefix     | 4.18.2  | ✓      | 12647.9    | 78.52   | 4.68          |
| fastify-big-json         | 3.29.5  | ✓      | 11765.4    | 84.43   | 135.36        |
| egg.js                   | 2.37.0  | ✓      | 8784.5     | 113.23  | 3.09          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
