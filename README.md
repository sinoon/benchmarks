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
* __Machine:__ Linux fv-az1384-380 6.8.0-1021-azure #25-Ubuntu SMP Wed Jan 15 20:45:09 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Tue Apr  1 01:14:57 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74880.0    | 12.87   | 13.35         |
| fastify                  | 3.29.5  | ✓      | 67734.0    | 14.26   | 12.08         |
| bare                     | 10.13.0 | ✗      | 64271.2    | 15.06   | 11.46         |
| foxify                   | 0.10.20 | ✓      | 63291.2    | 15.30   | 10.38         |
| polka                    | 0.5.2   | ✓      | 62195.2    | 15.58   | 11.09         |
| connect                  | 3.7.0   | ✗      | 61340.8    | 15.81   | 10.94         |
| micro                    | 9.4.1   | ✗      | 60824.0    | 15.95   | 10.85         |
| server-base              | 7.1.32  | ✗      | 60160.0    | 16.12   | 10.73         |
| yeps                     | 1.1.1   | ✗      | 57684.8    | 16.84   | 10.29         |
| server-base-router       | 6.1.5   | ✓      | 55444.8    | 17.54   | 9.89          |
| connect-router           | 1.3.8   | ✓      | 54344.0    | 17.90   | 9.69          |
| micro-route              | 2.5.0   | ✓      | 53895.2    | 18.05   | 9.61          |
| trek-engine              | 1.0.5   | ✗      | 53874.4    | 18.07   | 8.84          |
| trek-router              | 1.2.0   | ✓      | 53391.2    | 18.23   | 8.76          |
| yeps-router              | 1.2.0   | ✓      | 47460.8    | 20.57   | 8.46          |
| spirit                   | 0.6.1   | ✗      | 46612.0    | 20.95   | 8.31          |
| vapr                     | 0.5.5   | ✓      | 46267.2    | 21.12   | 7.59          |
| koa                      | 2.16.0  | ✗      | 45746.4    | 21.36   | 8.16          |
| spirit-router            | 0.5.0   | ✓      | 45320.8    | 21.58   | 8.08          |
| total.js                 | 3.4.13  | ✓      | 42898.4    | 22.81   | 13.13         |
| restify                  | 8.6.1   | ✓      | 41918.4    | 23.36   | 7.56          |
| koa-router               | 10.1.1  | ✓      | 40487.2    | 24.20   | 7.22          |
| hapi                     | 20.3.0  | ✓      | 35903.8    | 27.35   | 6.40          |
| microrouter              | 3.1.3   | ✓      | 33420.8    | 29.42   | 5.96          |
| express                  | 4.21.2  | ✓      | 14687.2    | 67.54   | 2.62          |
| fastify-big-json         | 3.29.5  | ✓      | 12928.8    | 76.79   | 148.74        |
| express-with-middlewares | 4.21.2  | ✓      | 12450.2    | 79.75   | 4.77          |
| express-route-prefix     | 4.21.2  | ✓      | 11022.8    | 90.14   | 4.08          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
