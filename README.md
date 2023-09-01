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
* __Machine:__ Linux fv-az674-806 5.15.0-1041-azure #48-Ubuntu SMP Tue Jun 20 20:34:08 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri Sep  1 01:03:40 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 70624.4    | 13.67   | 12.59         |
| fastify                  | 3.29.5  | ✓      | 68282.0    | 14.14   | 12.18         |
| bare                     | 10.13.0 | ✗      | 66905.6    | 14.44   | 11.93         |
| 0http                    | 3.5.2   | ✓      | 65739.2    | 14.71   | 11.72         |
| polka                    | 0.5.2   | ✓      | 63740.8    | 15.20   | 11.37         |
| connect                  | 3.7.0   | ✗      | 63197.6    | 15.33   | 11.27         |
| micro                    | 9.4.1   | ✗      | 61349.6    | 15.81   | 10.94         |
| yeps                     | 1.1.1   | ✗      | 60473.6    | 16.04   | 10.78         |
| server-base              | 7.1.32  | ✗      | 60275.2    | 16.09   | 10.75         |
| server-base-router       | 6.1.5   | ✓      | 58847.2    | 16.50   | 10.49         |
| restana                  | 4.9.7   | ✓      | 57679.2    | 16.85   | 10.29         |
| micro-route              | 2.5.0   | ✓      | 57172.8    | 16.99   | 10.20         |
| connect-router           | 1.3.8   | ✓      | 56692.8    | 17.15   | 10.11         |
| trek-router              | 1.2.0   | ✓      | 53981.6    | 18.03   | 8.85          |
| trek-engine              | 1.0.5   | ✗      | 53718.4    | 18.13   | 8.81          |
| vapr                     | 0.5.5   | ✓      | 49289.6    | 19.79   | 8.08          |
| yeps-router              | 1.2.0   | ✓      | 48797.6    | 20.00   | 8.70          |
| foxify                   | 0.10.20 | ✓      | 48000.0    | 20.33   | 7.87          |
| koa                      | 2.14.2  | ✗      | 45995.2    | 21.25   | 8.20          |
| spirit                   | 0.6.1   | ✗      | 45864.0    | 21.31   | 8.18          |
| spirit-router            | 0.5.0   | ✓      | 44465.6    | 22.00   | 7.93          |
| total.js                 | 3.4.13  | ✓      | 43313.6    | 22.59   | 13.26         |
| restify                  | 8.6.1   | ✓      | 43044.8    | 22.74   | 7.76          |
| koa-router               | 10.1.1  | ✓      | 41751.4    | 23.46   | 7.45          |
| hapi                     | 20.3.0  | ✓      | 35868.4    | 27.38   | 6.40          |
| microrouter              | 3.1.3   | ✓      | 34747.4    | 28.28   | 6.20          |
| express                  | 4.18.2  | ✓      | 14363.0    | 69.13   | 2.56          |
| express-with-middlewares | 4.18.2  | ✓      | 12483.8    | 79.54   | 4.79          |
| express-route-prefix     | 4.18.2  | ✓      | 11848.6    | 83.89   | 4.38          |
| fastify-big-json         | 3.29.5  | ✓      | 11182.4    | 88.90   | 128.65        |
| egg.js                   | 2.37.0  | ✓      | 8348.4     | 119.21  | 2.94          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
