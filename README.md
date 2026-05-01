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
* __Machine:__ Linux runnervmeorf1 6.17.0-1010-azure #10~24.04.1-Ubuntu SMP Fri Mar  6 22:00:57 UTC 2026 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri May  1 01:42:01 UTC 2026

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 71940.4    | 13.40   | 12.83         |
| bare                     | 10.13.0 | ✗      | 64981.2    | 14.90   | 11.59         |
| fastify                  | 3.29.5  | ✓      | 64752.4    | 14.95   | 11.55         |
| polka                    | 0.5.2   | ✓      | 63712.0    | 15.19   | 11.36         |
| foxify                   | 0.10.20 | ✓      | 62357.6    | 15.54   | 10.23         |
| connect                  | 3.7.0   | ✗      | 60690.4    | 15.98   | 10.82         |
| micro                    | 9.4.1   | ✗      | 59244.0    | 16.38   | 10.56         |
| server-base              | 7.1.32  | ✗      | 58085.6    | 16.71   | 10.36         |
| yeps                     | 1.1.1   | ✗      | 57831.2    | 16.79   | 10.31         |
| connect-router           | 1.3.8   | ✓      | 55444.8    | 17.54   | 9.89          |
| server-base-router       | 6.1.5   | ✓      | 55073.6    | 17.66   | 9.82          |
| micro-route              | 2.5.0   | ✓      | 55068.0    | 17.66   | 9.82          |
| trek-engine              | 1.0.5   | ✗      | 53852.8    | 18.07   | 8.83          |
| trek-router              | 1.2.0   | ✓      | 53661.6    | 18.14   | 8.80          |
| vapr                     | 0.5.5   | ✓      | 45860.8    | 21.31   | 7.52          |
| yeps-router              | 1.2.0   | ✓      | 45098.4    | 21.67   | 8.04          |
| koa                      | 2.16.4  | ✗      | 43216.0    | 22.64   | 7.71          |
| spirit-router            | 0.5.0   | ✓      | 42529.6    | 23.01   | 7.58          |
| total.js                 | 3.4.13  | ✓      | 41601.6    | 23.54   | 12.74         |
| spirit                   | 0.6.1   | ✗      | 40942.4    | 23.92   | 7.30          |
| restify                  | 8.6.1   | ✓      | 39556.0    | 24.78   | 7.13          |
| koa-router               | 10.1.1  | ✓      | 38894.6    | 25.21   | 6.94          |
| microrouter              | 3.1.3   | ✓      | 33350.2    | 29.48   | 5.95          |
| hapi                     | 20.3.0  | ✓      | 33079.6    | 29.73   | 5.90          |
| express                  | 4.22.1  | ✓      | 13615.6    | 72.91   | 2.43          |
| fastify-big-json         | 3.29.5  | ✓      | 12549.4    | 79.13   | 144.38        |
| express-with-middlewares | 4.22.1  | ✓      | 12069.2    | 82.28   | 4.63          |
| express-route-prefix     | 4.22.1  | ✓      | 10295.8    | 96.53   | 3.81          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
