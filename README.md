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
* __Machine:__ Linux fv-az246-953 5.13.0-1031-azure #37~20.04.1-Ubuntu SMP Mon Jun 13 22:51:01 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Fri Jul  1 01:07:21 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 72465.2    | 13.31   | 12.92         |
| fastify                  | 3.29.0  | ✓      | 71436.4    | 13.52   | 12.74         |
| bare                     | 10.13.0 | ✗      | 71014.8    | 13.62   | 12.66         |
| 0http                    | 3.4.1   | ✓      | 70604.4    | 13.67   | 12.59         |
| foxify                   | 0.10.20 | ✓      | 69231.6    | 13.94   | 11.36         |
| polka                    | 0.5.2   | ✓      | 68835.6    | 14.02   | 12.28         |
| rayo                     | 1.3.10  | ✓      | 68312.4    | 14.14   | 12.18         |
| connect                  | 3.7.0   | ✗      | 67782.4    | 14.25   | 12.09         |
| server-base              | 7.1.32  | ✗      | 66173.2    | 14.63   | 11.80         |
| micro                    | 9.3.4   | ✗      | 65486.4    | 14.77   | 11.68         |
| yeps                     | 1.1.1   | ✗      | 65167.2    | 14.84   | 11.62         |
| restana                  | 4.9.6   | ✓      | 64462.8    | 15.00   | 11.50         |
| connect-router           | 1.3.7   | ✓      | 63211.2    | 15.32   | 11.27         |
| micro-route              | 2.5.0   | ✓      | 61740.8    | 15.70   | 11.01         |
| server-base-router       | 6.1.5   | ✓      | 59144.0    | 16.41   | 10.55         |
| trek-router              | 1.2.0   | ✓      | 58622.4    | 16.56   | 9.62          |
| trek-engine              | 1.0.5   | ✗      | 58223.2    | 16.68   | 9.55          |
| vapr                     | 0.5.5   | ✓      | 52471.2    | 18.56   | 8.61          |
| yeps-router              | 1.2.0   | ✓      | 51640.8    | 18.87   | 9.21          |
| spirit                   | 0.6.1   | ✗      | 51422.4    | 18.96   | 9.17          |
| koa                      | 2.13.4  | ✗      | 48722.4    | 20.03   | 8.69          |
| spirit-router            | 0.5.0   | ✓      | 48676.8    | 20.05   | 8.68          |
| total.js                 | 3.4.13  | ✓      | 45794.4    | 21.34   | 14.02         |
| restify                  | 8.6.1   | ✓      | 44324.8    | 22.08   | 7.99          |
| koa-router               | 10.1.1  | ✓      | 43631.2    | 22.42   | 7.78          |
| hapi                     | 20.2.2  | ✓      | 37450.4    | 26.20   | 6.68          |
| microrouter              | 3.1.3   | ✓      | 35793.4    | 27.43   | 6.38          |
| egg.js                   | 2.36.0  | ✓      | 21512.4    | 45.97   | 7.57          |
| express                  | 4.18.1  | ✓      | 14715.2    | 67.42   | 2.62          |
| express-route-prefix     | 4.18.1  | ✓      | 12651.8    | 78.48   | 4.68          |
| express-with-middlewares | 4.18.1  | ✓      | 12634.4    | 78.59   | 4.84          |
| fastify-big-json         | 3.29.0  | ✓      | 11883.8    | 83.60   | 136.70        |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
