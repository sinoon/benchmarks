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
* __Machine:__ Linux runnervmh13bl 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu Jan  1 01:19:36 UTC 2026

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 76188.8    | 12.63   | 13.59         |
| fastify                  | 3.29.5  | ✓      | 66876.8    | 14.46   | 11.93         |
| bare                     | 10.13.0 | ✗      | 65216.4    | 14.84   | 11.63         |
| foxify                   | 0.10.20 | ✓      | 63715.6    | 15.20   | 10.45         |
| polka                    | 0.5.2   | ✓      | 61751.2    | 15.70   | 11.01         |
| connect                  | 3.7.0   | ✗      | 61352.0    | 15.80   | 10.94         |
| micro                    | 9.4.1   | ✗      | 59980.0    | 16.18   | 10.70         |
| server-base              | 7.1.32  | ✗      | 58680.0    | 16.54   | 10.47         |
| yeps                     | 1.1.1   | ✗      | 58187.2    | 16.69   | 10.38         |
| micro-route              | 2.5.0   | ✓      | 54813.6    | 17.75   | 9.77          |
| connect-router           | 1.3.8   | ✓      | 54516.0    | 17.85   | 9.72          |
| server-base-router       | 6.1.5   | ✓      | 54433.6    | 17.87   | 9.71          |
| trek-engine              | 1.0.5   | ✗      | 53565.6    | 18.17   | 8.79          |
| trek-router              | 1.2.0   | ✓      | 51623.2    | 18.87   | 8.47          |
| yeps-router              | 1.2.0   | ✓      | 47114.4    | 20.73   | 8.40          |
| vapr                     | 0.5.5   | ✓      | 45942.4    | 21.27   | 7.54          |
| koa                      | 2.16.3  | ✗      | 45386.4    | 21.54   | 8.09          |
| spirit-router            | 0.5.0   | ✓      | 44838.4    | 21.80   | 8.00          |
| spirit                   | 0.6.1   | ✗      | 42848.0    | 22.85   | 7.64          |
| restify                  | 8.6.1   | ✓      | 42190.4    | 23.21   | 7.60          |
| total.js                 | 3.4.13  | ✓      | 42067.2    | 23.27   | 12.88         |
| koa-router               | 10.1.1  | ✓      | 40772.0    | 24.03   | 7.27          |
| hapi                     | 20.3.0  | ✓      | 34594.6    | 28.41   | 6.17          |
| microrouter              | 3.1.3   | ✓      | 32747.0    | 30.03   | 5.84          |
| express                  | 4.22.1  | ✓      | 14048.4    | 70.64   | 2.51          |
| fastify-big-json         | 3.29.5  | ✓      | 13004.4    | 76.34   | 149.62        |
| express-with-middlewares | 4.22.1  | ✓      | 12401.8    | 80.08   | 4.75          |
| express-route-prefix     | 4.22.1  | ✓      | 11182.4    | 88.85   | 4.14          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
