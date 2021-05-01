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
* __Machine:__ Linux fv-az180-946 5.4.0-1046-azure #48-Ubuntu SMP Tue Apr 13 07:18:42 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.1`
* __Run:__ Sat May  1 00:56:10 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.15.1  | ✓      | 43152.0    | 22.67   | 7.70          |
| foxify                   | 0.10.20 | ✓      | 42852.8    | 22.84   | 7.03          |
| micro                    | 9.3.4   | ✗      | 41469.6    | 23.62   | 7.40          |
| polkadot                 | 1.0.0   | ✗      | 41336.0    | 23.69   | 7.37          |
| bare                     | 10.13.0 | ✗      | 37931.4    | 25.88   | 6.76          |
| 0http                    | 3.1.0   | ✓      | 36084.2    | 27.22   | 6.43          |
| yeps                     | 1.1.1   | ✗      | 36064.6    | 27.23   | 6.43          |
| rayo                     | 1.3.6   | ✓      | 35666.2    | 27.54   | 6.36          |
| connect                  | 3.7.0   | ✗      | 34983.2    | 28.09   | 6.24          |
| spirit                   | 0.6.1   | ✗      | 34310.2    | 28.71   | 6.12          |
| server-base              | 7.1.27  | ✗      | 34304.4    | 28.65   | 6.12          |
| polka                    | 0.5.2   | ✓      | 33731.0    | 29.14   | 6.02          |
| trek-router              | 1.2.0   | ✓      | 33424.6    | 29.42   | 5.48          |
| restana                  | 4.8.1   | ✓      | 33364.4    | 29.47   | 5.95          |
| spirit-router            | 0.5.0   | ✓      | 32909.6    | 29.93   | 5.87          |
| micro-route              | 2.5.0   | ✓      | 32737.6    | 30.04   | 5.84          |
| server-base-router       | 6.1.5   | ✓      | 32527.8    | 30.24   | 5.80          |
| yeps-router              | 1.2.0   | ✓      | 30738.0    | 32.04   | 5.48          |
| trek-engine              | 1.0.5   | ✗      | 30324.6    | 32.47   | 4.97          |
| connect-router           | 1.3.5   | ✓      | 29544.0    | 33.34   | 5.27          |
| koa                      | 2.13.1  | ✗      | 29140.0    | 33.82   | 5.20          |
| vapr                     | 0.5.5   | ✓      | 27080.8    | 36.42   | 4.44          |
| restify                  | 8.5.1   | ✓      | 26672.8    | 36.99   | 4.81          |
| total.js                 | 3.4.8   | ✓      | 24634.8    | 40.09   | 7.54          |
| koa-router               | 10.0.0  | ✓      | 23234.5    | 42.53   | 4.14          |
| hapi                     | 20.1.2  | ✓      | 21286.0    | 46.46   | 3.80          |
| microrouter              | 3.1.3   | ✓      | 19333.6    | 51.24   | 3.45          |
| egg.js                   | 2.29.4  | ✓      | 13225.8    | 75.07   | 4.65          |
| express                  | 4.17.1  | ✓      | 8550.9     | 116.34  | 1.52          |
| fastify-big-json         | 3.15.1  | ✓      | 8326.6     | 119.47  | 95.79         |
| express-with-middlewares | 4.17.1  | ✓      | 7767.1     | 128.10  | 2.98          |
| express-route-prefix     | 4.17.1  | ✓      | 7266.1     | 137.01  | 2.69          |
| farrow-http              | 1.10.3  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
