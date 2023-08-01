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
* __Machine:__ Linux fv-az587-579 5.15.0-1041-azure #48-Ubuntu SMP Tue Jun 20 20:34:08 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Tue Aug  1 01:07:43 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 71096.4    | 13.58   | 12.68         |
| fastify                  | 3.29.5  | ✓      | 70076.4    | 13.78   | 12.50         |
| bare                     | 10.13.0 | ✗      | 68346.8    | 14.14   | 12.19         |
| polka                    | 0.5.2   | ✓      | 68217.6    | 14.16   | 12.17         |
| 0http                    | 3.5.2   | ✓      | 67499.2    | 14.33   | 12.04         |
| foxify                   | 0.10.20 | ✓      | 66168.4    | 14.61   | 10.85         |
| connect                  | 3.7.0   | ✗      | 64591.0    | 15.00   | 11.52         |
| server-base              | 7.1.32  | ✗      | 64233.2    | 15.07   | 11.46         |
| micro                    | 9.4.1   | ✗      | 62577.6    | 15.49   | 11.16         |
| yeps                     | 1.1.1   | ✗      | 62197.6    | 15.58   | 11.09         |
| server-base-router       | 6.1.5   | ✓      | 60985.6    | 15.90   | 10.88         |
| restana                  | 4.9.7   | ✓      | 60273.6    | 16.10   | 10.75         |
| micro-route              | 2.5.0   | ✓      | 58583.2    | 16.58   | 10.45         |
| connect-router           | 1.3.8   | ✓      | 57572.8    | 16.88   | 10.27         |
| trek-engine              | 1.0.5   | ✗      | 56520.0    | 17.20   | 9.27          |
| trek-router              | 1.2.0   | ✓      | 54496.0    | 17.85   | 8.94          |
| yeps-router              | 1.2.0   | ✓      | 51500.0    | 18.93   | 9.18          |
| vapr                     | 0.5.5   | ✓      | 51270.4    | 19.00   | 8.41          |
| spirit                   | 0.6.1   | ✗      | 48703.2    | 20.04   | 8.69          |
| koa                      | 2.14.2  | ✗      | 46705.6    | 20.91   | 8.33          |
| spirit-router            | 0.5.0   | ✓      | 46262.4    | 21.13   | 8.25          |
| total.js                 | 3.4.13  | ✓      | 44880.0    | 21.78   | 13.74         |
| restify                  | 8.6.1   | ✓      | 42989.8    | 22.76   | 7.75          |
| koa-router               | 10.1.1  | ✓      | 41998.4    | 23.32   | 7.49          |
| hapi                     | 20.3.0  | ✓      | 37001.8    | 26.53   | 6.60          |
| microrouter              | 3.1.3   | ✓      | 35383.4    | 27.76   | 6.31          |
| express                  | 4.18.2  | ✓      | 14292.6    | 69.43   | 2.55          |
| express-with-middlewares | 4.18.2  | ✓      | 12561.0    | 79.06   | 4.82          |
| express-route-prefix     | 4.18.2  | ✓      | 11944.3    | 83.20   | 4.42          |
| fastify-big-json         | 3.29.5  | ✓      | 11468.2    | 86.75   | 131.93        |
| egg.js                   | 2.37.0  | ✓      | 8526.5     | 116.71  | 3.00          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
