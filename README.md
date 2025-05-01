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
* __Machine:__ Linux fv-az1718-195 6.11.0-1012-azure #12~24.04.1-Ubuntu SMP Mon Mar 10 19:00:39 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu May  1 01:15:21 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75811.2    | 12.70   | 13.52         |
| fastify                  | 3.29.5  | ✓      | 67774.8    | 14.26   | 12.09         |
| bare                     | 10.13.0 | ✗      | 65367.2    | 14.81   | 11.66         |
| foxify                   | 0.10.20 | ✓      | 64596.4    | 14.98   | 10.60         |
| polka                    | 0.5.2   | ✓      | 62636.8    | 15.46   | 11.17         |
| connect                  | 3.7.0   | ✗      | 62007.2    | 15.63   | 11.06         |
| micro                    | 9.4.1   | ✗      | 60625.6    | 16.00   | 10.81         |
| server-base              | 7.1.32  | ✗      | 60231.2    | 16.10   | 10.74         |
| yeps                     | 1.1.1   | ✗      | 57565.6    | 16.88   | 10.27         |
| server-base-router       | 6.1.5   | ✓      | 55812.8    | 17.41   | 9.95          |
| connect-router           | 1.3.8   | ✓      | 55038.4    | 17.67   | 9.82          |
| micro-route              | 2.5.0   | ✓      | 54283.2    | 17.93   | 9.68          |
| trek-engine              | 1.0.5   | ✗      | 54092.0    | 17.99   | 8.87          |
| trek-router              | 1.2.0   | ✓      | 53518.4    | 18.19   | 8.78          |
| yeps-router              | 1.2.0   | ✓      | 47784.0    | 20.43   | 8.52          |
| vapr                     | 0.5.5   | ✓      | 46252.0    | 21.12   | 7.59          |
| koa                      | 2.16.1  | ✗      | 46174.4    | 21.16   | 8.23          |
| spirit                   | 0.6.1   | ✗      | 45650.4    | 21.39   | 8.14          |
| spirit-router            | 0.5.0   | ✓      | 43126.4    | 22.71   | 7.69          |
| total.js                 | 3.4.13  | ✓      | 42724.8    | 22.91   | 13.08         |
| restify                  | 8.6.1   | ✓      | 42220.6    | 23.19   | 7.61          |
| koa-router               | 10.1.1  | ✓      | 41572.0    | 23.56   | 7.41          |
| hapi                     | 20.3.0  | ✓      | 36312.6    | 27.03   | 6.48          |
| microrouter              | 3.1.3   | ✓      | 33963.2    | 28.94   | 6.06          |
| express                  | 4.21.2  | ✓      | 14771.0    | 67.16   | 2.63          |
| fastify-big-json         | 3.29.5  | ✓      | 12849.0    | 77.29   | 147.81        |
| express-with-middlewares | 4.21.2  | ✓      | 12255.2    | 81.03   | 4.70          |
| express-route-prefix     | 4.21.2  | ✓      | 11125.8    | 89.30   | 4.12          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
