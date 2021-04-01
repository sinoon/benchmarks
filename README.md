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
* __Machine:__ Linux fv-az150-728 5.4.0-1041-azure #43-Ubuntu SMP Fri Feb 26 10:21:20 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.21.0`
* __Run:__ Thu Apr  1 03:23:35 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 43418.4    | 22.53   | 7.74          |
| micro                    | 9.3.4   | ✗      | 41616.0    | 23.53   | 7.42          |
| bare                     | 10.13.0 | ✗      | 41452.8    | 23.63   | 7.39          |
| fastify                  | 3.14.1  | ✓      | 39613.6    | 24.75   | 7.06          |
| polka                    | 0.5.2   | ✓      | 39612.0    | 24.75   | 7.06          |
| rayo                     | 1.3.6   | ✓      | 38840.8    | 25.24   | 6.93          |
| foxify                   | 0.10.20 | ✓      | 38566.2    | 25.43   | 6.33          |
| spirit-router            | 0.5.0   | ✓      | 38415.8    | 25.58   | 6.85          |
| connect                  | 3.7.0   | ✗      | 37700.6    | 26.03   | 6.72          |
| server-base              | 7.1.23  | ✗      | 37256.0    | 26.35   | 6.64          |
| yeps                     | 1.1.1   | ✗      | 36845.6    | 26.64   | 6.57          |
| 0http                    | 3.1.0   | ✓      | 35633.2    | 27.62   | 6.35          |
| spirit                   | 0.6.1   | ✗      | 34736.6    | 28.33   | 6.19          |
| server-base-router       | 6.1.5   | ✓      | 34485.0    | 28.50   | 6.15          |
| micro-route              | 2.5.0   | ✓      | 34361.0    | 28.60   | 6.13          |
| restana                  | 4.8.1   | ✓      | 34258.2    | 28.69   | 6.11          |
| connect-router           | 1.3.5   | ✓      | 33601.8    | 29.27   | 5.99          |
| yeps-router              | 1.2.0   | ✓      | 32373.6    | 30.38   | 5.77          |
| trek-engine              | 1.0.5   | ✗      | 31559.6    | 31.18   | 5.18          |
| trek-router              | 1.2.0   | ✓      | 31114.6    | 31.64   | 5.10          |
| koa                      | 2.13.1  | ✗      | 29809.6    | 33.04   | 5.32          |
| vapr                     | 0.5.5   | ✓      | 28956.0    | 34.03   | 4.75          |
| restify                  | 8.5.1   | ✓      | 26388.8    | 37.39   | 4.76          |
| total.js                 | 3.4.8   | ✓      | 25320.0    | 38.99   | 7.75          |
| koa-router               | 10.0.0  | ✓      | 24932.4    | 39.60   | 4.45          |
| hapi                     | 20.1.2  | ✓      | 21233.6    | 46.58   | 3.79          |
| microrouter              | 3.1.3   | ✓      | 19268.8    | 51.39   | 3.44          |
| egg.js                   | 2.29.3  | ✓      | 13931.0    | 71.29   | 4.90          |
| express                  | 4.17.1  | ✓      | 8170.8     | 121.79  | 1.46          |
| fastify-big-json         | 3.14.1  | ✓      | 8163.1     | 121.87  | 93.91         |
| express-route-prefix     | 4.17.1  | ✓      | 7337.3     | 135.67  | 2.71          |
| express-with-middlewares | 4.17.1  | ✓      | 7181.9     | 138.60  | 2.75          |
| farrow-http              | 1.8.10  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
