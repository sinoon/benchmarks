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
* __Machine:__ Linux fv-az693-257 6.5.0-1024-azure #25~22.04.1-Ubuntu SMP Mon Jun 17 18:38:57 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu Aug  1 01:08:32 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 75835.2    | 12.70   | 13.52         |
| fastify                  | 3.29.5  | ✓      | 67518.8    | 14.31   | 12.04         |
| polka                    | 0.5.2   | ✓      | 64850.4    | 14.93   | 11.56         |
| foxify                   | 0.10.20 | ✓      | 63800.4    | 15.18   | 10.47         |
| bare                     | 10.13.0 | ✗      | 63315.6    | 15.31   | 11.29         |
| connect                  | 3.7.0   | ✗      | 61516.0    | 15.76   | 10.97         |
| micro                    | 9.4.1   | ✗      | 61304.8    | 15.81   | 10.93         |
| server-base              | 7.1.32  | ✗      | 60093.6    | 16.14   | 10.72         |
| yeps                     | 1.1.1   | ✗      | 58258.4    | 16.67   | 10.39         |
| micro-route              | 2.5.0   | ✓      | 57098.4    | 17.01   | 10.18         |
| server-base-router       | 6.1.5   | ✓      | 56759.2    | 17.12   | 10.12         |
| connect-router           | 1.3.8   | ✓      | 55104.0    | 17.65   | 9.83          |
| trek-engine              | 1.0.5   | ✗      | 54028.0    | 18.01   | 8.86          |
| trek-router              | 1.2.0   | ✓      | 52559.2    | 18.53   | 8.62          |
| spirit                   | 0.6.1   | ✗      | 48397.6    | 20.19   | 8.63          |
| yeps-router              | 1.2.0   | ✓      | 47652.8    | 20.49   | 8.50          |
| vapr                     | 0.5.5   | ✓      | 46958.4    | 20.80   | 7.70          |
| koa                      | 2.15.3  | ✗      | 44988.8    | 21.73   | 8.02          |
| spirit-router            | 0.5.0   | ✓      | 43178.4    | 22.67   | 7.70          |
| total.js                 | 3.4.13  | ✓      | 41834.4    | 23.40   | 12.81         |
| restify                  | 8.6.1   | ✓      | 41524.8    | 23.58   | 7.48          |
| koa-router               | 10.1.1  | ✓      | 40999.2    | 23.89   | 7.31          |
| hapi                     | 20.3.0  | ✓      | 35502.6    | 27.66   | 6.33          |
| microrouter              | 3.1.3   | ✓      | 33181.4    | 29.64   | 5.92          |
| express                  | 4.19.2  | ✓      | 14788.4    | 67.08   | 2.64          |
| fastify-big-json         | 3.29.5  | ✓      | 13022.8    | 76.24   | 149.83        |
| express-with-middlewares | 4.19.2  | ✓      | 12546.4    | 79.14   | 4.81          |
| express-route-prefix     | 4.19.2  | ✓      | 11151.8    | 89.11   | 4.13          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
