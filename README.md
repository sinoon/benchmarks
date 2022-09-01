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
* __Machine:__ Linux fv-az213-324 5.15.0-1017-azure #20~20.04.1-Ubuntu SMP Fri Aug 5 12:16:53 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu Sep  1 01:06:29 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| bare                     | 10.13.0 | ✗      | 56352.8    | 17.26   | 10.05         |
| fastify                  | 3.29.2  | ✓      | 56305.6    | 17.28   | 10.04         |
| polka                    | 0.5.2   | ✓      | 54412.8    | 17.89   | 9.70          |
| polkadot                 | 1.0.0   | ✗      | 54076.0    | 18.01   | 9.64          |
| rayo                     | 1.3.10  | ✓      | 53802.4    | 18.10   | 9.60          |
| foxify                   | 0.10.20 | ✓      | 53704.0    | 18.12   | 8.81          |
| micro                    | 9.4.1   | ✗      | 52725.6    | 18.46   | 9.40          |
| 0http                    | 3.4.1   | ✓      | 51966.4    | 18.76   | 9.27          |
| connect                  | 3.7.0   | ✗      | 51960.6    | 18.75   | 9.27          |
| server-base              | 7.1.32  | ✗      | 51692.0    | 18.85   | 9.22          |
| yeps                     | 1.1.1   | ✗      | 51283.2    | 19.00   | 9.15          |
| micro-route              | 2.5.0   | ✓      | 49266.4    | 19.81   | 8.79          |
| connect-router           | 1.3.7   | ✓      | 49054.4    | 19.89   | 8.75          |
| server-base-router       | 6.1.5   | ✓      | 47909.6    | 20.37   | 8.54          |
| restana                  | 4.9.6   | ✓      | 47195.2    | 20.69   | 8.42          |
| trek-router              | 1.2.0   | ✓      | 45913.0    | 21.30   | 7.53          |
| trek-engine              | 1.0.5   | ✗      | 44904.8    | 21.78   | 7.37          |
| vapr                     | 0.5.5   | ✓      | 39936.0    | 24.54   | 6.55          |
| yeps-router              | 1.2.0   | ✓      | 39834.4    | 24.61   | 7.10          |
| koa                      | 2.13.4  | ✗      | 38534.8    | 25.45   | 6.87          |
| spirit                   | 0.6.1   | ✗      | 36705.0    | 26.75   | 6.55          |
| total.js                 | 3.4.13  | ✓      | 36579.8    | 26.84   | 11.20         |
| spirit-router            | 0.5.0   | ✓      | 34865.2    | 28.20   | 6.22          |
| koa-router               | 10.1.1  | ✓      | 34513.8    | 28.48   | 6.16          |
| restify                  | 8.6.1   | ✓      | 34429.0    | 28.54   | 6.21          |
| hapi                     | 20.2.2  | ✓      | 28559.2    | 34.51   | 5.09          |
| microrouter              | 3.1.3   | ✓      | 26513.6    | 37.21   | 4.73          |
| egg.js                   | 2.36.0  | ✓      | 17723.7    | 55.88   | 6.24          |
| express                  | 4.18.1  | ✓      | 10698.8    | 92.90   | 1.91          |
| express-with-middlewares | 4.18.1  | ✓      | 9152.0     | 108.70  | 3.51          |
| fastify-big-json         | 3.29.2  | ✓      | 8525.4     | 116.66  | 98.08         |
| express-route-prefix     | 4.18.1  | ✓      | 8448.0     | 117.77  | 3.13          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
