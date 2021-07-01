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
* __Machine:__ Linux fv-az238-641 5.8.0-1036-azure #38~20.04.1-Ubuntu SMP Thu Jun 17 14:14:18 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.1`
* __Run:__ Thu Jul  1 01:20:02 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| bare                     | 10.13.0 | ✗      | 66690.0    | 14.51   | 11.89         |
| 0http                    | 3.1.1   | ✓      | 65837.2    | 14.70   | 11.74         |
| micro                    | 9.3.4   | ✗      | 64036.0    | 15.14   | 11.42         |
| server-base              | 7.1.27  | ✗      | 62065.6    | 15.61   | 11.07         |
| yeps                     | 1.1.1   | ✗      | 60676.0    | 15.99   | 10.82         |
| connect-router           | 1.3.5   | ✓      | 60036.8    | 16.16   | 10.71         |
| micro-route              | 2.5.0   | ✓      | 58162.4    | 16.70   | 10.37         |
| trek-router              | 1.2.0   | ✓      | 56062.4    | 17.34   | 9.20          |
| spirit                   | 0.6.1   | ✗      | 53143.2    | 18.34   | 9.48          |
| yeps-router              | 1.2.0   | ✓      | 48592.8    | 20.09   | 8.67          |
| koa                      | 2.13.1  | ✗      | 48260.8    | 20.22   | 8.61          |
| restify                  | 8.5.1   | ✓      | 35276.7    | 27.97   | 6.36          |
| polka                    | 0.5.2   | ✓      | 35141.8    | 28.09   | 6.27          |
| rayo                     | 1.3.6   | ✓      | 34060.9    | 28.88   | 6.07          |
| koa-router               | 10.0.0  | ✓      | 32359.3    | 30.46   | 5.77          |
| vapr                     | 0.5.5   | ✓      | 31617.6    | 31.25   | 5.19          |
| spirit-router            | 0.5.0   | ✓      | 27790.0    | 35.91   | 4.96          |
| microrouter              | 3.1.3   | ✓      | 24687.4    | 40.46   | 4.40          |
| restana                  | 4.9.1   | ✓      | 23981.9    | 41.77   | 4.28          |
| fastify                  | 3.18.1  | ✓      | 22746.4    | 43.58   | 4.06          |
| polkadot                 | 1.0.0   | ✗      | 22596.7    | 43.95   | 4.03          |
| foxify                   | 0.10.20 | ✓      | 20650.5    | 48.01   | 3.39          |
| connect                  | 3.7.0   | ✗      | 20554.5    | 48.29   | 3.67          |
| server-base-router       | 6.1.5   | ✓      | 20282.5    | 48.79   | 3.62          |
| trek-engine              | 1.0.5   | ✗      | 17731.4    | 55.95   | 2.91          |
| total.js                 | 3.4.9   | ✓      | 16637.2    | 59.59   | 5.09          |
| egg.js                   | 2.29.4  | ✓      | 15887.7    | 62.86   | 5.59          |
| hapi                     | 20.1.5  | ✓      | 12826.4    | 77.41   | 2.29          |
| express                  | 4.17.1  | ✓      | 11761.0    | 84.48   | 2.10          |
| express-with-middlewares | 4.17.1  | ✓      | 10519.5    | 94.49   | 4.03          |
| fastify-big-json         | 3.18.1  | ✓      | 7775.7     | 127.75  | 89.46         |
| express-route-prefix     | 4.17.1  | ✓      | 4963.9     | 200.42  | 1.84          |
| farrow-http              | 1.10.9  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
