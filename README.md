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
* __Machine:__ Linux fv-az178-186 5.11.0-1028-azure #31~20.04.2-Ubuntu SMP Tue Jan 18 08:46:15 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.10`
* __Run:__ Tue Mar  1 02:03:53 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 107.7      | 17.32   | 0.02          |
| fastify                  | 3.27.2  | ✓      | 106.5      | 17.24   | 0.02          |
| bare                     | 10.13.0 | ✗      | 101.6      | 17.38   | 0.02          |
| polka                    | 0.5.2   | ✓      | 69.7       | 17.87   | 0.01          |
| 0http                    | 3.1.2   | ✓      | 65.7       | 17.68   | 0.01          |
| connect                  | 3.7.0   | ✗      | 56.0       | 18.45   | 0.01          |
| foxify                   | 0.10.20 | ✓      | 55.8       | 18.09   | 0.01          |
| rayo                     | 1.3.10  | ✓      | 54.8       | 18.25   | 0.01          |
| micro                    | 9.3.4   | ✗      | 53.6       | 18.66   | 0.01          |
| restana                  | 4.9.3   | ✓      | 53.3       | 19.99   | 0.01          |
| yeps                     | 1.1.1   | ✗      | 53.0       | 19.13   | 0.01          |
| server-base              | 7.1.29  | ✗      | 52.7       | 18.92   | 0.01          |
| connect-router           | 1.3.6   | ✓      | 50.9       | 19.76   | 0.01          |
| server-base-router       | 6.1.5   | ✓      | 50.1       | 19.93   | 0.01          |
| micro-route              | 2.5.0   | ✓      | 49.9       | 19.87   | 0.01          |
| spirit-router            | 0.5.0   | ✓      | 48.0       | 27.35   | 0.01          |
| trek-engine              | 1.0.5   | ✗      | 46.1       | 21.63   | 0.01          |
| trek-router              | 1.2.0   | ✓      | 45.9       | 21.74   | 0.01          |
| spirit                   | 0.6.1   | ✗      | 45.6       | 27.64   | 0.01          |
| yeps-router              | 1.2.0   | ✓      | 41.5       | 24.04   | 0.01          |
| koa                      | 2.13.4  | ✗      | 41.3       | 24.18   | 0.01          |
| vapr                     | 0.5.5   | ✓      | 40.0       | 24.95   | 0.01          |
| total.js                 | 3.4.13  | ✓      | 37.7       | 26.61   | 0.01          |
| koa-router               | 10.1.1  | ✓      | 35.6       | 28.64   | 0.01          |
| restify                  | 8.6.1   | ✓      | 34.9       | 28.91   | 0.01          |
| hapi                     | 20.2.1  | ✓      | 29.5       | 34.05   | 0.01          |
| microrouter              | 3.1.3   | ✓      | 27.7       | 36.10   | 0.00          |
| egg.js                   | 2.33.1  | ✓      | 19.2       | 52.74   | 0.01          |
| express                  | 4.17.3  | ✓      | 11.8       | 87.97   | 0.00          |
| express-route-prefix     | 4.17.3  | ✓      | 10.5       | 101.83  | 0.00          |
| express-with-middlewares | 4.17.3  | ✓      | 10.2       | 101.67  | 0.00          |
| fastify-big-json         | 3.27.2  | ✓      | 9.4        | 108.64  | 0.11          |
| farrow-http              | 1.11.4  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
