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
* __Machine:__ Linux fv-az1490-764 6.5.0-1025-azure #26~22.04.1-Ubuntu SMP Thu Jul 11 22:33:04 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Dec  1 01:15:57 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75686.4    | 12.72   | 13.50         |
| fastify                  | 3.29.5  | ✓      | 66470.0    | 14.55   | 11.85         |
| bare                     | 10.13.0 | ✗      | 64092.4    | 15.10   | 11.43         |
| polka                    | 0.5.2   | ✓      | 62780.8    | 15.43   | 11.20         |
| foxify                   | 0.10.20 | ✓      | 62564.8    | 15.48   | 10.26         |
| connect                  | 3.7.0   | ✗      | 61651.2    | 15.72   | 10.99         |
| micro                    | 9.4.1   | ✗      | 59986.4    | 16.17   | 10.70         |
| server-base              | 7.1.32  | ✗      | 59939.2    | 16.18   | 10.69         |
| yeps                     | 1.1.1   | ✗      | 57071.2    | 17.03   | 10.18         |
| server-base-router       | 6.1.5   | ✓      | 56203.2    | 17.30   | 10.02         |
| micro-route              | 2.5.0   | ✓      | 53943.2    | 18.04   | 9.62          |
| connect-router           | 1.3.8   | ✓      | 53864.0    | 18.07   | 9.61          |
| trek-engine              | 1.0.5   | ✗      | 53559.2    | 18.18   | 8.79          |
| trek-router              | 1.2.0   | ✓      | 51460.8    | 18.93   | 8.44          |
| yeps-router              | 1.2.0   | ✓      | 46820.8    | 20.86   | 8.35          |
| vapr                     | 0.5.5   | ✓      | 44949.6    | 21.75   | 7.37          |
| koa                      | 2.15.3  | ✗      | 44546.4    | 21.95   | 7.94          |
| spirit                   | 0.6.1   | ✗      | 43996.0    | 22.22   | 7.85          |
| spirit-router            | 0.5.0   | ✓      | 43584.8    | 22.43   | 7.77          |
| total.js                 | 3.4.13  | ✓      | 41954.4    | 23.34   | 12.84         |
| restify                  | 8.6.1   | ✓      | 41524.8    | 23.58   | 7.48          |
| koa-router               | 10.1.1  | ✓      | 39852.2    | 24.59   | 7.11          |
| hapi                     | 20.3.0  | ✓      | 34682.2    | 28.33   | 6.19          |
| microrouter              | 3.1.3   | ✓      | 32270.0    | 30.48   | 5.75          |
| express                  | 4.21.1  | ✓      | 14184.8    | 69.95   | 2.53          |
| fastify-big-json         | 3.29.5  | ✓      | 12807.2    | 77.53   | 147.35        |
| express-with-middlewares | 4.21.1  | ✓      | 12298.6    | 80.76   | 4.71          |
| express-route-prefix     | 4.21.1  | ✓      | 11029.6    | 90.09   | 4.08          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
