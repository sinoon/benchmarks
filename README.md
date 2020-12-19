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
* __Machine:__ Linux fv-az116-655 5.4.0-1032-azure #33~18.04.1-Ubuntu SMP Tue Nov 17 11:40:52 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.20.0`
* __Run:__ Fri Dec 18 17:06:05 UTC 2020

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.9.2   | ✓      | 61008.8    | 15.90   | 10.88         |
| polkadot                 | 1.0.0   | ✗      | 60699.2    | 15.99   | 10.82         |
| bare                     | 10.13.0 | ✗      | 59283.2    | 16.38   | 10.57         |
| polka                    | 0.5.2   | ✓      | 58684.8    | 16.55   | 10.47         |
| micro                    | 9.3.4   | ✗      | 57493.6    | 16.89   | 10.25         |
| foxify                   | 0.10.20 | ✓      | 57380.0    | 16.93   | 9.41          |
| rayo                     | 1.3.6   | ✓      | 57365.6    | 16.93   | 10.23         |
| 0http                    | 3.0.0   | ✓      | 56750.4    | 17.14   | 10.12         |
| connect                  | 3.7.0   | ✗      | 56727.2    | 17.12   | 10.12         |
| server-base              | 7.1.23  | ✗      | 54480.8    | 17.86   | 9.72          |
| yeps                     | 1.1.1   | ✗      | 53322.4    | 18.25   | 9.51          |
| server-base-router       | 6.1.5   | ✓      | 52964.8    | 18.38   | 9.45          |
| micro-route              | 2.5.0   | ✓      | 52798.4    | 18.44   | 9.42          |
| restana                  | 4.8.1   | ✓      | 51859.2    | 18.79   | 9.25          |
| connect-router           | 1.3.5   | ✓      | 51110.4    | 19.07   | 9.11          |
| trek-engine              | 1.0.5   | ✗      | 50253.8    | 19.41   | 8.24          |
| trek-router              | 1.2.0   | ✓      | 48395.0    | 20.17   | 7.94          |
| yeps-router              | 1.2.0   | ✓      | 44279.2    | 22.08   | 7.90          |
| koa                      | 2.13.0  | ✗      | 43365.2    | 22.57   | 7.73          |
| vapr                     | 0.5.5   | ✓      | 41976.0    | 23.33   | 6.89          |
| spirit                   | 0.6.1   | ✗      | 41908.0    | 23.38   | 7.47          |
| spirit-router            | 0.5.0   | ✓      | 40934.4    | 23.94   | 7.30          |
| total.js                 | 3.4.6   | ✓      | 38307.2    | 25.62   | 11.73         |
| koa-router               | 10.0.0  | ✓      | 37244.6    | 26.35   | 6.64          |
| restify                  | 8.5.1   | ✓      | 36078.2    | 27.21   | 6.50          |
| hapi                     | 20.0.3  | ✓      | 30961.2    | 31.80   | 5.52          |
| microrouter              | 3.1.3   | ✓      | 29175.2    | 33.77   | 5.20          |
| egg.js                   | 2.29.1  | ✓      | 19169.5    | 51.66   | 6.75          |
| express                  | 4.17.1  | ✓      | 11474.0    | 86.60   | 2.05          |
| express-with-middlewares | 4.17.1  | ✓      | 9973.5     | 99.67   | 3.82          |
| express-route-prefix     | 4.17.1  | ✓      | 9469.4     | 105.01  | 3.50          |
| fastify-big-json         | 3.9.2   | ✓      | 9217.4     | 107.91  | 106.03        |
| farrow-http              | 1.3.0   | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
