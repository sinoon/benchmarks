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
* __Machine:__ Linux fv-az585-363 6.5.0-1018-azure #19~22.04.2-Ubuntu SMP Thu Mar 21 16:45:46 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed May  1 01:05:26 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 71691.6    | 13.48   | 12.78         |
| fastify                  | 3.29.5  | ✓      | 64943.6    | 14.91   | 11.58         |
| bare                     | 10.13.0 | ✗      | 62950.8    | 15.39   | 11.23         |
| polka                    | 0.5.2   | ✓      | 61044.0    | 15.89   | 10.89         |
| connect                  | 3.7.0   | ✗      | 60931.2    | 15.92   | 10.87         |
| foxify                   | 0.10.20 | ✓      | 60508.0    | 16.03   | 9.93          |
| micro                    | 9.4.1   | ✗      | 58716.0    | 16.54   | 10.47         |
| yeps                     | 1.1.1   | ✗      | 58127.2    | 16.71   | 10.37         |
| server-base              | 7.1.32  | ✗      | 58039.2    | 16.74   | 10.35         |
| connect-router           | 1.3.8   | ✓      | 54774.4    | 17.76   | 9.77          |
| server-base-router       | 6.1.5   | ✓      | 54600.0    | 17.82   | 9.74          |
| trek-engine              | 1.0.5   | ✗      | 53864.8    | 18.07   | 8.84          |
| trek-router              | 1.2.0   | ✓      | 53674.4    | 18.14   | 8.80          |
| micro-route              | 2.5.0   | ✓      | 53512.0    | 18.20   | 9.54          |
| spirit                   | 0.6.1   | ✗      | 49759.2    | 19.61   | 8.87          |
| yeps-router              | 1.2.0   | ✓      | 46704.0    | 20.91   | 8.33          |
| vapr                     | 0.5.5   | ✓      | 46563.2    | 20.98   | 7.64          |
| spirit-router            | 0.5.0   | ✓      | 46301.6    | 21.10   | 8.26          |
| koa                      | 2.15.3  | ✗      | 42763.2    | 22.89   | 7.63          |
| total.js                 | 3.4.13  | ✓      | 41931.2    | 23.35   | 12.84         |
| restify                  | 8.6.1   | ✓      | 40903.2    | 23.95   | 7.37          |
| koa-router               | 10.1.1  | ✓      | 38313.8    | 25.61   | 6.83          |
| hapi                     | 20.3.0  | ✓      | 33971.2    | 28.93   | 6.06          |
| microrouter              | 3.1.3   | ✓      | 32514.6    | 30.25   | 5.80          |
| express                  | 4.19.2  | ✓      | 14280.6    | 69.48   | 2.55          |
| fastify-big-json         | 3.29.5  | ✓      | 12706.0    | 78.15   | 146.18        |
| express-with-middlewares | 4.19.2  | ✓      | 12483.4    | 79.53   | 4.79          |
| express-route-prefix     | 4.19.2  | ✓      | 11164.6    | 89.02   | 4.13          |
| egg.js                   | 2.37.0  | ✓      | 10162.0    | 97.81   | 3.58          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
