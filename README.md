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
* __Machine:__ Linux fv-az58-467 5.4.0-1032-azure #33~18.04.1-Ubuntu SMP Tue Nov 17 11:40:52 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.20.0`
* __Run:__ Sat Dec 19 03:44:54 UTC 2020

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.9.2   | ✓      | 69495.6    | 13.90   | 12.39         |
| polkadot                 | 1.0.0   | ✗      | 68900.4    | 14.03   | 12.29         |
| foxify                   | 0.10.20 | ✓      | 66461.2    | 14.53   | 10.90         |
| bare                     | 10.13.0 | ✗      | 66037.2    | 14.65   | 11.78         |
| connect                  | 3.7.0   | ✗      | 64588.0    | 14.98   | 11.52         |
| polka                    | 0.5.2   | ✓      | 64055.2    | 15.10   | 11.42         |
| rayo                     | 1.3.6   | ✓      | 63976.4    | 15.13   | 11.41         |
| 0http                    | 3.0.0   | ✓      | 63926.0    | 15.15   | 11.40         |
| micro                    | 9.3.4   | ✗      | 62918.4    | 15.40   | 11.22         |
| server-base              | 7.1.23  | ✗      | 62792.0    | 15.42   | 11.20         |
| micro-route              | 2.5.0   | ✓      | 59732.0    | 16.25   | 10.65         |
| restana                  | 4.8.1   | ✓      | 59364.8    | 16.35   | 10.59         |
| yeps                     | 1.1.1   | ✗      | 58895.2    | 16.48   | 10.50         |
| server-base-router       | 6.1.5   | ✓      | 57897.6    | 16.77   | 10.33         |
| connect-router           | 1.3.5   | ✓      | 57895.2    | 16.78   | 10.32         |
| trek-router              | 1.2.0   | ✓      | 56473.6    | 17.21   | 9.26          |
| vapr                     | 0.5.5   | ✓      | 55564.8    | 17.50   | 9.11          |
| trek-engine              | 1.0.5   | ✗      | 52910.4    | 18.41   | 8.68          |
| yeps-router              | 1.2.0   | ✓      | 50493.6    | 19.31   | 9.00          |
| koa                      | 2.13.0  | ✗      | 46812.0    | 20.86   | 8.35          |
| total.js                 | 3.4.6   | ✓      | 45085.6    | 21.68   | 13.80         |
| spirit-router            | 0.5.0   | ✓      | 44620.0    | 21.93   | 7.96          |
| spirit                   | 0.6.1   | ✗      | 42900.0    | 22.82   | 7.65          |
| koa-router               | 10.0.0  | ✓      | 41587.2    | 23.55   | 7.42          |
| restify                  | 8.5.1   | ✓      | 41307.2    | 23.71   | 7.45          |
| hapi                     | 20.0.3  | ✓      | 34329.4    | 28.62   | 6.12          |
| microrouter              | 3.1.3   | ✓      | 31984.4    | 30.77   | 5.70          |
| egg.js                   | 2.29.1  | ✓      | 19697.7    | 50.26   | 6.93          |
| express                  | 4.17.1  | ✓      | 13336.8    | 74.44   | 2.38          |
| express-with-middlewares | 4.17.1  | ✓      | 11373.2    | 87.36   | 4.36          |
| express-route-prefix     | 4.17.1  | ✓      | 10836.8    | 91.73   | 4.01          |
| fastify-big-json         | 3.9.2   | ✓      | 10647.2    | 93.34   | 122.49        |
| farrow-http              | 1.3.0   | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
