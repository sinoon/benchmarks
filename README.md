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
* __Machine:__ Linux pkrvmjbmru5nbw0 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri Aug  1 01:19:40 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74256.4    | 12.98   | 13.24         |
| fastify                  | 3.29.5  | ✓      | 66504.8    | 14.54   | 11.86         |
| bare                     | 10.13.0 | ✗      | 65055.2    | 14.88   | 11.60         |
| polka                    | 0.5.2   | ✓      | 63228.8    | 15.32   | 11.28         |
| foxify                   | 0.10.20 | ✓      | 62668.0    | 15.46   | 10.28         |
| connect                  | 3.7.0   | ✗      | 61883.2    | 15.66   | 11.04         |
| micro                    | 9.4.1   | ✗      | 61052.0    | 15.88   | 10.89         |
| server-base              | 7.1.32  | ✗      | 59605.6    | 16.28   | 10.63         |
| yeps                     | 1.1.1   | ✗      | 58272.8    | 16.66   | 10.39         |
| server-base-router       | 6.1.5   | ✓      | 56247.2    | 17.28   | 10.03         |
| connect-router           | 1.3.8   | ✓      | 56076.0    | 17.33   | 10.00         |
| micro-route              | 2.5.0   | ✓      | 55420.8    | 17.54   | 9.88          |
| trek-router              | 1.2.0   | ✓      | 52322.4    | 18.62   | 8.58          |
| trek-engine              | 1.0.5   | ✗      | 52319.2    | 18.62   | 8.58          |
| yeps-router              | 1.2.0   | ✓      | 47211.2    | 20.69   | 8.42          |
| koa                      | 2.16.2  | ✗      | 45800.8    | 21.33   | 8.17          |
| vapr                     | 0.5.5   | ✓      | 45144.8    | 21.65   | 7.41          |
| spirit-router            | 0.5.0   | ✓      | 43388.8    | 22.55   | 7.74          |
| total.js                 | 3.4.13  | ✓      | 43068.0    | 22.72   | 13.18         |
| spirit                   | 0.6.1   | ✗      | 42091.2    | 23.26   | 7.51          |
| restify                  | 8.6.1   | ✓      | 41592.0    | 23.54   | 7.50          |
| koa-router               | 10.1.1  | ✓      | 39817.6    | 24.62   | 7.10          |
| hapi                     | 20.3.0  | ✓      | 34682.4    | 28.33   | 6.18          |
| microrouter              | 3.1.3   | ✓      | 33855.6    | 29.03   | 6.04          |
| express                  | 4.21.2  | ✓      | 14446.4    | 68.68   | 2.58          |
| fastify-big-json         | 3.29.5  | ✓      | 13089.8    | 75.86   | 150.59        |
| express-with-middlewares | 4.21.2  | ✓      | 12230.8    | 81.21   | 4.69          |
| express-route-prefix     | 4.21.2  | ✓      | 11055.6    | 89.86   | 4.09          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
