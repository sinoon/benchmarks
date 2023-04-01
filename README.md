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
* __Machine:__ Linux fv-az571-892 5.15.0-1034-azure #41-Ubuntu SMP Fri Feb 10 19:59:45 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Apr  1 01:04:46 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 33357.2    | 29.53   | 5.95          |
| fastify                  | 3.29.5  | ✓      | 31696.8    | 31.09   | 5.65          |
| micro                    | 9.4.1   | ✗      | 31661.8    | 31.09   | 5.65          |
| connect                  | 3.7.0   | ✗      | 30256.4    | 32.57   | 5.40          |
| polka                    | 0.5.2   | ✓      | 30057.6    | 32.76   | 5.36          |
| 0http                    | 3.5.1   | ✓      | 29636.8    | 33.25   | 5.29          |
| bare                     | 10.13.0 | ✗      | 29482.0    | 33.47   | 5.26          |
| server-base              | 7.1.32  | ✗      | 28784.8    | 34.26   | 5.13          |
| foxify                   | 0.10.20 | ✓      | 28766.0    | 34.26   | 4.72          |
| yeps                     | 1.1.1   | ✗      | 28691.6    | 34.36   | 5.12          |
| connect-router           | 1.3.8   | ✓      | 27553.6    | 35.80   | 4.91          |
| server-base-router       | 6.1.5   | ✓      | 27209.2    | 36.25   | 4.85          |
| trek-engine              | 1.0.5   | ✗      | 27098.4    | 36.40   | 4.44          |
| restana                  | 4.9.7   | ✓      | 26552.4    | 37.16   | 4.73          |
| micro-route              | 2.5.0   | ✓      | 26470.4    | 37.27   | 4.72          |
| trek-router              | 1.2.0   | ✓      | 26301.5    | 37.52   | 4.31          |
| yeps-router              | 1.2.0   | ✓      | 25547.6    | 38.66   | 4.56          |
| spirit-router            | 0.5.0   | ✓      | 24823.6    | 39.86   | 4.43          |
| koa                      | 2.14.1  | ✗      | 22698.0    | 43.57   | 4.05          |
| spirit                   | 0.6.1   | ✗      | 22683.6    | 43.64   | 4.05          |
| vapr                     | 0.5.5   | ✓      | 22406.4    | 44.12   | 3.68          |
| restify                  | 8.6.1   | ✓      | 21902.4    | 45.16   | 3.95          |
| total.js                 | 3.4.13  | ✓      | 20468.8    | 48.35   | 6.27          |
| koa-router               | 10.1.1  | ✓      | 19499.5    | 50.77   | 3.48          |
| hapi                     | 20.3.0  | ✓      | 18415.4    | 53.79   | 3.28          |
| microrouter              | 3.1.3   | ✓      | 18333.1    | 54.05   | 3.27          |
| express                  | 4.18.2  | ✓      | 7137.6     | 139.43  | 1.27          |
| fastify-big-json         | 3.29.5  | ✓      | 6984.4     | 142.44  | 80.35         |
| express-with-middlewares | 4.18.2  | ✓      | 6287.2     | 158.37  | 2.41          |
| express-route-prefix     | 4.18.2  | ✓      | 6166.4     | 161.34  | 2.28          |
| egg.js                   | 2.37.0  | ✓      | 4693.0     | 212.44  | 1.65          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
