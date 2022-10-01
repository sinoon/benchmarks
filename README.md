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
* __Machine:__ Linux fv-az343-100 5.15.0-1020-azure #25~20.04.1-Ubuntu SMP Thu Sep 1 19:20:56 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Oct  1 01:18:22 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 71621.2    | 13.47   | 12.77         |
| rayo                     | 1.3.10  | ✓      | 68022.0    | 14.19   | 12.13         |
| fastify                  | 3.29.2  | ✓      | 67908.4    | 14.22   | 12.11         |
| bare                     | 10.13.0 | ✗      | 67349.6    | 14.34   | 12.01         |
| polka                    | 0.5.2   | ✓      | 66810.4    | 14.46   | 11.91         |
| foxify                   | 0.10.20 | ✓      | 66704.4    | 14.48   | 10.94         |
| 0http                    | 3.4.1   | ✓      | 66150.8    | 14.62   | 11.80         |
| server-base              | 7.1.32  | ✗      | 65970.0    | 14.66   | 11.77         |
| connect                  | 3.7.0   | ✗      | 64279.2    | 15.06   | 11.46         |
| micro                    | 9.4.1   | ✗      | 63056.8    | 15.36   | 11.25         |
| yeps                     | 1.1.1   | ✗      | 63008.8    | 15.37   | 11.24         |
| restana                  | 4.9.6   | ✓      | 62758.4    | 15.44   | 11.19         |
| server-base-router       | 6.1.5   | ✓      | 61660.8    | 15.72   | 11.00         |
| connect-router           | 1.3.7   | ✓      | 58484.0    | 16.60   | 10.43         |
| micro-route              | 2.5.0   | ✓      | 57772.8    | 16.81   | 10.30         |
| trek-router              | 1.2.0   | ✓      | 55883.2    | 17.40   | 9.17          |
| trek-engine              | 1.0.5   | ✗      | 55818.4    | 17.42   | 9.16          |
| yeps-router              | 1.2.0   | ✓      | 50860.0    | 19.16   | 9.07          |
| vapr                     | 0.5.5   | ✓      | 50555.2    | 19.29   | 8.29          |
| koa                      | 2.13.4  | ✗      | 47160.0    | 20.70   | 8.41          |
| spirit                   | 0.6.1   | ✗      | 47047.2    | 20.77   | 8.39          |
| spirit-router            | 0.5.0   | ✓      | 44938.4    | 21.76   | 8.01          |
| total.js                 | 3.4.13  | ✓      | 43840.0    | 22.31   | 13.42         |
| restify                  | 8.6.1   | ✓      | 43468.0    | 22.51   | 7.83          |
| koa-router               | 10.1.1  | ✓      | 42604.8    | 22.97   | 7.60          |
| hapi                     | 20.2.2  | ✓      | 36225.8    | 27.10   | 6.46          |
| microrouter              | 3.1.3   | ✓      | 34668.2    | 28.34   | 6.18          |
| egg.js                   | 2.37.0  | ✓      | 20743.6    | 47.71   | 7.30          |
| express                  | 4.18.1  | ✓      | 14117.2    | 70.29   | 2.52          |
| express-with-middlewares | 4.18.1  | ✓      | 12388.8    | 80.16   | 4.75          |
| express-route-prefix     | 4.18.1  | ✓      | 12164.6    | 81.67   | 4.50          |
| fastify-big-json         | 3.29.2  | ✓      | 11435.2    | 86.87   | 131.57        |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
