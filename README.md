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
* __Machine:__ Linux runnervmf2e7y 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Nov  1 01:15:21 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 76630.4    | 12.56   | 13.67         |
| bare                     | 10.13.0 | ✗      | 66763.2    | 14.49   | 11.91         |
| fastify                  | 3.29.5  | ✓      | 66369.6    | 14.58   | 11.84         |
| foxify                   | 0.10.20 | ✓      | 65191.6    | 14.84   | 10.69         |
| polka                    | 0.5.2   | ✓      | 65146.4    | 14.86   | 11.62         |
| connect                  | 3.7.0   | ✗      | 63468.0    | 15.25   | 11.32         |
| micro                    | 9.4.1   | ✗      | 61848.8    | 15.67   | 11.03         |
| server-base              | 7.1.32  | ✗      | 60569.6    | 16.01   | 10.80         |
| yeps                     | 1.1.1   | ✗      | 58957.6    | 16.46   | 10.51         |
| connect-router           | 1.3.8   | ✓      | 57074.4    | 17.02   | 10.18         |
| server-base-router       | 6.1.5   | ✓      | 56852.0    | 17.10   | 10.14         |
| micro-route              | 2.5.0   | ✓      | 56216.8    | 17.29   | 10.03         |
| trek-engine              | 1.0.5   | ✗      | 55256.0    | 17.60   | 9.06          |
| trek-router              | 1.2.0   | ✓      | 53674.4    | 18.13   | 8.80          |
| spirit                   | 0.6.1   | ✗      | 47952.0    | 20.39   | 8.55          |
| yeps-router              | 1.2.0   | ✓      | 47232.8    | 20.68   | 8.42          |
| vapr                     | 0.5.5   | ✓      | 46492.0    | 21.02   | 7.63          |
| spirit-router            | 0.5.0   | ✓      | 46460.0    | 20.99   | 8.29          |
| koa                      | 2.16.3  | ✗      | 45919.2    | 21.28   | 8.19          |
| total.js                 | 3.4.13  | ✓      | 42605.6    | 22.97   | 13.04         |
| restify                  | 8.6.1   | ✓      | 42059.2    | 23.28   | 7.58          |
| koa-router               | 10.1.1  | ✓      | 41327.4    | 23.70   | 7.37          |
| hapi                     | 20.3.0  | ✓      | 36426.2    | 26.95   | 6.50          |
| microrouter              | 3.1.3   | ✓      | 33652.8    | 29.22   | 6.00          |
| express                  | 4.21.2  | ✓      | 14431.6    | 68.76   | 2.57          |
| fastify-big-json         | 3.29.5  | ✓      | 13134.4    | 75.58   | 151.11        |
| express-with-middlewares | 4.21.2  | ✓      | 12378.4    | 80.22   | 4.75          |
| express-route-prefix     | 4.21.2  | ✓      | 11160.4    | 89.03   | 4.13          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
